# Ingreso de datos desde la terminal

Swift tiene la instrucción `readLine()` que permite 
solicitar al usuario una entrada desde el teclado 
y almacenarla en una constante o variable 
*String Opcional*. 

Para leer una entrada y guardarla en una constante 
*x*, se debe *desenvolver* la entrada dado que se
traba de un *String Opcional*. Por lo tanto, el 
código queda de la siguiente forma:

```swift
if let x = readLine() {
    print("La entrada es: \(x)")
}
```

Si lo que se ingresa a través de readLine debe
ser tratado como un número entero, se debe hacer la
conversión con el método *Int* pero es necesario
desenvolver el *Int Opcional*. El código queda de la
siguiente forma:

```swift 
if let entrada = readLine() {
  if let numero = Int(entrada) {
      print(numero)
  }
}
```
Si deseara convertir la entrada a otro tipo de dato
numérico, bastaría con usar de la misma forma los 
métodos *Float* o *Double*.

Si desea recibir dos números desde `readLine`, primero
se leen las entradas y luego se deben desenvolver los 
*String Opcionales* y los *Int Opcionales* utilizando un 
solo `if` simultáneo. El código queda de la siguiente
forma:

```swift
// Se piden dos entradas:
let entrada1 = readLine()
let entrada2 = readLine()

// Se desenvuelven simultáneamente:
if let respuesta1 = entrada1, 
  let respuesta2 = entrada2, 
  let num1 = Int(respuesta1), 
  let num2 = Int(respuesta2) {
    print("The sum of \(num1) and \(num2) is \(num1 + num2)")
}
```