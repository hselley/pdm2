# Variables y Propiedades

## Declaración de una variable
Para declarar una variable se debe utilizar la palabra clave ´var´ seguida del nombre
de la variable, su tipo de dato y valor. El valor inicial es opcional.

```swift
var num:Int = 10
```

Las variables pueden cambiar de valor en cualquier momento, ya sea por el flujo del 
programa o por una asignación directa.

```swift
num = 20    // La variable ahora vale 20
```

Si se desea una variable que no cambie su valor, es decir una constante, se debe
utilizar la palabra clave `let` seguido de su nombre, tipo de dato y valor. El 
valor inicial (y permanente) no es opcional.

```swift
let num:Int = 10    // Este valor no puede cambiar
```

Es posible delcarar una variable y asignarle un valor sin indicar el tipo de dato.
Si no se especifica un tipo de dato, Swift inferirá y asignará el tipo de manera
automática. 

```swift 
let ten = 10 // num is an Int
let pi = 3.14 // pi is a Double
let floatPi: Float = 3.14 // floatPi is a Float
```

Los nombres de las variables y constantes no están limitados a caracteres alfanuméricos, 
pueden contener la mayoría de caracteres *Unicode* aunque existen algunas excepciones. 
Los nombres no pueden contener espacios, símbolos matemáticos, flechas, símbolos *Unicode*
privados y no pueden comenzar con un número.

```swift
var π: Double = 3.14159
var 🍎🍎: String = "Apples"
```


###### [Anterior](intro.html) | [Inicio](index.html) | [Siguiente](.html) 