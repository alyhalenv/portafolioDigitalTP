# 🚀 Guía Práctica de Programación: Modularidad y Estructuras de Arreglos

Este repositorio contiene una explicación académica, clara y totalmente estructurada de los conceptos fundamentales de **Modularidad** y **Arreglos**, acompañados de sus respectivos ejemplos prácticos individuales en C++.

---

## 📌 PARTE 1: Modularidad y Transmisión de Parámetros

La **modularidad** consiste en dividir un problema grande en partes más pequeñas y autónomas llamadas **módulos** (o funciones). Para comunicarse, las funciones intercambian datos a través de **parámetros** usando dos métodos fundamentales:

* **Paso por Valor:** La función recibe una **copia** del dato original. Cualquier cambio hecho dentro de la función **no afecta** a la variable externa.
* **Paso por Referencia:** La función recibe la **dirección de memoria** real del dato (usando el símbolo `&`). Cualquier cambio hecho dentro de la función **sí afecta** a la variable externa.

### 💻 Código 1: Demostración de Parámetros

```cpp

#include <stdio.h>

void valor(int x){
    x = 20;
}

void referencia(int *x){
    *x = 20;
}

int main(){

    int numero = 10;

    valor(numero);
    printf("%d\n", numero);

    referencia(&numero);
    printf("%d\n", numero);

    return 0;
}
```
<img width="741" height="76" alt="image" src="https://github.com/user-attachments/assets/e0c867f8-02de-4a33-9f16-dde3bef37d4e" />

# 🚀 Guía Fundamental de Programación: Modularidad y Arreglos

Este repositorio contiene una explicación académica y simplificada de la **Modularidad** y los **Arreglos**. Los ejemplos de código en C++ se han reducido a su estructura más básica posible para facilitar la comprensión directa de la teoría.

---

## 📌 PARTE 1: Modularidad y Transmisión de Parámetros

La **modularidad** es el principio de diseño que consiste en dividir un programa en partes pequeñas llamadas **módulos** (funciones). Las funciones intercambian datos mediante **parámetros**. Existen dos formas básicas de transmitir estos datos:

### 🅰️ Paso por Valor
* **Teoría:** La función recibe una **copia** del dato. La variable original fuera de la función no sufre ningún cambio.

```cpp
#include <stdio.h>

void valor(int x){
    x = 20;
}

int main(){

    int numero = 10;

    valor(numero);

    printf("%d\n", numero);

    return 0;
}
```
<img width="738" height="63" alt="image" src="https://github.com/user-attachments/assets/2c311960-275c-4bbe-b65a-0baa05a7fca7" />

---

### 🅱️ Paso por Referencia
* **Teoría:** La función recibe la **dirección real** de la variable usando el símbolo `&`. Cualquier cambio dentro de la función modifica la variable original.

```cpp
#include <stdio.h>

void referencia(int *x){
    *x = 20;
}

int main(){

    int numero = 10;

    referencia(&numero);

    printf("%d\n", numero);

    return 0;
}
```
<img width="736" height="62" alt="image" src="https://github.com/user-attachments/assets/b4dbca34-fa67-4666-bdc4-30cdde02c4b3" />

---
---

## 📌 PARTE 2: Estructuras de Datos - Arreglos (Arrays)

Un **arreglo** es una colección de datos del **mismo tipo** (homogénea) y de tamaño **fijo** (estática). Se accede a cada elemento mediante un **índice** numérico que siempre inicia en `0`.

### 1️⃣ Arreglo Unidimensional (Vector)
* **Teoría:** Es una lista simple de una sola dimensión. Solo requiere **un índice** `[i]` para acceder al dato.

```cpp
#include <stdio.h>

int main(){

    int vector[3] = {5, 10, 15};

    printf("%d\n", vector[0]);
    printf("%d\n", vector[2]);

    return 0;
}
```
<img width="738" height="82" alt="image" src="https://github.com/user-attachments/assets/e7b3ad8d-934a-4b46-8d09-c1db59cd4d4b" />

