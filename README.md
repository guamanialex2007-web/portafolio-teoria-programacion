# 📘 PORTAFOLIO DIGITAL DE APRENDIZAJE
## ⚡ Teoría de la Programación — Unidad 1

---

## 🏫 Información General

| 🏢 DIMENSIÓN INSTITUCIONAL | 🏛️ DETALLES ACADÉMICOS |
| :--- | :--- |
| **🏫 Universidad** | Universidad Nacional de Loja |
| **🏛️ Facultad** | Facultad de la Energía, las Industrias y los Recursos Naturales No Renovables |
| **🎓 Carrera** | Computación |
| **📚 Asignatura** | Teoría de la Programación |
| **📆 Ciclo** | Primer Ciclo |
| **🗓️ Período Académico** | Abril – Agosto 2026 |
| **👨‍🏫 Docente** | [Nombre del Docente] |
| **👨‍🎓 Estudiante** | Alexander Ventura Guaman Puli |

---

## 📂 UNIDAD 1: CONTENIDOS TEÓRICOS

> [!NOTE]
> ### 🔍 1. Algoritmo
> Un algoritmo es una secuencia finita, ordenada y bien definida de pasos lógicos que permiten resolver problemas.
>
> * **✔ Preciso:** Indica el orden estricto de cada paso.
> * **✔ Finito:** Tiene un número limitado de pasos.
> * **✔ Determinista:** Mismos datos de entrada producen siempre el mismo resultado.

> [!TIP]
> ### 🔄 2. Diagrama de Flujo y Pseudocódigo
> Fundamentos y herramientas clave para el diseño estructural antes de la codificación.
>
> * 🔷 **Diagrama de flujo:** Representación gráfica y visual de un algoritmo usando símbolos estandarizados y flechas de dirección.
> * 📝 **Pseudocódigo:** Descripción narrativa y estructurada en lenguaje natural de un algoritmo, libre de reglas rígidas de sintaxis.

> [!IMPORTANT]
> ### 🧪 3. Prueba de Escritorio
> Técnica de validación manual que simula la ejecución paso a paso de un algoritmo dentro de una tabla de seguimiento. Su fin primordial es detectar errores lógicos antes de transcribir al código.

> [!WARNING]
> ### 💻 4. Lenguajes de Programación
> Sistema formal de símbolos y reglas que permite dictar instrucciones detalladas a un computador.
>
> * 🧷 **Bajo nivel:** Lenguajes íntimamente cercanos al hardware y registros de la máquina (ej. Ensamblador).
> * 🚀 **Alto nivel:** Lenguajes abstractos y legibles, muy cercanos al idioma humano (ej. Python, Java, C++).

> [!CAUTION]
> ### 🧩 5. Programación por Bloques
> Metodología educativa y visual basada en arrastrar y soltar piezas interconectables estilo rompecabezas. Permite asimilar la lógica algorítmica aislando por completo al alumno de la complejidad gramatical.

---

## 💻 EJERCICIO PRÁCTICO SECUENCIAL

> [!NOTE]
> ### 📌 Planteamiento del problema
> * **Enunciado:** Diseñar un programa estructurado que calcule el área y el perímetro de un rectángulo a partir de los datos introducidos por el usuario.

### 📊 Análisis del problema

* **📥 Entrada:** Base ($b$), Altura ($h$) `[Tipo: Real]`
* **⚙️ Proceso:**
  * $Área = base \times altura$
  * $Perímetro = 2 \times (base + altura)$
* **📤 Salida:** Área calculada, Perímetro calculado

### 🧾 Pseudocódigo (PSeInt)

```text
Algoritmo CalcularRectangulo
    Definir base, altura, area, perimetro Como Real

    Escribir "Ingrese la base del rectángulo:"
    Leer base

    Escribir "Ingrese la altura del rectángulo:"
    Leer altura

    area <- base * altura
    perimetro <- 2 * (base + altura)

    Escribir "El área es: ", area
    Escribir "El perímetro es: ", perimetro
FinAlgoritmo
