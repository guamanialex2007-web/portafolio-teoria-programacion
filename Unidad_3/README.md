# 📘 Unidad 3 – Modularidad y Arreglos

⬅️ [Volver al Portafolio Principal](../README.md)

---

# 📖 Introducción

En esta unidad se abordaron dos temas fundamentales de la programación: la **modularidad** y los **arreglos**. La modularidad permite dividir un programa en funciones o procedimientos que realizan tareas específicas, facilitando el mantenimiento y reutilización del código. Por otro lado, los arreglos permiten almacenar múltiples datos del mismo tipo en una sola estructura, optimizando el manejo de información dentro de los programas.

---

# 🧩 1. Modularidad

## 📘 Sustento teórico

La modularidad es una técnica de programación que consiste en dividir un programa en pequeñas partes llamadas **módulos**, **funciones** o **procedimientos**.

Cada módulo tiene una responsabilidad específica y puede ser reutilizado desde diferentes partes del programa.

Entre sus principales ventajas se encuentran:

- Reutilización del código.
- Facilidad para detectar errores.
- Mayor organización del programa.
- Mejor mantenimiento del software.
- Desarrollo colaborativo.

Los parámetros permiten intercambiar información entre el programa principal y las funciones.

Existen dos formas principales:

- Paso por valor.
- Paso por referencia.

---

## 💻 Ejemplo 1: Paso de parámetros por valor

En el paso por valor la función recibe una **copia** de la variable original.

Los cambios realizados dentro de la función **no modifican** la variable original.

```c
#include <stdio.h>

void duplicar(int numero){

    numero = numero * 2;

    printf("Dentro de la funcion: %d\n", numero);

}

int main(){

    int numero = 10;

    printf("Antes de llamar la funcion: %d\n", numero);

    duplicar(numero);

    printf("Despues de llamar la funcion: %d\n", numero);

    return 0;
}
```

### Resultado

```
Antes de llamar la funcion: 10
Dentro de la funcion: 20
Despues de llamar la funcion: 10
```

---

## 💻 Ejemplo 2: Paso de parámetros por referencia

En el paso por referencia se envía la dirección de memoria de la variable.

Los cambios realizados dentro de la función modifican directamente la variable original.

```c
#include <stdio.h>

void duplicar(int *numero){

    *numero = (*numero) * 2;

}

int main(){

    int numero = 10;

    printf("Antes de llamar la funcion: %d\n", numero);

    duplicar(&numero);

    printf("Despues de llamar la funcion: %d\n", numero);

    return 0;
}
```

### Resultado

```
Antes de llamar la funcion: 10
Despues de llamar la funcion: 20
```

---

# 📂 2. Arreglos

## 📘 Sustento teórico

Los arreglos son estructuras de datos homogéneas que permiten almacenar varios elementos del mismo tipo bajo un único nombre.

Cada elemento ocupa una posición dentro del arreglo y puede accederse mediante un índice.

Los arreglos pueden ser:

- Unidimensionales (Vectores).
- Bidimensionales (Matrices).

---

## 🗂️ Arreglo unidimensional (Vector)

Los vectores almacenan datos en una sola dimensión.

```c
#include <stdio.h>

int main(){

    float notas[5]={8.5,9.0,7.2,10.0,6.8};

    printf("Listado de notas\n\n");

    for(int i=0;i<5;i++){

        printf("Estudiante %d: %.1f\n",i+1,notas[i]);

    }

    return 0;

}
```

### Resultado

```
Listado de notas

Estudiante 1: 8.5
Estudiante 2: 9.0
Estudiante 3: 7.2
Estudiante 4: 10.0
Estudiante 5: 6.8
```

---

## 🗂️ Arreglo bidimensional (Matriz)

Las matrices organizan la información mediante filas y columnas.

```c
#include <stdio.h>

int main(){

    float notas[3][2]={

        {8.0,9.5},
        {7.0,8.2},
        {9.0,10.0}

    };

    for(int fila=0;fila<3;fila++){

        printf("Estudiante %d -> ",fila+1);

        for(int columna=0;columna<2;columna++){

            printf("Materia %d: %.1f  ",columna+1,notas[fila][columna]);

        }

        printf("\n");

    }

    return 0;

}
```

### Resultado

```
Estudiante 1 -> Materia 1: 8.0  Materia 2: 9.5
Estudiante 2 -> Materia 1: 7.0  Materia 2: 8.2
Estudiante 3 -> Materia 1: 9.0  Materia 2: 10.0
```

---
---

## 🗂️ Arreglos tridimensionales

Los arreglos tridimensionales permiten almacenar datos organizados en **tres dimensiones**. Se utilizan cuando la información requiere tres índices para ser identificada, por ejemplo: **edificio → piso → habitación**, **año → mes → día** o **curso → estudiante → calificación**.

La sintaxis general en C es:

