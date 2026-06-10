
# 🛠️ Estructuras de Control de Flujo: Condicionales y Repetitivas

Las estructuras de control son los pilares fundamentales de la lógica de programación. Permiten modificar el flujo lineal de un programa, tomando decisiones o repitiendo bloques de código según se cumplan o no determinadas condiciones.

---

## 1. 🔀 ESTRUCTURAS CONDICIONALES 

Permiten bifurcar el flujo de ejecución de un programa basándose en el resultado de una expresión lógica (verdadera o falsa).

### A. 🔹 Condicional Simple (Si-Entonces / If)
Es una estructura de control que evalúa una expresión lógica (una condición que solo puede ser verdadera o falsa). Si el resultado de la evaluación es verdadero, el flujo del programa se desvía temporalmente para ejecutar un bloque específico de instrucciones; si es falso, el programa ignora por completo dicho bloque y continúa con la ejecución de la siguiente línea de código inmediata.

<div align="center">

#### 📝 Estructura en Pseudocódigo

<img width="228" height="107" alt="image" src="https://github.com/user-attachments/assets/ce452a5e-c3c0-4998-9176-b461ea6a9bb8" />

#### 📊 Diagrama de flujo

<img width="403" height="235" alt="image" src="https://github.com/user-attachments/assets/6634d573-2128-4528-8340-ba6885e285d1" />

</div>

### B. 🔸 Condicional Doble: (Si-Entonces-Sino / If-Else)
A diferencia e la estructura simple, esta permite al programa elegir entre dos caminos o alternativas mutuamente excluyentes basados en el resultado de una condición. Si la expresión lógica es verdadera, se ejecuta obligatoriamente el primer bloque de instrucciones (rama del Entonces); si es falsa, se ejecuta un segundo bloque alternativo de instrucciones (rama del Sino).

<div align="center">

#### 📝 Estructura en Pseudocódigo

<img width="203" height="136" alt="image" src="https://github.com/user-attachments/assets/2da1fb82-8240-4b70-b1c4-c107cbd1615c" />

#### 📊 Diagrama de flujo

<img width="346" height="212" alt="image" src="https://github.com/user-attachments/assets/1279a3e0-1aa5-419a-927c-6c17236c7426" />

</div>

### C. 💠 Condicional Múltiple: (Según Sea / Switch)
Es una estructura de control de selección que evalúa el valor exacto de una variable o expresión frente a un conjunto de constantes o casos predefinidos. En lugar de evaluar expresiones booleanas complexes (como respuestas de verdadero/falso), compara de forma directa si el contenido de la variable coincide con alguna de las opciones disponibles para ejecutar el bloque de código asignado a ese caso específico. Por lo general, incluye una opción por defecto (De Otro Modo / Default) que se ejecuta únicamente si el valor de la variable no coincide con ninguno de los casos listados.

<div align="center">

#### 📝 Estructura en Pseudocódigo

<img width="243" height="206" alt="image" src="https://github.com/user-attachments/assets/093bf31c-5a89-4380-ad46-7e54b7ede118" />

#### 📊 Diagrama de flujo

<img width="447" height="290" alt="image" src="https://github.com/user-attachments/assets/aa3f8305-0d70-4098-9fa0-84e7973e5520" />

</div>

---


## 2. 🔄 ESTRUCTURAS REPETITIVAS

Las **estructuras de control de flujo** son los pilares fundamentales de la lógica de programación. Su función principal es **romper la ejecución lineal y secuencial** por defecto de un ordenador (que procesa el código línea por línea, de arriba hacia abajo). Al evaluar condiciones lógicas o matemáticas, estas herramientas otorgan al desarrollador la capacidad de reaccionar ante datos cambiantes mediante dos acciones clave: **bifurcar el camino** del programa (tomar decisiones) o **ciclar bloques de instrucciones** (repetir tareas monótonas) de forma totalmente automatizada.

---

### A. 🔁 Bucle Mientras (Mientras-Hacer / While)
Es una estructura clasificada como de "pre-prueba" o evaluación previa, debido a que tiene la particularidad de validar la expresión lógica obligatoriamente antes de permitir el ingreso al bloque de código interno. Si la condición matemática o lógica resulta ser falsa desde la primera comprobación, el cuerpo del bucle se descarta y nunca se ejecuta; por el contrario, si es verdadera, el ciclo se repetirá indefinidamente hasta que la condición deje de cumplirse por completo.

