# Estructuras de Control de Flujo: Condicionales y Repetitivas

Las estructuras de control son los pilares fundamentales de la lógica de programación. Permiten modificar el flujo lineal de un programa, tomando decisiones o repitiendo bloques de código según se cumplan o no determinadas condiciones.

---

## 1. Estructuras Condicionales

Permiten bifurcar el flujo de ejecución de un programa basándose en el resultado de una expresión lógica (verdadera o falsa).

### A. Condicional Simple (Si-Entonces / If)
Es una estructura de control que evalúa una expresión lógica (una condición que solo puede ser verdadera o falsa). Si el resultado de la evaluación es verdadero, el flujo del programa se desvía temporalmente para ejecutar un bloque específico de instrucciones; si es falso, el programa ignora por completo dicho bloque y continúa con la ejecución de la siguiente línea de código inmediata.

#### Estructura en Pseudocódigo

<img width="403" height="235" alt="image" src="https://github.com/user-attachments/assets/6634d573-2128-4528-8340-ba6885e285d1" />


### B. Condicional Doble: (Si-Entonces-Sino / If-Else)
A diferencia e la estructura simple, esta permite al programa elegir entre dos caminos o alternativas mutuamente excluyentes basados en el resultado de una condición. Si la expresión lógica es verdadera, se ejecuta obligatoriamente el primer bloque de instrucciones (rama del Entonces); si es falsa, se ejecuta un segundo bloque alternativo de instrucciones (rama del Sino).

#### Estructura en Pseudocódigo
<img width="346" height="212" alt="image" src="https://github.com/user-attachments/assets/1279a3e0-1aa5-419a-927c-6c17236c7426" />

### C. Condicional Múltiple: (Según Sea / Switch)
Es una estructura de control de selección que evalúa el valor exacto de una variable o expresión frente a un conjunto de constantes o casos predefinidos. En lugar de evaluar expresiones booleanas complejas (como respuestas de verdadero/falso), compara de forma directa si el contenido de la variable coincide con alguna de las opciones disponibles para ejecutar el bloque de código asignado a ese caso específico. Por lo general, incluye una opción por defecto (De Otro Modo / Default) que se ejecuta únicamente si el valor de la variable no coincide con ninguno de los casos listados.

#### Estructura en Pseudocódigo

<img width="447" height="290" alt="image" src="https://github.com/user-attachments/assets/aa3f8305-0d70-4098-9fa0-84e7973e5520" />


