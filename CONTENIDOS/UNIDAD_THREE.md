# Introducción a la Modularidad y Transmisión de Parámetros

## 1. ¿Qué es la Modularidad?

La **modularidad** es el principio de diseño de software que consiste en dividir un programa grande en partes más pequeñas y autónomas llamadas **módulos** (o funciones). 

Su objetivo es aplicar la estrategia de *"divide y vencerás"*, permitiendo que el código sea más ordenado, fácil de entender, mantener y reutilizar.

---

## 2. Paso por Valor vs. Paso por Referencia

Para que los módulos se comuniquen entre sí, utilizan **parámetros** (datos que se pasan a las funciones). Existen dos formas fundamentales de transferir estos datos:

### A. Paso por Valor (Copia)
* **Definición:** La función recibe una **copia** del dato original.
* **Resultado:** Cualquier cambio que se haga dentro de la función **no afecta** a la variable original externa, ya que solo se modifica su réplica.

### B. Paso por Referencia (Original)
* **Definición:** La función recibe el acceso directo (la dirección de memoria) del dato original.
* **Resultado:** Cualquier cambio que se haga dentro de la función **sí afecta** y modifica de forma permanente a la variable original externa.

---

## 3. Ejemplo Práctico en C++

El siguiente código muestra la diferencia de forma directa y básica:

```cpp
#include <iostream>
using namespace std;

// Función por Valor: Recibe una copia
void cambiarPorValor(int x) {
    x = 99; // Solo cambia la copia local
}

// Función por Referencia: Recibe el dato original (usa el símbolo &)
void cambiarPorReferencia(int &x) {
    x = 99; // Cambia la variable original externa
}

int main() {
    int numero = 10;

    // Caso 1: Paso por Valor
    cambiarPorValor(numero);
    cout << "Resultado por Valor: " << numero << endl; 
    // Imprime 10 (El valor original NO cambió)

    // Caso 2: Paso por Referencia
    cambiarPorReferencia(numero);
    cout << "Resultado por Referencia: " << numero << endl; 
    // Imprime 99 (El valor original SÍ cambió)

    return 0;
}
