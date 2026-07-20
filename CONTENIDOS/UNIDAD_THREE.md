# 🚀 Guía Práctica de Programación: Modularidad y Estructuras de Arreglos

Este repositorio contiene una explicación académica, clara y totalmente estructurada de los conceptos fundamentales de **Modularidad** y **Arreglos**, acompañados de sus respectivos ejemplos prácticos individuales en C++.

---

## 📌 PARTE 1: Modularidad y Transmisión de Parámetros

La **modularidad** consiste en dividir un problema grande en partes más pequeñas y autónomas llamadas **módulos** (o funciones). Para comunicarse, las funciones intercambian datos a través de **parámetros** usando dos métodos fundamentales:

* **Paso por Valor:** La función recibe una **copia** del dato original. Cualquier cambio hecho dentro de la función **no afecta** a la variable externa.
* **Paso por Referencia:** La función recibe la **dirección de memoria** real del dato (usando el símbolo `&`). Cualquier cambio hecho dentro de la función **sí afecta** a la variable externa.

### 💻 Código 1: Demostración de Parámetros

```cpp

#include <iostream>
using namespace std;

// Función por Valor: Trabaja con una copia
void cambiarPorValor(int x) {
    x = 99; // Solo modifica la copia local
}

// Función por Referencia: Trabaja con el dato original
void cambiarPorReferencia(int &x) {
    x = 99; // Modifica la variable externa real
}

int main() {
    int numero = 10;

    cout << "=== PRUEBA DE PARÁMETROS ===" << endl;
    cout << "Valor inicial de la variable: " << numero << endl;

    // 1. Ejecución Paso por Valor
    cambiarPorValor(numero);
    cout << "Resultado por Valor: " << numero << " (No cambio)" << endl; 

    // 2. Ejecución Paso por Referencia
    cambiarPorReferencia(numero);
    cout << "Resultado por Referencia: " << numero << " (Si cambio)" << endl; 

    return 0;
}

```
# 🚀 Guía Fundamental de Programación: Modularidad y Arreglos

Este repositorio contiene una explicación académica y simplificada de la **Modularidad** y los **Arreglos**. Los ejemplos de código en C++ se han reducido a su estructura más básica posible para facilitar la comprensión directa de la teoría.

---

## 📌 PARTE 1: Modularidad y Transmisión de Parámetros

La **modularidad** es el principio de diseño que consiste en dividir un programa en partes pequeñas llamadas **módulos** (funciones). Las funciones intercambian datos mediante **parámetros**. Existen dos formas básicas de transmitir estos datos:

### 🅰️ Paso por Valor
* **Teoría:** La función recibe una **copia** del dato. La variable original fuera de la función no sufre ningún cambio.

```cpp
#include <iostream>
using namespace std;

void funcionValor(int x) {
    x = 20; // Solo cambia la copia dentro de la función
}

int main() {
    int numero = 10;
    funcionValor(numero);
    cout << "Paso por Valor: " << numero << endl; // Imprime 10 (No cambió)
    return 0;
}
```

---

### 🅱️ Paso por Referencia
* **Teoría:** La función recibe la **dirección real** de la variable usando el símbolo `&`. Cualquier cambio dentro de la función modifica la variable original.

```cpp
#include <iostream>
using namespace std;

void funcionReferencia(int &x) {
    x = 20; // Modifica la variable original externa
}

int main() {
    int numero = 10;
    funcionReferencia(numero);
    cout << "Paso por Referencia: " << numero << endl; // Imprime 20 (Sí cambió)
    return 0;
}
```

---
---

## 📌 PARTE 2: Estructuras de Datos - Arreglos (Arrays)

Un **arreglo** es una colección de datos del **mismo tipo** (homogénea) y de tamaño **fijo** (estática). Se accede a cada elemento mediante un **índice** numérico que siempre inicia en `0`.

### 1️⃣ Arreglo Unidimensional (Vector)
* **Teoría:** Es una lista simple de una sola dimensión. Solo requiere **un índice** `[i]` para acceder al dato.

```cpp
#include <iostream>
using namespace std;

int main() {
    // Un vector con 3 elementos
    int vector[3] = {10, 20, 30};

    // Acceso directo por índice
    cout << "Indice 0: " << vector[0] << endl; // Imprime 10
    cout << "Indice 2: " << vector[2] << endl; // Imprime 30

    return 0;
}
```

---

### 2️⃣ Arreglo Bidimensional (Matriz)
* **Teoría:** Estructura organizada en **filas y columnas** (como una tabla). Requiere **dos índices** `[fila][columna]` para localizar un dato.

```cpp
#include <iostream>
using namespace std;

int main() {
    // Matriz de 2 filas y 2 columnas
    int matriz[2][2] = {
        {5, 8},  // Fila 0
        {4, 9}   // Fila 1
    };

    // Acceso directo indicando [Fila][Columna]
    cout << "Fila 0, Columna 1: " << matriz[0][1] << endl; // Imprime 8
    cout << "Fila 1, Columna 0: " << matriz[1][0] << endl; // Imprime 4

    return 0;
}
```

---

### 3️⃣ Arreglo Multidimensional (Tridimensional)
* **Teoría:** Estructuras de tres o más dimensiones. Una matriz 3D se puede ver como un **cubo de datos** o un conjunto de matrices apiladas. Requiere **tres índices** `[capa][fila][columna]`.

```cpp
#include <iostream>
using namespace std;

int main() {
    // Arreglo 3D de tamaño 2x2x2 (2 Capas, 2 Filas, 2 Columnas)
    int cubo[2][2][2] = {
        { {1, 2}, {3, 4} }, // Capa 0
        { {5, 6}, {7, 8} }  // Capa 1
    };

    // Acceso directo indicando [Capa][Fila][Columna]
    cout << "Capa 0, Fila 1, Columna 0: " << cubo[0][1][0] << endl; // Imprime 3
    cout << "Capa 1, Fila 0, Columna 1: " << cubo[1][0][1] << endl; // Imprime 6

    return 0;
}
```

---

## 📊 Tablas de Resumen Visual

### Parámetros
| Tipo de Paso | ¿Qué recibe la función? | ¿Modifica el original? |
| :--- | :--- | :---: |
| **Por Valor** | Una copia del dato. | ❌ No |
| **Por Referencia** | La variable real (`&`). | ✅ Sí |

### Arreglos
| Tipo | Índices | Estructura |
| :--- | :---: | :--- |
| **Unidimensional** | `[i]` | Una sola fila (Lista). |
| **Bidimensional** | `[f][c]` | Una cuadrícula (Tabla de filas y columnas). |
| **Multidimensional**| `[x][y][z]` | Un bloque volumétrico (Cubo u objetos apilados). |

