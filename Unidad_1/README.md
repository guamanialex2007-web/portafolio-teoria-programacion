# 📘 Unidad 1: Algoritmos y Estructuras Secuenciales

🔗 [« Volver al Inicio del Portafolio](../README.md)

---

## 🎯 Objetivo de la Unidad
Registrar y organizar de manera sistemática las actividades de aprendizaje de la Unidad 1, consolidando los conocimientos sobre el ciclo de vida de un algoritmo y la implementación de soluciones mediante estructuras secuenciales.

---

## 📚 1. Desarrollo del Contenido Temático

### 📌 Conceptos Fundamentales
* **Algoritmo:** Secuencia ordenada, finita y precisa de pasos lógicos encaminados a resolver un problema determinado. Un algoritmo debe ser definido (producir siempre el mismo resultado ante las mismas entradas) y finito.
* **Pseudocódigo:** Lenguaje de especificación de algoritmos de alto nivel que utiliza una mezcla de lenguaje natural con convenciones sintácticas propias de los lenguajes de programación. Facilita la transición del pensamiento lógico al código real.
* **Diagrama de Flujo:** Representación gráfica de un algoritmo mediante un conjunto de símbolos estandarizados (óvalos, rectángulos, rombos) interconectados por flechas que indican la dirección del flujo de datos.
* **Prueba de Escritorio:** Técnica de validación manual que consiste en simular la ejecución paso a paso de un algoritmo utilizando datos de prueba concretos para verificar si el resultado lógico es el esperado y detectar errores tempranos.
* **Lenguajes de Programación:** Sistemas de comunicación estructurados con reglas sintácticas y semánticas precisas que permiten a un programador escribir instrucciones ejecutables por una computadora.

### 🧱 Programación por Bloques
Es un enfoque visual de aprendizaje de la computación que permite diseñar lógica de programación arrastrando y soltando piezas o "bloques" gráficos en un lienzo interactivo (como en Scratch o App Inventor). Elimina las barreras de la sintaxis estricta y los errores de punto y coma, permitiendo al estudiante enfocarse exclusivamente en el desarrollo de la lógica algorítmica fundamental.
<img width="783" height="517" alt="image" src="https://github.com/user-attachments/assets/d723ac31-8234-4b76-8b0c-c8293e8d88dc" />

---

## 💻 2. Ejercicio Práctico con Estructura Secuencial
*(Evidencia de Aplicación Práctica)*
<img width="1053" height="726" alt="image" src="https://github.com/user-attachments/assets/ca39ed19-e538-44c5-a395-f13d1e7561f2" />

### 📝 A. Planteamiento del Problema
Dado un triángulo, calcular su área conociendo la longitud de su base y su altura. El programa debe solicitar ambos valores al usuario, aplicar la fórmula matemática correspondiente y mostrar el resultado.

### 🔍 B. Análisis del Problema
* **Datos de Entrada:**
  * Variable numérica real: `base` (longitud horizontal del triángulo).
  * Variable numérica real: `altura` (distancia vertical desde la base al vértice opuesto).
* **Proceso Requerido:**
  * Aplicación lineal de la fórmula geométrica del área:
    $$area = \frac{base \times altura}{2}$$
* **Datos de Salida:**
  * Variable numérica real: `area` (superficie total calculada).

---

### 📐 C. Diseño del Algoritmo

#### 📊 Diagrama de Flujo (Exportado de PSeInt)
<img width="693" height="859" alt="Diagrama de Flujo del Algoritmo Secuencial" src="https://github.com/user-attachments/assets/aabf8c3b-83da-4d70-8efd-77bde453661c" />

#### 📝 Pseudocódigo (PSeInt / Estándar)
```text
Algoritmo EjercicioSecuencial
    // 1. Definición de variables
    Definir base, altura, area Como Real
    
    // 2. Entrada de datos
    Escribir "Ingrese la base del triángulo:"
    Leer base
    Escribir "Ingrese la altura del triángulo:"
    Leer altura
    
    // 3. Proceso secuencial
    area <- (base * altura) / 2
    
    // 4. Salida
    Escribir "El área calculada es: ", area
FinAlgoritmo
