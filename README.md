## Factorial
### El factorial de un número entero positivo se define como el producto de todos los números naturales anteriores o iguales a él.
### ¿Qué es la función factorial?
La función factorial se representa con un signo de exclamación “!” detrás de un número. Esta exclamación quiere decir que hay que multiplicar todos los números enteros positivos que hay entre ese número y el 1.

![Texto alternativo](/factoriales.png)

## Factorial en Kotlin
~~~
fun factorial(n: Int): Int {          # funcion con un parametro
    if (n <= 1) {          # estructura condicional
        return 1           # cuando llega 1 se acaba el programa
    } else {          # si no llega a 1 se resta el parametro n
        return n * factorial(n - 1)
    }
}

fun main() {          # se ejecuta el codigo
    val number = 5          # define el valor 5
    println("El factorial de $number es ${factorial(number)}")         # se invoca o llama al programa
}
~~~