---

### 2️⃣ Arreglo Bidimensional (Matriz)
* **Teoría:** Estructura organizada en **filas y columnas** (como una tabla). Requiere **dos índices** `[fila][columna]` para localizar un dato.

```cpp
#include <stdio.h>

int main(){

    int matriz[2][2] = {
        {1, 2},
        {3, 4}
    };

    printf("%d\n", matriz[0][1]);
    printf("%d\n", matriz[1][0]);

    return 0;
}
```
<img width="743" height="70" alt="image" src="https://github.com/user-attachments/assets/a25754a7-fafd-413e-bbd3-38145d0db66c" />

---

### 3️⃣ Arreglo Multidimensional (Tridimensional)
* **Teoría:** Estructuras de tres o más dimensiones. Una matriz 3D se puede ver como un **cubo de datos** o un conjunto de matrices apiladas. Requiere **tres índices** `[capa][fila][columna]`.

```cpp
#include <stdio.h>

int main(){

    int cubo[2][2][2] = {
        {
            {1, 2},
            {3, 4}
        },
        {
            {5, 6},
            {7, 8}
        }
    };

    printf("%d\n", cubo[0][1][0]);
    printf("%d\n", cubo[1][0][1]);

    return 0;
}
```
<img width="740" height="65" alt="image" src="https://github.com/user-attachments/assets/2b516f0a-0148-499f-9c6a-936bc560dd0e" />

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

## 📌 PARTE 3: Principales Dificultades y Reflexión Crítica

La transición hacia la programación modular y el manejo de arreglos estáticos presenta retos conceptuales específicos durante su aplicación práctica.

### 1. Dificultades Técnicas Identificadas
* **Confusión en la Transmisión de Parámetros:** Durante del desarollo de la activida existiio una tendencia común a evitar el uso del operador de referencia (`&`) por temor a modificar accidentalmente los datos originales, lo que deriva en un uso ineficiente de copias en memoria (paso por valor).
* **El Desfase del Índice Cero (*Off-by-One Error*):** Otro de ello fue el olvidar que los arreglos inician estrictamente en el índice `0` genera errores frecuentes de desbordamiento de memoria (*segmentation fault*) al intentar acceder a la posición equivalente al tamaño total del arreglo.
* **Complejidad Multidimensional:** Y finalmente la coordinación de múltiples ciclos `for` anidados para recorrer arreglos bidimensionales y tridimensionales me representó una alta dificultad en durante el uso, pues existia una confusión incial en como lograr que cumpla esta función todos los espacios de la matriz o espacio.

### 2. Reflexión Crítica sobre el Aprendizaje

> 💡 **Diseño vs. Líneas de Código**
> La modularidad transforma la metodología de trabajo del desarrollador: se pasa de escribir código secuencial a diseñar una arquitectura basada en funciones independientes, mejorando la legibilidad y la reutilización del software.

Por otra parte, el estudio de los arreglos permite comprender las limitaciones físicas del hardware. Aunque el acceso indexado es sumamente veloz, la naturaleza **estática** de estas estructuras resulta rígida para escenarios reales donde el volumen de datos es impredecible. Esta restricción actúa como el puente conceptual necesario para justificar el uso futuro de la memoria dinámica.

---

## 📊 Matriz de Diagnóstico Rápido

| Error Común | Causa Técnica | Solución Práctica |
| :--- | :--- | :--- |
| Los cambios dentro de una función no se guardan en `main()`. | El parámetro se envió **por valor** (copia local). | Añadir el operador `&` en la función para usar **referencia**. |
| El programa muestra datos basura o se cierra inesperadamente. | El ciclo `for` intenta leer un índice que no existe. | Asegurar que la condición del ciclo sea menor estricto (`i < tamaño`). |
| Datos desalineados en matrices. | Inversión accidental en el orden de los índices. | Mantener el estándar estricto de acceso: `[fila][columna]`. |

<div align="center">

[⬅️ VOLVER A CONTENIDOS](./CONTENIDOS.MD)

</div>