<div align="center">

#### 📝 Estructura en Pseudocódigo

<img width="246" height="101" alt="image" src="https://github.com/user-attachments/assets/6a1edf79-13ec-4d79-8f06-43532b3157de" />

#### 📊 Diagrama de flujo

<img width="356" height="237" alt="image" src="https://github.com/user-attachments/assets/b211cfaf-647e-4002-b1ee-4e972890a800" />

</div>

### B. ↩️ Bucle Repetir (Hacer-Cuando/ Do-While)
A diferencia radical del bucle analizado anteriormente, esta se consolida como una estructura de "post-prueba" o evaluación posterior. El compilador primero ejecuta el bloque de instrucciones designado y luego realiza la evaluación de la condición al final del camino; esto garantiza de forma estricta que el código interno se ejecute al menos una vez antes de que el programa verifique si se debe continuar con la siguiente iteración.

<div align="center">

#### 📝 Estructura en Pseudocódigo

<img width="281" height="110" alt="image" src="https://github.com/user-attachments/assets/50246726-e57b-411a-8366-f0d7cd84f0b9" />

#### 📊 Diagrama de flujo

<img width="368" height="202" alt="image" src="https://github.com/user-attachments/assets/2487f719-60c1-4e8d-9a23-87e28770e4f1" />

</div>

### C. 🔢 Bucle Para (Para-Hasta-Hacer / For)
Es una estructura de control especializada que se utiliza principalmente cuando el programador conoce con absoluta exactitud el número determinado y fijo de veces que se debe realizar la iteración antes de iniciar el ciclo. Esta herramienta utiliza una variable contadora interna que se inicializa explícitamente en un rango, se incrementa (o decrementa) automáticamente según el paso configurado y detiene de inmediato su ejecución al alcanzar el valor límite final fijado.

<div align="center">

#### 📝 Estructura en Pseudocódigo

<img width="544" height="106" alt="image" src="https://github.com/user-attachments/assets/e7150598-e5c0-4ea3-8052-a952f2a35aca" />

#### 📊 Diagrama de flujo

<img width="511" height="212" alt="image" src="https://github.com/user-attachments/assets/fba2380e-58bb-45e2-9026-7cd5cba4f2f0" />

</div>

<div align="center">
  
---

<div align="center">

## 🧠 EJERCICIO APLICATIVO NRO. 2: CONTROL DE NOTAS 🧠

</div>

## 📑 PLANTEAMIENTO DEL PROBLEMA 
Se requiere un programa en lenguaje C que solicite al usuario la nota final de un estudiante (un valor entre 0.0 y 10.0). El programa debe cumplir con dos condiciones:
1. Si el usuario ingresa una nota menor a 0 o mayor a 10, el sistema debe mostrar un mensaje de error y exigir que se vuelva a ingresar la nota de forma repetida hasta que sea válida.
2. Una vez que la nota sea correcta, el programa debe evaluar si el estudiante aprobó o reprobó. Se aprueba con una nota mayor o igual a 7.0.

---

### 🔍 ANÁLISIS DEL PROBLEMA 

| Datos de Entrada | Proceso | Condición | Datos de Salida |
|------------------|----------|------------|------------------|
| `nota`: Variable de tipo flotante (`float`) que almacena la calificación del alumno. | Usar un bucle de post-prueba `do-while` para obligar al usuario a ingresar una nota válida en el rango de 0 a 10. | `if (nota >= 7.0)` → **Aprobado**<br><br>`else` → **Reprobado** | Mensaje en pantalla indicando si el alumno está **"APROBADO"** o **"REPROBADO"**. |

---

### 📊 DIAGRAMA DE FLUJO OBTENIDO ✅

<img width="293" height="500" alt="image" src="https://github.com/user-attachments/assets/31c9094d-2056-4d73-87b3-9b63639460b5" />

---

### ⚪ CODIFICACIÓN EN LENGUAJE DE PROGRAMACIÓN C ⚪
El código es directo y utiliza pocas líneas, manteniendo la estructura limpia y fácil de leer:

