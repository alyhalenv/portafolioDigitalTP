# Fundamentos de la Programación: Modularidad y Mecanismos de Transmisión de Parámetros

## 1. Teoría de la Modularidad

La **modularidad** es un principio de diseño de software que consiste en la descomposición de un sistema informático en partes más pequeñas, independientes y diferenciadas, denominadas **módulos**. Cada uno de estos módulos se encarga de ejecutar una tarea específica y bien definida dentro del ecosistema del programa.

Este enfoque se fundamenta en el axioma metodológico de *"divide y vencerás"*, permitiendo abordar problemas complejos mediante la resolución de subproblemas más simples. 

### Beneficios Principales
* **Mantenibilidad:** Facilita la localización y corrección de errores, ya que las modificaciones en un módulo no alteran de forma imprevista el comportamiento de los demás.
* **Reutilización de Código:** Los módulos diseñados genéricamente pueden ser invocados en múltiples secciones del proyecto o incluso en desarrollos futuros.
* **Legibilidad:** Reduce la densidad del código principal, permitiendo una comprensión abstracta y estructurada del flujo del programa.
* **Alta Cohesión y Bajo Acoplamiento:** Idealmente, un módulo debe tener una alta cohesión (concentrado en una sola tarea) y un bajo acoplamiento (independencia estricta de otros módulos).

---

## 2. Mecanismos de Transmisión de Parámetros

En el ámbito de la programación modular, los módulos (funciones o procedimientos) requieren comunicarse entre sí a través del intercambio de datos. Esto se logra mediante la **transmisión de parámetros**. A continuación, se analizan los dos métodos fundamentales.

### A. Paso de Parámetros por Valor

En el paso por valor, la función recibe una **copia local** del argumento que se le transfiere. Desde una perspectiva de gestión de memoria, se asigna una nueva dirección de memoria para almacenar esta réplica. 

* **Comportamiento:** Cualquier modificación realizada sobre el parámetro dentro del ámbito (*scope*) de la función afectará únicamente a la copia local. 
* **Seguridad:** La variable original declarada en el entorno llamador permanece inmutable, garantizando la integridad de los datos externos.

### B. Paso de Parámetros por Referencia

En el paso por referencia, la función no recibe una copia, sino la **dirección de memoria explícita** de la variable original. 

* **Comportamiento:** El parámetro formal actúa como un alias o puntero directo a la variable del entorno llamador. Por lo tanto, cualquier operación o asignación efectuada dentro del módulo impactará de forma directa e inmediata a la variable original.
* **Eficiencia:** Es óptimo para manejar estructuras de datos voluminosas (como arreglos u objetos complejos), ya que evita el costo computacional de duplicar la información en memoria.

---

## 3. Demostración Práctica (Ejemplo en C++)

A continuación se presenta un programa en lenguaje C++ que ilustra de manera empírica la diferencia operativa entre ambos mecanismos de transmisión.

```cpp
#include <iostream>

// Prototipos de funciones
void demostrarPasoPorValor(int numero);
void demostrarPasoPorReferencia(int &numero);

int main() {
    int variableOriginal = 10;

    std::cout << "=== ESTADO INICIAL ===" << std::endl;
    std::cout << "Valor original de la variable: " << variableOriginal << "\n\n";

    // 1. Ejecución del paso por valor
    std::cout << "--- Ejecutando Paso por Valor ---" << std::endl;
    demostrarPasoPorValor(variableOriginal);
    std::cout << "Valor en main() despues de la funcion: " << variableOriginal << "\n\n";

    // 2. Ejecución del paso por referencia
    std::cout << "--- Ejecutando Paso por Referencia ---" << std::endl;
    demostrarPasoPorReferencia(variableOriginal);
    std::cout << "Valor en main() despues de la funcion: " << variableOriginal << "\n";

    return 0;
}

// Implementación: Recibe una copia (Paso por Valor)
void demostrarPasoPorValor(int numero) {
    numero = numero + 50; // Se modifica solo la copia local
    std::cout << "Valor modificado dentro de la funcion (copia): " << numero << std::endl;
}

// Implementación: Recibe la dirección de memoria (Paso por Referencia usando el operador &)
void demostrarPasoPorReferencia(int &numero) {
    numero = numero + 50; // Se modifica la variable original directamente
    std::cout << "Valor modificado dentro de la funcion (referencia): " << numero << std::endl;
}
