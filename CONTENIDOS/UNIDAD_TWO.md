# Estructuras de Control de Flujo: Condicionales y Repetitivas

Las estructuras de control son los pilares fundamentales de la lógica de programación. Permiten modificar el flujo lineal de un programa, tomando decisiones o repitiendo bloques de código según se cumplan o no determinadas condiciones.

---

## 1. Estructuras Condicionales

Permiten bifurcar el flujo de ejecución de un programa basándose en el resultado de una expresión lógica (verdadera o falsa).

### A. Condicional Simple (Si-Entonces / If)
Es una estructura de control que evalúa una expresión lógica (una condición que solo puede ser verdadera o falsa). Si el resultado de la evaluación es verdadero, el flujo del programa se desvía temporalmente para ejecutar un bloque específico de instrucciones; si es falso, el programa ignora por completo dicho bloque y continúa con la ejecución de la siguiente línea de código inmediata.

#### Estructura en Pseudocódigo

<img width="228" height="107" alt="image" src="https://github.com/user-attachments/assets/ce452a5e-c3c0-4998-9176-b461ea6a9bb8" />

#### Diagrama de flujo
<img width="403" height="235" alt="image" src="https://github.com/user-attachments/assets/6634d573-2128-4528-8340-ba6885e285d1" />


### B. Condicional Doble: (Si-Entonces-Sino / If-Else)
A diferencia e la estructura simple, esta permite al programa elegir entre dos caminos o alternativas mutuamente excluyentes basados en el resultado de una condición. Si la expresión lógica es verdadera, se ejecuta obligatoriamente el primer bloque de instrucciones (rama del Entonces); si es falsa, se ejecuta un segundo bloque alternativo de instrucciones (rama del Sino).

#### Estructura en Pseudocódigo

<img width="203" height="136" alt="image" src="https://github.com/user-attachments/assets/2da1fb82-8240-4b70-b1c4-c107cbd1615c" />


#### Diagrama de flujo
<img width="346" height="212" alt="image" src="https://github.com/user-attachments/assets/1279a3e0-1aa5-419a-927c-6c17236c7426" />

### C. Condicional Múltiple: (Según Sea / Switch)
Es una estructura de control de selección que evalúa el valor exacto de una variable o expresión frente a un conjunto de constantes o casos predefinidos. En lugar de evaluar expresiones booleanas complejas (como respuestas de verdadero/falso), compara de forma directa si el contenido de la variable coincide con alguna de las opciones disponibles para ejecutar el bloque de código asignado a ese caso específico. Por lo general, incluye una opción por defecto (De Otro Modo / Default) que se ejecuta únicamente si el valor de la variable no coincide con ninguno de los casos listados.

#### Estructura en Pseudocódigo
<img width="243" height="206" alt="image" src="https://github.com/user-attachments/assets/093bf31c-5a89-4380-ad46-7e54b7ede118" />

#### Diagrama de flujo
<img width="447" height="290" alt="image" src="https://github.com/user-attachments/assets/aa3f8305-0d70-4098-9fa0-84e7973e5520" />

# Estructuras de Control de Flujo: Condicionales y Repetitivas

Las **estructuras de control de flujo** son los pilares fundamentales de la lógica de programación. Su función principal es **romper la ejecución lineal y secuencial** por defecto de un ordenador (que procesa el código línea por línea, de arriba hacia abajo). Al evaluar condiciones lógicas o matemáticas, estas herramientas otorgan al desarrollador la capacidad de reaccionar ante datos cambiantes mediante dos acciones clave: **bifurcar el camino** del programa (tomar decisiones) o **ciclar bloques de instrucciones** (repetir tareas monótonas) de forma totalmente automatizada.

---

### A. Bucle Mientras (Mientras-Hacer / While)
Es una estructura clasificada como de "pre-prueba" o evaluación previa, debido a que tiene la particularidad de validar la expresión lógica obligatoriamente antes de permitir el ingreso al bloque de código interno. Si la condición matemática o lógica resulta ser falsa desde la primera comprobación, el cuerpo del bucle se descarta y nunca se ejecuta; por el contrario, si es verdadera, el ciclo se repetirá indefinidamente hasta que la condición deje de cumplirse por completo.

#### Estructura en Pseudocódigo

<img width="400" height="250" alt="Bucle Mientras" src="" />


### B. Bucle Repetir (Repetir-Hasta Que / Do-Until)
A diferencia radical del bucle analizado anteriormente, esta se consolida como una estructura de "post-prueba" o evaluación posterior. El compilador primero ejecuta el bloque de instrucciones designado y luego realiza la evaluación de la condición al final del camino; esto garantiza de forma estricta que el código interno se ejecute al menos una vez antes de que el programa verifique si se debe continuar con la siguiente iteración.

#### Estructura en Pseudocódigo

<img width="400" height="250" alt="Bucle Repetir" src="" />


### C. Bucle Para (Para-Hasta-Hacer / For)
Es una estructura de control especializada que se utiliza principalmente cuando el programador conoce con absoluta exactitud el número determinado y fijo de veces que se debe realizar la iteración antes de iniciar el ciclo. Esta herramienta utiliza una variable contadora interna que se inicializa explícitamente en un rango, se incrementa (o decrementa) automáticamente según el paso configurado y detiene de inmediato su ejecución al alcanzar el valor límite final fijado.

#### Estructura en Pseudocódigo

<img width="400" height="250" alt="Bucle Para" src="" />


