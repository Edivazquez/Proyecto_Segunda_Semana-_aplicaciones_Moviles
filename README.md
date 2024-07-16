# Proyecto_Segunda_Semana-_aplicaciones_Moviles
##Autor: Edgar Vazquez Ramirez

La primer semana comenzamos con la definicion de Kotlin e hicimos algunos ejercicios desde la plataforma https://play.kotlinlang.org/#eyJ2ZXJzaW9uIjoiMi4wLjAiLCJwbGF0Zm9ybSI6ImphdmEiLCJhcmdzIjoiIiwibm9uZU1hcmtlcnMiOnRydWUsInRoZW1lIjoiaWRlYSIsImNvZGUiOiIvKipcbiAqIFlvdSBjYW4gZWRpdCwgcnVuLCBhbmQgc2hhcmUgdGhpcyBjb2RlLlxuICogcGxheS5rb3RsaW5sYW5nLm9yZ1xuICovXG5cbmFic3RyYWN0IGNsYXNzIEZpZ3VyYSB7XG4gICAgYWJzdHJhY3QgdmFsIGFyZWE6IERvdWJsZVxuICAgIGFic3RyYWN0IGZ1biBjYWxjdWxhckFyZWEoKTogRG91YmxlXG59XG5cbmltcG9ydCBrb3RsaW4ubWF0aC5QSVxuXG5jbGFzcyBDaXJjdWxvKHZhbCByYWRpbzogRG91YmxlKSA6IEZpZ3VyYSgpIHtcbiAgICBvdmVycmlkZSB2YWwgYXJlYTogRG91YmxlXG4gICAgICAgIGdldCgpID0gUEkgKiByYWRpbyAqIHJhZGlvXG5cbiAgICBvdmVycmlkZSBmdW4gY2FsY3VsYXJBcmVhKCk6IERvdWJsZSB7XG4gICAgICAgIHByaW50bG4oXCJFbCDDoXJlYSBkZWwgY8OtcmN1bG8gZXM6ICRhcmVhXCIpXG4gICAgICAgIHJldHVybiBhcmVhXG4gICAgfVxufVxuXG5jbGFzcyBSZWN0YW5ndWxvKHZhbCBsYXJnbzogRG91YmxlLCB2YWwgYW5jaG86IERvdWJsZSkgOiBGaWd1cmEoKSB7XG4gICAgb3ZlcnJpZGUgdmFsIGFyZWE6IERvdWJsZVxuICAgICAgICBnZXQoKSA9IGxhcmdvICogYW5jaG9cblxuICAgIG92ZXJyaWRlIGZ1biBjYWxjdWxhckFyZWEoKTogRG91YmxlIHtcbiAgICAgICAgcHJpbnRsbihcIkVsIMOhcmVhIGRlbCByZWN0w6FuZ3VsbyBlczogJGFyZWFcIilcbiAgICAgICAgcmV0dXJuIGFyZWFcbiAgICB9XG59XG5cbmZ1biBtYWluKCkge1xuICAgIHZhbCBjaXJjdWxvID0gQ2lyY3Vsbyg1LjApXG4gICAgdmFsIHJlY3Rhbmd1bG8gPSBSZWN0YW5ndWxvKDQuMCwgNi4wKVxuXG4gICAgY2lyY3Vsby5jYWxjdWxhckFyZWEoKVxuICAgIHJlY3Rhbmd1bG8uY2FsY3VsYXJBcmVhKClcbn1cbiJ9

##Ejercicios de Práctica en Kotlin
Declara variables para representar la información de un producto:

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

##Ejercicio 2: Operaciones Aritméticas
Crea dos variables numéricas y realiza las siguientes operaciones:

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

##Ejercicio 3: Incremento y Decremento
Declara una variable numérica y:

Incrementa su valor en 1 y muestra el resultado Decrementa su valor en 1 y muestra el resultado
```sql
var contador = 5
  println("Incremento: ${++contador}")
  println("Decremento: ${--contador}")
```

##Ejercicio 4: Operadores de Asignación Compuesta
Declara una variable numérica y utiliza operadores de asignación compuesta para:

Sumar 5 Multiplicar por 2 Restar 3 Dividir entre 4 Muestra el resultado después de cada operación.
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
##Ejercicio 5: Comparaciones
Declara dos variables numéricas y utiliza operadores de comparación para:

Verificar si son iguales Verificar si la primera es mayor que la segunda Verificar si la segunda es menor o igual que la primera Muestra el resultado de cada comparación.

```sql
val a = 15
  val b = 20
  println("a es igual a b: ${a == b}")
  println("a es mayor que b: ${a > b}")
  println("b es menor o igual que a: ${b <= a}")
```

##Ejercicio 6: Operaciones con Strings
Declara dos variables de tipo String y:

Concaténalas usando el operador + Compara si son iguales Obtén la longitud de ambas y suma los resultados Muestra los resultados.

```sql
val str1 = "Hola"
  val str2 = "Mundo"
  println("Concatenación: ${str1 + " " + str2}")
  println("Son iguales: ${str1 == str2}")
  println("Suma de longitudes: ${str1.length + str2.length}")
```

##Ejercicio 7: Cálculo de Descuento
Crea variables para el precio de un producto y el porcentaje de descuento. Calcula el precio final después del descuento. Muestra el precio original, el descuento y el precio final.

```sql
val precioOriginal = 100.0
  val porcentajeDescuento = 20
  val descuento = precioOriginal * porcentajeDescuento / 100
  val precioFinal = precioOriginal - descuento
  
  println("Precio original: $precioOriginal")
  println("Descuento: $descuento")
  println("Precio final: $precioFinal")
```

##Ejercicio 8: Conversión de Tipos
Declara una variable de tipo String que contenga un número. Conviértela a Int y luego a Double. Realiza una operación aritmética con cada tipo y muestra los resultados.
```sql
  val numeroString = "42"
  val numeroInt = numeroString.toInt()
  val numeroDouble = numeroInt.toDouble()
  
  println("Int + 10: ${numeroInt + 10}")
  println("Double + 10.5: ${numeroDouble + 10.5}")
```

##Ejercicio 9: Operaciones Booleanas
Crea tres variables booleanas y utiliza operadores lógicos (AND, OR, NOT) para combinarlas. Muestra el resultado de al menos tres combinaciones diferentes.
```sql
val p = true
  val q = false
  val r = true
  
  println("p AND q: ${p && q}")
  println("p OR q: ${p || q}")
  println("NOT p: ${!p}")
  println("(p OR q) AND r: ${(p || q) && r}")
```
##Ejercicio 10: Cálculo de IMC
Crea variables para el peso (en kg) y la altura (en metros) de una persona. Calcula el Índice de Masa Corporal (IMC) usando la fórmula: IMC = peso / (altura * altura) Muestra el resultado del IMC.
```sql
 val peso = 70.0 // kg
  val altura = 1.75 // metros
  val imc = peso / (altura * altura)
  
  println("IMC: ${"%.2f".format(imc)}")
```
