# Proyecto_Segunda_Semana-_Aplicaciones_Moviles 

## Autor: Edgar Vazquez Ramirez. 
 
![image](https://github.com/user-attachments/assets/eb6e11fa-5923-4240-a504-17f628e93eda)

 
La primera semana comenzamos con la definición de Kotlin e hicimos algunos ejercicios desde la plataforma. 

![image](https://github.com/user-attachments/assets/82616d24-85f2-4bb6-975c-6b47dff0b6e4)


## 1: ¿Qué es Kotlin?
### Declara variables para representar la información de un producto:

Nombre del producto (String)
Precio (Double)
Disponible en inventario (Boolean)
Código de producto (String) Imprime todas las variables.

```sql
  val nombreProducto: String = "Laptop Gaming"
  val precio: Double = 1299.99
  val disponible: Boolean = true
  val codigoProducto: String = "LPT-001"

  println("Producto: $nombreProducto")
  println("Precio: $precio")
  println("Disponible: $disponible")
  println("Código: $codigoProducto")
```

### Ejercicio 2: Operaciones Aritméticas
# Crea dos variables numéricas y realiza las siguientes operaciones:

Suma Resta Multiplicación División Módulo Imprime el resultado de cada operación.

```sql
val num1 = 20
  val num2 = 6

  println("Suma: ${num1 + num2}")
  println("Resta: ${num1 - num2}")
  println("Multiplicación: ${num1 * num2}")
  println("División: ${num1 / num2}")
  println("Módulo: ${num1 % num2}")
```

### Ejercicio 3: Incremento y Decremento
# Declara una variable numérica y: Incrementa su valor en 1 y muestra el resultado Decrementa su valor en 1 y muestra el resultado

```sql
var contador = 5
  println("Incremento: ${++contador}")
  println("Decremento: ${--contador}")
```

### Ejercicio 4: Operadores de Asignación Compuesta
# Declara una variable numérica y utiliza operadores de asignación compuesta para: Sumar 5 Multiplicar por 2 Restar 3 Dividir entre 4 Muestra el resultado después de cada operación.

```sql
var numero = 10
  numero += 5
  println("Después de sumar 5: $numero")
  numero *= 2
  println("Después de multiplicar por 2: $numero")
  numero -= 3
  println("Después de restar 3: $numero")
  numero /= 4
  println("Después de dividir entre 4: $numero")
```

### Ejercicio 5: Comparaciones
# Declara dos variables numéricas y utiliza operadores de comparación para: Verificar si son iguales Verificar si la primera es mayor que la segunda Verificar si la segunda es menor o igual que la primera Muestra el resultado de cada comparación.

```sql
val a = 15
  val b = 20
  println("a es igual a b: ${a == b}")
  println("a es mayor que b: ${a > b}")
  println("b es menor o igual que a: ${b <= a}")
```

### Ejercicio 6: Operaciones con Strings
# Declara dos variables de tipo String y:Concaténalas usando el operador + Compara si son iguales Obtén la longitud de ambas y suma los resultados Muestra los resultados.

```sql
val str1 = "Hola"
  val str2 = "Mundo"
  println("Concatenación: ${str1 + " " + str2}")
  println("Son iguales: ${str1 == str2}")
  println("Suma de longitudes: ${str1.length + str2.length}")
```

### Ejercicio 7: Cálculo de Descuento
# Crea variables para el precio de un producto y el porcentaje de descuento. Calcula el precio final después del descuento. Muestra el precio original, el descuento y el precio final.

```sql
val precioOriginal = 100.0
  val porcentajeDescuento = 20
  val descuento = precioOriginal * porcentajeDescuento / 100
  val precioFinal = precioOriginal - descuento
  
  println("Precio original: $precioOriginal")
  println("Descuento: $descuento")
  println("Precio final: $precioFinal")
```

### Ejercicio 8: Conversión de Tipos
# Declara una variable de tipo String que contenga un número. Conviértela a Int y luego a Double. Realiza una operación aritmética con cada tipo y muestra los resultados.

```sql
  val numeroString = "42"
  val numeroInt = numeroString.toInt()
  val numeroDouble = numeroInt.toDouble()
  
  println("Int + 10: ${numeroInt + 10}")
  println("Double + 10.5: ${numeroDouble + 10.5}")
```

### Ejercicio 9: Operaciones Booleanas
# Crea tres variables booleanas y utiliza operadores lógicos (AND, OR, NOT) para combinarlas. Muestra el resultado de al menos tres combinaciones diferentes.
```sql
val p = true
  val q = false
  val r = true
  
  println("p AND q: ${p && q}")
  println("p OR q: ${p || q}")
  println("NOT p: ${!p}")
  println("(p OR q) AND r: ${(p || q) && r}")
```
### Ejercicio 10: Cálculo de IMC
# Crea variables para el peso (en kg) y la altura (en metros) de una persona. Calcula el Índice de Masa Corporal (IMC) usando la fórmula: IMC = peso / (altura * altura) Muestra el resultado del IMC.

```sql
 val peso = 70.0 // kg
  val altura = 1.75 // metros
  val imc = peso / (altura * altura)
  
  println("IMC: ${"%.2f".format(imc)}")
```

### Sesión 2: Fundamentos de programación

## Ejercicio 1: Calculadora de volumen de cilindro: Crea una función que calcule el volumen de un cilindro dado su radio y altura.
```sql
import kotlin.math.PI

fun calcularVolumenCilindro(radio: Double, altura: Double): Double {
    return PI * radio * radio * altura
}

fun main() {
    println("Volumen del cilindro: ${calcularVolumenCilindro(5.0, 10.0)}")
}
```

### Ejercicio 2: Verificador de número primo
# Implementa una función que determine si un número es primo.
```sql

fun esPrimo(numero: Int): Boolean {
    if (numero <= 1) return false
    for (i in 2..Math.sqrt(numero.toDouble()).toInt()) {
        if (numero % i == 0) return false
    }
    return true
}

fun main() {
    println("¿Es 17 primo? ${esPrimo(17)}")
    println("¿Es 24 primo? ${esPrimo(24)}")
}
```

### Ejercicio 3: Validador de email con función local
# Desarrolla una función que valide una dirección de email utilizando una función local.
```sql
 fun validarEmail(email: String): Boolean {
    fun tieneArrobaYPunto(str: String): Boolean {
        return str.contains("@") && str.contains(".")
    }

    return email.isNotEmpty() && tieneArrobaYPunto(email)
}

fun main() {
    println("¿Es válido user@example.com? ${validarEmail("user@example.com")}")
    println("¿Es válido invalid-email? ${validarEmail("invalid-email")}")
}
```
### Ejercicio 4: Clasificador de edades usando when
# Crea una función que clasifique a una persona según su edad utilizando when.

```sql
fun clasificarEdad(edad: Int) {
    when (edad) {
        in 0..12 -> println("Niño")
        in 13..19 -> println("Adolescente")
        in 20..64 -> println("Adulto")
        else -> println("Adulto mayor")
    }
}

fun main() {
    clasificarEdad(8)
    clasificarEdad(15)
    clasificarEdad(35)
    clasificarEdad(70)
}
```

### Ejercicio 5: Imprimir números pares en un rango
# Utiliza un ciclo for para imprimir los números pares en un rango dado.

```sql
fun imprimirPares(inicio: Int, fin: Int) {
    for (i in inicio..fin step 2) {
        if (i % 2 == 0) {
            println(i)
        }
    }
}

fun main() {
    imprimirPares(1, 10)
}
```
### Ejercicio 6: Contar vocales en una lista de palabras
# Usa una lista y un ciclo para contar las vocales en una lista de palabras.

```sql
un contarVocales(palabras: List<String>): Int {
    val vocales = setOf('a', 'e', 'i', 'o', 'u')
    var totalVocales = 0
    
    for (palabra in palabras) {
        totalVocales += palabra.lowercase().count { it in vocales }
    }
    
    return totalVocales
}

fun main() {
    val listaPalabras = listOf("Hola", "Mundo", "Kotlin")
    println("Total de vocales: ${contarVocales(listaPalabras)}")
}
```
### Ejercicio 7: Diccionario de sinónimos
# Crea un mapa de sinónimos y una función para obtener sinónimos de una palabra.

```sql
val sinonimos = mapOf(
    "feliz" to listOf("contento", "alegre", "dichoso"),
    "triste" to listOf("melancólico", "abatido", "apenado"),
    "enojado" to listOf("furioso", "irritado", "colérico")
)

fun obtenerSinonimos(palabra: String): List<String> {
    return sinonimos[palabra.lowercase()] ?: listOf("No se encontraron sinónimos")
}

fun main() {
    println("Sinónimos de 'feliz': ${obtenerSinonimos("feliz")}")
    println("Sinónimos de 'cansado': ${obtenerSinonimos("cansado")}")
}
```

### Ejercicios de Kotlin: Clases, Objetos y Constructores

# Ejercicio 1: Clase Libro

```sql
Crea una clase Libro con los atributos titulo, autor y añoPublicacion. Incluye un constructor primario y un método para imprimir la información del libro.
class Libro(val titulo: String, val autor: String, val añoPublicacion: Int) {
    fun imprimirInfo() {
        println("'$titulo' por $autor ($añoPublicacion)")
    }
}

fun main() {
    val miLibro = Libro("1984", "George Orwell", 1949)
    miLibro.imprimirInfo()
}
```
### Ejercicio 2: Clase Cuenta Bancaria
# Diseña una clase CuentaBancaria con un atributo privado saldo. Incluye métodos para depositar, retirar y consultar saldo.

```sql
class CuentaBancaria(saldoInicial: Double) {
    private var saldo = saldoInicial

    fun depositar(monto: Double) {
        saldo += monto
        println("Depósito de $monto realizado. Nuevo saldo: $saldo")
    }

    fun retirar(monto: Double) {
        if (monto <= saldo) {
            saldo -= monto
            println("Retiro de $monto realizado. Nuevo saldo: $saldo")
        } else {
            println("Saldo insuficiente")
        }
    }

    fun consultarSaldo() = println("Saldo actual: $saldo")
}

fun main() {
    val cuenta = CuentaBancaria(100.0)
    cuenta.depositar(50.0)
    cuenta.retirar(30.0)
    cuenta.consultarSaldo()
}
```

### Ejercicio 3: Clase con Constructor Secundario
# Crea una clase Rectangulo con atributos ancho y alto. Incluye un constructor primario y un constructor secundario que inicialice ambos valores con el mismo número.

```sql
class Rectangulo(val ancho: Double, val alto: Double) {
    constructor(lado: Double) : this(lado, lado)

    fun calcularArea() = ancho * alto
}

fun main() {
    val rectangulo1 = Rectangulo(5.0, 3.0)
    val cuadrado = Rectangulo(4.0)

    println("Área del rectángulo: ${rectangulo1.calcularArea()}")
    println("Área del cuadrado: ${cuadrado.calcularArea()}")
}
```
### Ejercicio 4: Getters y Setters Personalizados
#Implementa una clase Temperatura con un atributo en Celsius. Incluye getters y setters personalizados para obtener y establecer la temperatura en Fahrenheit.

```sql
class Temperatura(celsius: Double) {
    var celsius = celsius
        set(value) {
            field = value
            println("Temperatura establecida a $value°C")
        }

    var fahrenheit: Double
        get() = celsius * 9/5 + 32
        set(value) {
            celsius = (value - 32) * 5/9
            println("Temperatura establecida a $value°F")
        }
}

fun main() {
    val temp = Temperatura(25.0)
    println("En Fahrenheit: ${temp.fahrenheit}°F")
    temp.fahrenheit = 68.0
    println("En Celsius: ${temp.celsius}°C")
}
```

### Ejercicio 5: Clase con Propiedades Lazy
# Crea una clase Calculadora con una propiedad pi que se inicialice de manera perezosa (lazy) y un método para calcular el área de un círculo.

```sql
class Calculadora {
    val pi: Double by lazy {
        println("Calculando pi...")
        3.14159265359
    }

    fun areaCirculo(radio: Double): Double {
       #  return pi * radio * radio
    }
}

fun main() {
    val calc = Calculadora()
    println("Área de un círculo con radio 5: ${calc.areaCirculo(5.0)}")
    println("Área de un círculo con radio 3: ${calc.areaCirculo(3.0)}")
}
```
### Ejercicio 6: Clase con Métodos de Extensión
# Define una clase Persona con propiedades nombre y edad. Luego, crea un método de extensión para imprimir un saludo personalizado.

```sql
class Persona(val nombre: String, val edad: Int)

fun Persona.saludar() {
    println("Hola, mi nombre es $nombre y tengo $edad años.")
}

fun main() {
    val persona = Persona("Ana", 28)
    persona.saludar()
}
```
## Sesion-04

### 1. Herencia y Polimorfismo
# Crea una clase base Animal con un método hacerSonido(). Luego, crea dos clases derivadas Perro y Gato que hereden de Animal y sobrescriban el método hacerSonido(). Finalmente, crea una función que reciba un Animal y llame a su método hacerSonido().

```sql
open class Animal {
    open fun hacerSonido() {
        println("El animal hace un sonido")
    }
}

class Perro : Animal() {
    override fun hacerSonido() {
        println("El perro ladra")
    }
}

class Gato : Animal() {
    override fun hacerSonido() {
        println("El gato maulla")
    }
}

fun hacerSonar(animal: Animal) {
    animal.hacerSonido()
}

fun main() {
    val perro = Perro()
    val gato = Gato()
    
    hacerSonar(perro) // Imprime: El perro ladra
    hacerSonar(gato)  // Imprime: El gato maulla
}
```

### 2. Clases Abstractas
# Crea una clase abstracta Figura con un método abstracto calcularArea(). Luego, implementa dos clases concretas Circulo y Rectangulo que hereden de Figura e implementen el método calcularArea().

```sql
abstract class Figura {
    abstract fun calcularArea(): Double
}

class Circulo(private val radio: Double) : Figura() {
    override fun calcularArea(): Double {
        return Math.PI * radio * radio
    }
}

class Rectangulo(private val base: Double, private val altura: Double) : Figura() {
    override fun calcularArea(): Double {
        return base * altura
    }
}

fun main() {
    val circulo = Circulo(5.0)
    val rectangulo = Rectangulo(4.0, 6.0)
    
    println("Área del círculo: ${circulo.calcularArea()}")
    println("Área del rectángulo: ${rectangulo.calcularArea()}")
```
### 3. Interfaces
# Crea una interfaz Volador con un método volar(). Luego, implementa esta interfaz en las clases Ave y Avion. Crea una función que reciba un Volador y llame a su método volar().

```sql
interface Volador {
    fun volar()
}

class Ave : Volador {
    override fun volar() {
        println("El ave vuela moviendo sus alas")
    }
}

class Avion : Volador {
    override fun volar() {
        println("El avión vuela usando motores")
    }
}

fun hacerVolar(volador: Volador) {
    volador.volar()
}

fun main() {
    val ave = Ave()
    val avion = Avion()
    
    hacerVolar(ave)   // Imprime: El ave vuela moviendo sus alas
    hacerVolar(avion) // Imprime: El avión vuela usando motores
}
```
### 4. Data Classes
# Crea una data class Libro con propiedades para título, autor y año de publicación. Luego, crea una lista de libros y utiliza las funciones generadas automáticamente para copiar un libro y comparar dos libros.

```sql
data class Libro(val titulo: String, val autor: String, val anioPublicacion: Int)

fun main() {
    val libro1 = Libro("1984", "George Orwell", 1949)
    val libro2 = Libro("Cien años de soledad", "Gabriel García Márquez", 1967)
    val libro3 = libro1.copy(titulo = "Rebelión en la granja")
    
    val libros = listOf(libro1, libro2, libro3)
    
    println(libro1 == libro2) // false
    println(libro1 == libro1.copy()) // true
    
    libros.forEach { println(it) }
}
```
### 5. Companion Object
# Crea una clase Contador con un companion object que mantenga un contador global de instancias creadas. Cada vez que se cree una nueva instancia de Contador, el contador global debe incrementarse.

```sql
class Contador {
    companion object {
        private var contadorGlobal = 0
        
        fun obtenerContadorGlobal(): Int {
            return contadorGlobal
        }
    }
    
    init {
        contadorGlobal++
    }
}

fun main() {
    println(Contador.obtenerContadorGlobal()) // 0
    
    val contador1 = Contador()
    println(Contador.obtenerContadorGlobal()) // 1
    
    val contador2 = Contador()
    val contador3 = Contador()
    println(Contador.obtenerContadorGlobal()) // 3
}
```
### 6. Herencia Múltiple con Interfaces
# Crea dos interfaces Nadador y Corredor con métodos nadar() y correr() respectivamente. Luego, crea una clase Triatleta que implemente ambas interfaces. Finalmente, crea una función que reciba un objeto y verifique si puede nadar, correr o ambos.

```sql
interface Nadador {
    fun nadar()
}

interface Corredor {
    fun correr()
}

class Triatleta : Nadador, Corredor {
    override fun nadar() {
        println("El triatleta está nadando")
    }
    
    override fun correr() {
        println("El triatleta está corriendo")
    }
}

fun verificarHabilidades(obj: Any) {
    if (obj is Nadador) {
        obj.nadar()
    }
    if (obj is Corredor) {
        obj.correr()
    }
}

fun main() {
    val triatleta = Triatleta()
    verificarHabilidades(triatleta)
}
```
# Sesión 5: Programación funcional

```sql

data class Libro(val titulo: String, val autor: String, val añoPublicación: Int)
fun main(){
    val libro1 = Libro("1984", "George Orwell", 1949)
    val libro2 = Libro("Cien años de Soledad", "Gabriel García Márquez", 1967)
    val libro3 = libro1.copy(titulo = "Rebelion de la granja")
    
    val libros = listOf(libro1, libro2, libro3)
    
    println(libro1 == libro2)
    println(libro1 == libro1.copy())
    
    libros.forEach {println(it)}
}
```

### 5. Companion Object

```sql
class Contador{
    companion object{
        private var contadorGlobal = 0 
        
        fun obtenerContadorGlobal(): Int {
            return contadorGlobal
        }
    }
    
    init {
        contadorGlobal++
    }
}
fun main(){
    println(Contador.obtenerContadorGlobal())
    val contador1 = Contador()
    println(Contador.obtenerContadorGlobal())
    
    val contador2 = Contador()
    val contador3 = Contador()
    println(Contador.obtenerContadorGlobal())
}
```
### 6. Herencia Múltiple con Interfaces
# Crea dos interfaces Nadador y Corredor con métodos nadar() y correr() respectivamente. Luego, crea una clase Triatleta que implemente ambas interfaces. Finalmente, crea una función que reciba un objeto y verifique si puede nadar, correr o ambos.

```sql
interface Nadador {
    fun nadar()
}

interface Corredor {
    fun correr()
}

class Triatleta : Nadador, Corredor {
    override fun nadar() {
        println("El triatleta está nadando")
    }
    
    override fun correr() {
        println("El triatleta está corriendo")
    }
}

fun verificarHabilidades(obj: Any) {
    if (obj is Nadador) {
        obj.nadar()
    }
    if (obj is Corredor) {
        obj.correr()
    }
}

fun main() {
    val triatleta = Triatleta()
    verificarHabilidades(triatleta)
}
```
### Crea una función literal que calcule el cuadrado de un número y úsala para calcular el cuadrado de 5.

```sql
val cuadrado = {x: Int -> x * x}
fun main (){
    println(cuadrado(5))
}
```
### Función de orden superior personalizada: Crea una función de orden superior llamada aplicarOperacion que tome dos números y una función, y aplique esa función a los números.

```sql
fun aplicarOperacion(a: Int, b: Int, operacion: (Int, Int) -> Int): Int{
    return operacion(a,b)
} 
val suma = aplicarOperacion(5.0, 3.0){x, y -> x + y}
fun main(){
    println("Suma: $suma")
}
```
### Crea una función de orden superior llamada transformarLista que tome una lista de números enteros y una función de transformación. La función debe aplicar la transformación a cada elemento de la lista y devolver una nueva lista con los resultados.
```sql
fun main(){
fun transformarLista(lista: List<Int>, transformacion: (Int) -> Int): List <Int> {
    return lista.map {transformacion(it)}
}
val numeros = listOf(1, 2, 3, 4, 5)
val listaDoble = transformarLista(numeros){ it * 2}
println("Lista duplicada: $listaDoble")
}
```

### Ejercicios de Programación Funcional en Kotlin
# 1. Expresiones Lambda

```sql
val obtenerMayor: (Int, Int) -> Int = { a, b -> if (a > b) a else b }

fun main() {
    val numeros = listOf(5, 2, 10, 8, 3, 1)
    val maximo = numeros.reduce(obtenerMayor)
    println("El número más grande es: $maximo")
}
```
### 2. Funciones de Orden Superior
# Crea una función de orden superior llamada operacion que tome dos números enteros y una función como parámetros. Esta función debe aplicar la función recibida a los dos números. Luego, utiliza esta función de orden superior para realizar suma, resta y multiplicación.
```sql
fun operacion(a: Int, b: Int, func: (Int, Int) -> Int): Int {
    return func(a, b)
}

fun main() {
    val suma = { x: Int, y: Int -> x + y }
    val resta = { x: Int, y: Int -> x - y }
    val multiplicacion = { x: Int, y: Int -> x * y }

    println("Suma: ${operacion(5, 3, suma)}")
    println("Resta: ${operacion(5, 3, resta)}")
    println("Multiplicación: ${operacion(5, 3, multiplicacion)}")
}

```

### 3. Inline Functions
# Crea una función inline que tome una lambda como parámetro y la ejecute dentro de un bloque try-catch. Luego, usa esta función para ejecutar una operación que podría lanzar una excepción.
```sql
inline fun saludar(nombre: String){
    println("Hola, $nombre")
}

    
fun main (){
    println("Hi soy Edgar")
}
![image](https://github.com/user-attachments/assets/51f272a5-892c-4a14-aaa3-17095d9a0aee)


```
### 4. Filter y Map
# Dada una lista de palabras, utiliza filter para obtener solo las palabras que tengan más de 5 letras, y luego usa map para convertir estas palabras a mayúsculas.
```sql
fun main() {
    val palabras = listOf("gato", "perro", "elefante", "ratón", "hipopótamo")
    
    val resultado = palabras
        .filter { it.length > 5 }
        .map { it.uppercase() }
    
    println(resultado)
}

```
### 5. Partition y FlatMap
# Dada una lista de números, usa partition para separar los números pares e impares. Luego, usa flatMap para crear una nueva lista que contenga el cuadrado de los números pares y el cubo de los números impares.
```sql
<fun main() {
    val numeros = listOf(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
    
    val (pares, impares) = numeros.partition { it % 2 == 0 }
    
    val resultado = listOf(pares, impares).flatMap { lista ->
        lista.map { numero ->
            if (numero % 2 == 0) numero * numero
            else numero * numero * numero
        }
    }
    
    println(resultado)
}
```

### 6. Reduce y ForEach
# Crea una lista de números decimales que representen precios. Utiliza reduce para calcular el total de los precios. Luego, usa forEach para imprimir cada precio con un formato específico (por ejemplo, con dos decimales y el símbolo de moneda).
```sql
fun main() {
    val precios = listOf(19.99, 24.50, 9.95, 4.20, 99.99)
    
    val total = precios.reduce { acc, precio -> acc + precio }
    
    println("Total: ${"%.2f".format(total)}")
    
    precios.forEach { precio ->
        println("${"$%.2f".format(precio)}")
    }
}

```