```c
tipo nombre[dim1][dim2][dim3];
```

Cada elemento se accede mediante tres índices:

```c
nombre[i][j][k]
```

### 💻 Ejemplo en C

```c
#include <stdio.h>

int main() {

    int ventas[2][2][3] = {
        {
            {100, 120, 150},
            {200, 180, 160}
        },
        {
            {130, 140, 170},
            {210, 220, 230}
        }
    };

    for (int sucursal = 0; sucursal < 2; sucursal++) {

        printf("Sucursal %d\n", sucursal + 1);

        for (int vendedor = 0; vendedor < 2; vendedor++) {

            printf("  Vendedor %d: ", vendedor + 1);

            for (int mes = 0; mes < 3; mes++) {

                printf("%d ", ventas[sucursal][vendedor][mes]);

            }

            printf("\n");
        }

        printf("\n");
    }

    return 0;
}
```

### ✅ Resultado esperado

```
Sucursal 1
  Vendedor 1: 100 120 150
  Vendedor 2: 200 180 160

Sucursal 2
  Vendedor 1: 130 140 170
  Vendedor 2: 210 220 230
```

### 📌 Explicación

En este ejemplo se utiliza un arreglo de **2 × 2 × 3**, donde:

- La **primera dimensión** representa las sucursales.
- La **segunda dimensión** representa los vendedores.
- La **tercera dimensión** representa las ventas registradas durante tres meses.

Para recorrer un arreglo tridimensional es necesario utilizar **tres ciclos `for` anidados**, uno por cada dimensión del arreglo.
---

# 🖥️ Evidencia práctica

Como aplicación de los contenidos estudiados en esta unidad, se desarrolló un programa en lenguaje **C** que utiliza un **arreglo tridimensional (2×2×2)**. El programa implementa el uso de **funciones (modularidad)** para mostrar los elementos del arreglo y calcular la suma de todos sus valores, integrando así los dos temas principales de la unidad: modularidad y arreglos.

### 💻 Código desarrollado

```c
#include <stdio.h>

// Función para mostrar los elementos del arreglo tridimensional
void mostrar(int datos[2][2][2]) {
    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            for (int k = 0; k < 2; k++) {
                printf("%d ", datos[i][j][k]);
            }
            printf("\n");
        }
        printf("\n");
    }
}

// Función para sumar todos los elementos del arreglo
int sumar(int datos[2][2][2]) {
    int suma = 0;

    for (int i = 0; i < 2; i++) {
        for (int j = 0; j < 2; j++) {
            for (int k = 0; k < 2; k++) {
                suma += datos[i][j][k];
            }
        }
    }

    return suma;
}

int main() {

    int cubo[2][2][2] = {
        {{1, 2}, {3, 4}},
        {{5, 6}, {7, 8}}
    };

    printf("Contenido del arreglo tridimensional:\n\n");

    mostrar(cubo);

    printf("Suma total: %d\n", sumar(cubo));

    return 0;
}
```

### ▶️ Resultado obtenido

```
Contenido del arreglo tridimensional:

1 2
3 4

5 6
7 8

Suma total: 36
```
<img width="794" height="199" alt="image" src="https://github.com/user-attachments/assets/80c1a279-6b45-4964-9dc0-290192836502" />

### 📌 Análisis

En esta práctica se implementó un **arreglo tridimensional** de tamaño **2 × 2 × 2**, utilizando **tres ciclos `for` anidados** para recorrer todos sus elementos.

Además, el programa fue dividido en dos funciones:

- **`mostrar()`**: se encarga de recorrer y visualizar el contenido del arreglo tridimensional.
- **`sumar()`**: calcula la suma de todos los elementos almacenados en el arreglo.

Esta práctica permitió reforzar el concepto de **modularidad**, ya que las tareas fueron divididas en funciones independientes, y también el manejo de **arreglos tridimensionales**, demostrando cómo recorrer y procesar estructuras de datos con tres dimensiones de manera organizada y eficiente.
---

# 🧠 Principales dificultades

Durante el aprendizaje se presentaron algunas dificultades:

- Comprender la diferencia entre el paso por valor y el paso por referencia.
- Identificar cuándo utilizar funciones para mejorar la organización del código.
- Evitar errores de índices fuera del tamaño del arreglo.
- Manejar correctamente los ciclos anidados en matrices.

---

# 💡 Reflexión crítica

La modularidad y los arreglos representan herramientas fundamentales para desarrollar programas más organizados, eficientes y fáciles de mantener. El uso de funciones permite dividir problemas complejos en tareas más pequeñas, mientras que los arreglos facilitan el almacenamiento y procesamiento de grandes cantidades de datos. Estos conocimientos fortalecen las bases de la programación y preparan al estudiante para el estudio de estructuras de datos más avanzadas.


---

⬅️ [Volver al Portafolio Principal](../README.md)