```

#include <stdio.h>

int main() {
    float nota;

    printf("=== SISTEMA DE NOTAS ACADEMICAS ===\n\n");

    // 1. BUCLE DE VALIDACIÓN (DO-WHILE)
    do {
        printf("Ingrese la nota final del estudiante (0 - 10): ");
        scanf("%f", &nota);

        // Mensaje de error si la nota no cumple el rango solicitado
        if (nota < 0.0f || nota > 10.0f) {
            printf("[ERROR]: Nota invalida. Debe ser entre 0 y 10.\n\n");
        }
    } while (nota < 0.0f || nota > 10.0f);

    // 2. ESTRUCTURA CONDICIONAL (IF-ELSE)
    printf("\n-------------------------------------------------\n");
    if (nota >= 7.0f) {
        printf("ESTADO: ¡ESTUDIANTE APROBADO!\n");
    } else {
        printf("ESTADO: ESTUDIANTE REPROBADO\n");
    }
    printf("-------------------------------------------------\n");

    return 0;
}

```


### 🟦 VERIFICACION EN LA TERMINAL DE VISUAL STUDIO CODE 🟦
Ya escrito el codigo fuente, copilamos con el comando *"gcc diezsuma.c -o diezsuma"*,  y posterior lo ejecutamos en la terminal con el comando *".\diezsuma.exe"*.

## CASO 1

<img width="725" height="180" alt="image" src="https://github.com/user-attachments/assets/b88bd10b-7cc5-42b3-920b-559e32bcb8dc" />

## CASO 2

<img width="733" height="191" alt="image" src="https://github.com/user-attachments/assets/706e6b6a-fbde-4536-82d1-59b13d67f4e0" />

### ☑️PRUEBA DE ESCRITORIO☑️
Con el fin de ver la veracidad de los datos obtenidos por nuestro algoritmo en el programa, se procede a generar una prueba de escritorio.

## CASO 1

| Intento | Valor ingresado (nota) | Condición del Bucle (nota < 0 \|\| nota > 10) | Condición de Aprobación (nota >= 7.0) | Resultado en Pantalla |
|----------|-------------------------|-----------------------------------------------|---------------------------------------|------------------------|
| 1 | -2 | **Verdadera** (Inválida, el bucle repite) | - | Mensaje de ERROR |
| 2 | 10 | **Falsa** (Válida, sale del bucle) | **Verdadera** | **ESTUDIANTE APROBADO** |

## CASO 2

| Intento | Valor ingresado (nota) | Condición del Bucle (nota < 0 \|\| nota > 10) | Condición de Aprobación (nota >= 7.0) | Resultado en Pantalla |
|----------|-------------------------|-----------------------------------------------|---------------------------------------|------------------------|
| 1 | -8 | **Verdadera** (Inválida, el bucle repite) | - | Mensaje de ERROR |
| 2 | 5 | **Falsa** (Válida, sale del bucle) | **Falsa** | **ESTUDIANTE REPROBADO** |

### FINALMENTE
Se pudo dar resolución a la problemática del usuario por medio de la generación de este algorito y de igual manera se comprueba la vericidad de los datos generados por el algoritmo.

## DIFICULTADES

La principal dificultad que se tuvo durante el desarrollo del siguiente ejercicio es el uso correcto de los operadores lógicos: Al construir la condición del bucle while, la principal confusión inicial suele ser usar el operador && (Y) en lugar de || (O). Si escribimos while(nota < 0 && nota > 10), el bucle nunca se repetiría porque una nota no puede ser menor que cero y mayor que diez al mismo tiempo. Se requiere obligatoriamente el operador || para detectar que cualquiera de los dos errores rompa el rango de evaluación de entrada.


---

## 🟡REFLEXIÓN CRÍTICA 🟡

Este ejercicio nos permite demostrar que no se necesita un código gigante y complejo para blindar un programa contra datos erróneos. La combinación correcta de bucles y condicionales como el do-while y el if-else soluciona de forma óptima esta problematica, puesto que el programa no avanza ni toma decisiones de aprobación hasta que su dato de entrada sea un valor real y lógico. Esta estructura fundamenta las bases de la escritura de código seguro en ingeniería informática.


