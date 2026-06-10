# 📗 Unidad 2: Estructuras Condicionales y Repetitivas

🔗 [« Volver al Inicio del Portafolio](../README.md) | 📚 [Ver Referencias de la Unidad](./referencias.md)

---

## 🎯 Objetivo de la Unidad
Registrar, organizar y consolidar las actividades de aprendizaje de la Unidad 2, integrando evidencias técnicas y reflexiones críticas sobre la lógica de control de flujo en la resolución de problemas lógicos y computacionales.

---

## 🧩 1. Estructuras Condicionales

Permiten bifurcar el flujo de ejecución de un programa basándose en el cumplimiento de una condición lógica (verdadera o falsa).

### Tipos de Estructuras Condicionales en C:
* **Condicional Simple (`if`):** Evalúa una condición; si es verdadera, ejecuta el bloque de código entre llaves `{}`.
* **Condicional Compuesta (`if - else`):** Evalúa una condición y ofrece una ruta alternativa de ejecución bajo la cláusula `else` si el resultado es falso.
* **Condicional Anidada / Múltiple (`switch`):** Evalúa una expresión de tipo entera o carácter frente a una lista de casos estáticos (`case`), redirigiendo el flujo al bloque correspondiente.

### 📐 Representación Estructural y Sintaxis

#### A. Condicional Simple y Compuesta
Enfoque y Representación 

**Diagrama de Flujo**  🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama.md)


 **Código Estructural (C)** 
 ```c
if (condicion) {
    // Instrucciones si es verdadero
} else {
    // Instrucciones si es falso
}
```
#### B. Condicional Múltiple (Switch)
Enfoque y Representación 

**Diagrama de Flujo** 🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama_switch.md) 


 **Código Estructural (C)** 
 
```c
switch (variable) {

    case 1:
        instrucciones_1;
        break;

    default:
        instrucciones_alternativas;
}
```

---

## 🔁 2. Estructuras Repetitivas (Bucles)

Estructuras diseñadas para iterar o ejecutar un bloque de instrucciones múltiples veces mientras una condición lógica se mantenga activa o un rango numérico se cumpla.

### Tipos de Estructuras Repetitivas en C:
* **Bucle Mientras (`while`):** Evalúa la condición al inicio del ciclo (Pre-test). Si la condición es falsa desde el primer intento, el bloque interno nunca se ejecuta.
* **Bucle Hacer-Mientras (`do - while`):** Ejecuta el bloque de instrucciones al menos una vez antes de verificar la condición lógica al final (Post-test).
* **Bucle Para (`for`):** Agrupa en una sola línea la inicialización, la condición de parada y el incremento/decremento de una variable de control. Es ideal cuando se conoce de antemano el número exacto de iteraciones.

### 📐 Representación Estructural y Sintaxis

#### A. Estructura `while`
 Enfoque y Representación 

 **Diagrama de Flujo**  🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama_while.md) 
 

 **Código Estructural (C)** 
 
```c
while (condicion) {
    // Instrucciones a repetir
}
```

#### B. Estructura `do - while`
 Enfoque y Representación 


 **Diagrama de Flujo**  🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama_do_while.md) 
 
 
 **Código Estructural (C)** 
 
```c
do {
    // Instrucciones a repetir
} while (condicion);
```

#### C. Estructura `for`
 Enfoque y Representación 


 **Diagrama de Flujo**  🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama_for.md) 

 
 **Código Estructural (C)** 
 
```c
for (int i = valor_inicial; i <= valor_final; i++) {
    // Instrucciones a repetir
}
```

---

## 💻 3. Ejercicio Integrador Práctico

### 📝 A. Planteamiento del Problema
Desarrollar un programa en **lenguaje C** que permita procesar las calificaciones finales de un grupo de $N$ estudiantes en la asignatura de Teoría de la Programación. El programa debe solicitar la cantidad total de alumnos, pedir secuencialmente la nota de cada uno, validar mediante una estructura condicional si el estudiante está "Aprobado" (nota mayor o igual a 7.0) o "Reprobado", y al finalizar desplegar el promedio general del aula junto al total de alumnos aprobados.

### 🔍 B. Análisis del Problema
* **Datos de Entrada:**
  * Variable de tipo entero (`int`): `n` (Número de estudiantes).
  * Variable de tipo entero (`int`): `i` (Contador interno del bucle).
  * Variable de tipo flotante (`float`): `nota` (Calificación ingresada cíclicamente).
* **Proceso Requerido:**
  * Inicializar el acumulador `suma = 0.0` y el contador de aprobados `aprobados = 0`.
  * Implementar un bucle repetitivo `for` controlado por `i` desde 1 hasta `n`.
  * **Ecuación del Promedio (Calculada dinámicamente en la salida):**
    $$Promedio = \frac{suma}{n}$$
## 💻 3. Codigo fuente 
<img width="785" height="745" alt="image" src="https://github.com/user-attachments/assets/1c5bd0d1-9872-4ceb-9c4b-7c1b4e2a5a71" />

### 📊 C. Evidencia de la Prueba de Escritorio
<img width="655" height="669" alt="image" src="https://github.com/user-attachments/assets/9386aa20-92bd-4683-9c97-14be2944a014" />

### 📐 D. Diseño del Algoritmo (Diagrama de Flujo)



<img width="460" height="829" alt="image" src="https://github.com/user-attachments/assets/8cd75579-bf46-4b02-b198-022b4449e090" />
