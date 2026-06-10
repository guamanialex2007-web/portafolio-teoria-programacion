# 📗 Unidad 2: Estructuras Condicionales y Repetitivas

🔗 [« Volver al Inicio del Portafolio](../README.md)

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
| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | 🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama.md) |
| **Código Estructural (C)** | <pre>if (condicion) {<br>    // Instrucciones si es verdadero<br>} else {<br>    // Instrucciones si es falso<br>}</pre> |

#### B. Condicional Múltiple (Switch)
| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | 🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama_switch.md) |
| **Código Estructural (C)** | <pre>switch (variable) {<br>    case 1:<br>        Instrucciones_1;<br>        break;<br>    default:<br>        Instrucciones_Alternativas;<br>}</pre> |
---

## 🔁 2. Estructuras Repetitivas (Bucles)

Estructuras diseñadas para iterar o ejecutar un bloque de instrucciones múltiples veces mientras una condición lógica se mantenga activa o un rango numérico se cumpla.

### Tipos de Estructuras Repetitivas en C:
* **Bucle Mientras (`while`):** Evalúa la condición al inicio del ciclo (Pre-test). Si la condición es falsa desde el primer intento, el bloque interno nunca se ejecuta.
* **Bucle Hacer-Mientras (`do - while`):** Ejecuta el bloque de instrucciones al menos una vez antes de verificar la condición lógica al final (Post-test).
* **Bucle Para (`for`):** Agrupa en una sola línea la inicialización, la condición de parada y el incremento/decremento de una variable de control. Es ideal cuando se conoce de antemano el número exacto de iteraciones.

### 📐 Representación Estructural y Sintaxis

#### A. Estructura `while`
| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | 🔍 [Clic aquí para ver el Diagrama en Pantalla Completa](./ver_diagrama_while.md) |
| **Código Estructural (C)** | <pre>while (condicion) {<br>    // Instrucciones a repetir<br>}</pre> |

#### B. Estructura `do - while`
| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | *(Sube la captura de tu bucle como `bucle_repetir.png`)* |
| **Código Estructural (C)** | <pre>do {<br>    // Instrucciones a repetir<br>} while (condicion);</pre> |

#### C. Estructura `for`
| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | *(Sube la captura de tu bucle como `bucle_para.png`)* |
| **Código Estructural (C)** | <pre>for (int i = valor_inicial; i <= valor_final; i++) {<br>    // Instrucciones a repetir<br>}</pre> |

---

## 💻 3. Ejercicio Integrador Práctico
<img width="785" height="745" alt="image" src="https://github.com/user-attachments/assets/1c5bd0d1-9872-4ceb-9c4b-7c1b4e2a5a71" />

### 📝 A. Planteamiento del Problema
Desarrollar un programa en **lenguaje C** que permita procesar las calificaciones finales de un grupo de $N$ estudiantes en la asignatura de Teoría de la Programación. El programa debe solicitar la cantidad total de alumnos, pedir secuencialmente la nota de cada uno, validar mediante una estructura condicional si el estudiante está "Aprobado" (nota mayor o igual a 7.0) o "Reprobado", y al finalizar desplegar el promedio general del aula junto al total de alumnos aprobados.

### 🔍 B. Análisis del Problema
* **Datos de Entrada:**
  * Variable de tipo entero (`int`): `n` (Cantidad total de estudiantes a evaluar).
  * Variable de tipo flotante (`float`): `nota` (Calificación ingresada cíclicamente en cada iteración).
* **Proceso Requerido:**
  * Inicializar el acumulador de notas de tipo flotante `suma_notas = 0.0` y el contador de aprobados `aprobados = 0`.
  * Implementar un bucle repetitivo `for` controlado por una variable contador `i` desde $1$ hasta `n`.
