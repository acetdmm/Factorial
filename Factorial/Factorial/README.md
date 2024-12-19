# Cálculo del Factorial en C++

Este proyecto es un programa en C++ que permite calcular el factorial de un número entero positivo utilizando un enfoque iterativo.

## ¿Qué es un factorial?

El factorial de un número entero positivo \( n \), representado como \( n! \), es el producto de todos los enteros positivos desde 1 hasta \( n \). Por ejemplo:

- \( 5! = 5 \times 4 \times 3 \times 2 \times 1 = 120 \)
- \( 0! = 1 \) (definición especial)

## Propósito del código

El programa tiene como objetivo calcular el factorial de un número ingresado por el usuario, validando previamente que sea un número entero positivo.

## ¿Qué incluye el código?

1. **Función Iterativa para el Factorial**
   - La función `factorialIterativo(int n)` calcula el factorial de un número utilizando un bucle `for`.  
     ```cpp
     int factorialIterativo(int n) {
         int resultado = 1;
         for (int i = 1; i <= n; ++i) {
             resultado *= i;
         }
         return resultado;
     }
     ```
   - Toma como entrada un número entero positivo y devuelve el factorial de ese número.

2. **Validación de Entrada**
   - El programa valida que el número ingresado sea un entero positivo. Si se ingresa un número negativo, muestra un mensaje de error y finaliza el programa.

3. **Interacción con el Usuario**
   - Solicita al usuario un número entero positivo, calcula su factorial llamando a la función iterativa, y muestra el resultado en pantalla.

## ¿Cómo usar el programa?

1. Compila el código fuente:
   ```bash
   g++ factorial.cpp -o factorial
