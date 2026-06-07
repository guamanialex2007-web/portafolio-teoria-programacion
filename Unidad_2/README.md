# 📗 Unidad 2: Estructuras Condicionales y Repetitivas
🔗 [« Volver al Inicio del Portafolio](../README.md)
## 🎯 Objetivo de la Unidad
Registrar, organizar y consolidar las actividades de aprendizaje de la Unidad 2, integrando evidencias técnicas y reflexiones críticas sobre la lógica de control de flujo en la resolución de problemas lógicos y computacionales.

---

## 🧩 1. Estructuras Condicionales

Permiten bifurcar el flujo de ejecución de un programa basándose en el cumplimiento de una condición lógica (verdadera o falsa).

### Tipos de Estructuras Condicionales:
* **Condicional Simple (`if`):** Evalúa una condición; si es verdadera, ejecuta un bloque de código.
* **Condicional Compuesta (`if-else`):** Ofrece un camino alternativo si la condición evalúa como falsa.
* **Condicional Anidada / Múltiple (`switch` o `if-elif-else`):** Permite evaluar múltiples condiciones en cascada o seleccionar entre varias alternativas posibles.

### 📐 Representación Estructural
> 💡 *Nota para el estudiante: Reemplaza las rutas de las imágenes de abajo `(diagrama_condicional.png)` con tus capturas reales de los diagramas que hagas en herramientas como PSeInt o Draw.io.*

| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | ![Diagrama Condicional](./imagenes/diagrama_condicional.png) |
| **Pseudocódigo Genérico** | <pre>Si (condicion) Entonces<br>    Instrucciones_Si_Verdadero<br>Sino<br>    Instrucciones_Si_Falso<br>FinSi</pre> |

---

## 🔁 2. Estructuras Repetitivas (Bucles)

Estructuras diseñadas para ejecutar un bloque de instrucciones múltiples veces mientras una condición lógica se mantenga activa o un rango se cumpla.

### Tipos de Estructuras Repetitivas:
* **Bucle Mientras (`While`):** Evalúa la condición al inicio. Si es falsa desde el principio, el bloque jamás se ejecuta.
* **Bucle Repetir / Hacer-Mientras (`Do-While` / `Repeat`):** Ejecuta el bloque de código al menos una vez antes de verificar la condición.
* **Bucle Para (`For`):** Ideal cuando se conoce de antemano el número exacto de iteraciones a realizar.

### 📐 Representación Estructural

| Enfoque | Representación |
| :--- | :--- |
| **Diagrama de Flujo** | ![Diagrama Repetitivo](./imagenes/diagrama_repetitivo.png) |
| **Pseudocódigo Genérico** | <pre>Mientras (condicion) Hacer<br>    Instrucciones_A_Repetir<br>FinMientras</pre> |

---

## 💻 3. Ejercicio Integrador Práctico
*(Aplicación de Estructuras Condicionales y Repetitivas)*

### 📝 A. Planteamiento del Problema
*Escribe aquí el enunciado del problema que te dio el profesor. (Ejemplo: "Desarrollar un algoritmo que lea N calificaciones de alumnos, calcule el promedio y determine cuántos aprobaron y reprobaron").*

### 🔍 B. Análisis del Problema
* **Entradas:** [Lista de variables de entrada, ej: Cantidad de alumnos (N), Calificaciones].
* **Proceso:** [Explicación de la lógica, ej: Sumar calificaciones en un bucle `Para` y evaluar cada una con un `Si-Entonces`].
* **Salidas:** [Resultados esperados, ej: Promedio final, contador de aprobados].

### 🎨 C. Diseño del Algoritmo (Diagrama de Flujo)
![Diagrama del Ejercicio Integrador](./imagenes/diagrama_ejercicio.png)

### ⚙️ D. Codificación (Código Fuente)
```python
# Modifica el lenguaje según el que estén usando en clase (ej: python, c++, java, pascal)
# Ejemplo de estructura integradora en Python:

n = int(input("Ingrese la cantidad de estudiantes: "))
aprobados = 0

for i in range(1, n + 1):
    nota = float(input(f"Ingrese la nota del estudiante {i}: "))
    if nota >= 7.0:
        aprobados += 1

print(f"El total de estudiantes aprobados es: {aprobados}")


