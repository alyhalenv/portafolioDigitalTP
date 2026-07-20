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

```cpp

# Estructuras de Datos: Arreglos (Arrays)

## 1. ¿Qué es un Arreglo?

En el ámbito de la ciencia de la computación, un **arreglo** (también conocido como *array*, vector o matriz) es una estructura de datos homogénea y estática. 

* **Homogénea:** Significa que todos los elementos almacenados dentro del arreglo deben ser estrictamente del mismo tipo de datos (por ejemplo, solo enteros, solo flotantes o solo caracteres).
* **Estática:** Su tamaño en memoria se define al momento de su creación y no puede cambiar durante la ejecución del programa.
* **Indexación:** Cada elemento ocupa una posición consecutiva en la memoria y se accede a él mediante un **índice** (el cual, en la mayoría de lenguajes, inicia siempre en `0`).

---

## 2. Tipos de Arreglos

Los arreglos se clasifican principalmente según el número de dimensiones (índices) que requieren para localizar un dato:

### A. Arreglos Unidimensionales (Vectores)
Tienen una sola dimensión. Se pueden imaginar como una sola fila o una lista simple de elementos. Solo necesitan **un índice** para acceder a cualquier dato.

### B. Arreglos Bidimensionales (Matrices)
Tienen dos dimensiones. Se estructuran en forma de tabla con **filas y columnas**. Para acceder a un elemento, se requieren **dos índices**: el primero especifica la fila y el segundo la columna.

*(Nota: Existen arreglos multidimensionales de 3 o más dimensiones, pero los unidimensionales y bidimensionales son los pilares fundamentales de la programación).*

---

## 3. Ejemplos Prácticos en C++

A continuación, se presentan dos ejemplos aislados y sumamente sencillos para entender cómo declarar, llenar y leer cada tipo de arreglo.

### Ejemplo 1: Arreglo Unidimensional (Vector)

```cpp
#include <iostream>
using namespace std;

int main() {
    // Declaración e inicialización de un vector de tamaño 3
    int calificaciones[3] = {85, 90, 95};

    cout << "=== ARREGLO UNIDIMENSIONAL ===" << endl;

    // Recorremos el arreglo con un solo ciclo 'for'
    for (int i = 0; i < 3; i++) {
        cout << "Estudiante " << i << " - Calificacion: " << calificaciones[i] << endl;
    }

    return 0;
}
