
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
  
## 🧠EJERCICIO APLICATIVO DE LOS CONOCIMIENTOS🧠

</div>

## PLANTEAMIENTO DEL PROBLEMA 




### ANALISIS DEL PROBLEMA 

•	Creacion de un programa  que debe permitir ingresar la cantidad total de estudiantes, y mediante un bucle, repetir el proceso de lectura de calificaciones y cálculo de la nota final, para cada uno de los estudiantes del curso.  
•	En cada repetición, el programa solicitará los valores de los componentes (ACD, APE, AA y ES), calculará la nota final, mostrará el resultado final y una referencia de su calificación antes de pasar al siguiente estudiante. 
•	Además, el programa debe permitir validar que las notas ingresadas estén dentro del rango permitido (0 a 10). Si el profesor ingresa una nota fuera de este rango, el programa mostrará un mensaje de error y le solicitara que ingrese el dato nuevamente hasta que sea correcto para las operaciones del algoritmo.


<div align="center">
  


</div>

### DIAGRAMA DE FLUJO OBTENIDO ✅

Para acceder al diagrama de flujo, por favor ingrese al siguiente enlace, cuando ingrese a drive, notara que la imagen esta borrosa, para observarla con la mejor calidad, de clik en la parte superior derecha Abrir con draw.io.

https://drive.google.com/file/d/1_Y7AWNTsnmndNXMcjblL8B_nMINaqZJM/view?usp=sharing

  
### ⚪ CODIFICACION EN LENGUAJE DE PROGRAMACION C ⚪
Una vez realizado el diagrama y haberlo probado, podemos proceder a escribir el algoritmo en lenguaje de programación C, tomando como referencia el diagrama con el fin de evitar errores. 

#include <stdio.h>
int main(){

    //DEFINIMOS LAS VARIABLES PARA EL PROBLEMA
    int est, cont;
    float notaACD, notaAA, notaAPE, notaES;
    float pACD, pAA, pAPE, pES, nF;

    //SOLICITAMOS EL # DE ESTUDIANTES AL USUARIO 
    do{
        printf("INGRESE EL NUMERO DE ESTUDIANTES DE SU CURSO: ");
        scanf("%i",&est);
            if(est<=0){
            printf("VALOR INVALIDO, INGRESE NUEVAMENTE.\n");
            }
    }while(est<=0);

    //INICIAMOS EL BUCLE PARA LAS NOTAS DE LOS ESTUDIANTES
    for(cont=1;cont<=est;cont++){
        printf("\n");
        printf("INGRESE LAS NOTAS DEL ESTUDIANTE NRO.%i\n",cont);\
        printf("\n");

        do{
        printf("Nota de ACD sobre 10: ");
        scanf("%f",&notaACD);
            if(notaACD<0 || notaACD>10){
                printf("NOTA INVALIDA, INGRESE NUEVAMENTE.\n");
            }
        }while(notaACD<0 || notaACD>10);

        do{
        printf("Nota de AA sobre 10: ");
        scanf("%f",&notaAA);
            if(notaAA<0 || notaAA>10){
                printf("NOTA INVALIDA, INGRESE NUEVAMENTE.\n");
            }
        }while(notaAA<0 || notaAA>10);

        do{
        printf("Nota de APE sobre 10: ");
        scanf("%f",&notaAPE);
            if(notaAPE<0 || notaAPE>10){
                printf("NOTA INVALIDA, INGRESE NUEVAMENTE.\n");
            }
        }while(notaAPE<0 || notaAPE>10);

        do{
        printf("Nota de ES sobre 10: ");
        scanf("%f",&notaES);
            if(notaES<0 || notaES>10){
                printf("NOTA INVALIDA, INGRESE NUEVAMENTE.\n");
            }
        }while(notaES<0 || notaES>10);
        
        //CON LOS DATOS PROCEDEMOS A REALIZAR EL CALCULO 
        pACD = notaACD*0.2f;
        pAA = notaAA*0.2f;
        pAPE = notaAPE*0.25f;
        pES = notaES*0.35f;
        nF = pACD + pAA + pAPE + pES;

        //IMPRIMIMOS LOS PONDERADOS Y NOTA FINAL DEL ESTUDIANTE
        printf("\n");
        printf("-------------------------------------------------\n");
        printf("\n");
        printf("El ponderado de la nota ACD es: %.2f\n",pACD);
        printf("El ponderado de la nota AA es: %.2f\n",pAA);
        printf("El ponderado de la nota APE es: %.2f\n",pAPE);
        printf("El ponderado de la nota ES es: %.2f\n",pES);
        printf("\n");
        printf("POR LO TANTO LA NOTA FINAL ES: %.2f\n", nF);

        //APLICAMOS UN CONDICIONAL PARA INDICAR SI LA NOTA ES BUENA O MALA
        if(nF >=9 ){
            printf("EXCELENTE PROMEDIO\n");
        }else if (nF >=7 && nF<9){
            printf("BUEN PROMEDIO\n");
        }else if(nF >=5 && nF<7){
            printf("PROMEDIO REGULAR\n");
        }else{
            printf("PROMEDIO DEFICIENTE\n");
        }
        printf("\n");
        printf("-------------------------------------------------\n");
    }
    return 0;
}
### 🟦 VERIFICACION EN LA TERMINAL DE VISUAL STUDIO CODE 🟦
Ya escrito el codigo fuente, copilamos con el comando *"gcc concesonariocarro.c -o consesonariocarro"*,  y posterior lo ejecutamos en la terminal con el comando *".\concesonariocarro.exe"*.



### ☑️PRUEBA DE ESCRITORIO☑️
Con el fin de ver la veracidad de los datos obtenidos por nuestro algoritmo en el programa, se procede a generar una prueba de escritorio.

| Datos de Entrada | Proceso | Datos de Salida |
| :--- | :--- | :--- |
| Precio Carro 1 = 20000 | 20000*0.4 | 800 |
| Precio Carro 2 = 15500 | 15500*0.4 | 620 |
| Precio Carro 3 = 32000 | 32000*0.4 | 1280 |

### FINALMENTE
Se pudo dar resolución a la problemática del usuario por medio de la generación de este algorito y de igual manera se comprueba la vericidad de los datos generados por el algoritmo.



---

## 🟡REFLEXIÓN CRÍTICA 🟡




