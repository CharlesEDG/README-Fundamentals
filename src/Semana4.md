## Lunes:

### Exercise-1 Average sales and commission: Make a program that asks how many sales the seller had, Once the number of sales is entered, ask for the value of each sale until all are entered, then return as a result the average value of sales, and the commission that the seller will take, If the seller had more than 5 sales, his commission will be 15% of the total value of the sales, if he sold 5 or less, his commission will be only 10%.

```python
Algoritmo PromedioVentasComision
	Escribir "Ingrese el número de ventas:"
	leer cantidad_de_ventas
	ingresos_totales = 0
	
	Para venta = 1 Hasta cantidad_de_ventas Con Paso 1 Hacer
		Escribir "Escriba el valor de la venta numero: ",venta
		leer cantidad
		ingresos_totales = ingresos_totales + cantidad
	FinPara
	
	promedio = ingresos_totales / cantidad_de_ventas 
	Imprimir 'La media de ventas es: ', promedio
	
	SI cantidad_de_ventas < 5 Entonces
		Imprimir 'La comisión que recibe el vendedor es: ', ingresos_totales * 0.10
	SiNo
		Imprimir 'La comisión que recibe el vendedor es: ', ingresos_totales * 0.15
	FinSi
	
FinAlgoritmo
```



### Exerise-2 Even or odd: Request a number from 1 to 50, if the number is not between those values, report the error and request it again until you get a valid number, then it shows on the screen all the numbers from 1 to that number, if the number is even it only shows the even numbers, if it is odd it only shows the odd ones.

```python
Algoritmo parOimpar
	Repetir
		Escribir "Ingrese un número entre 1 y 50"
		leer num
		SI  num < 1  | num > 50 Entonces
			Imprimir 'Número inválido'
		FinSi
	Mientras Que num < 1  | num > 50
	
	par =  num % 2 = 0
	
	Para count = 1 Hasta num Con Paso 1 Hacer
		SI count % 2 = 0 & par Entonces
			Imprimir count
		FinSi
		SI count % 2 = 1 & ~(par) Entonces
			Imprimir count
		FinSi
	FinPara
FinAlgoritmo
```



## Martes:

### Exercise-2 Full name: Make a program that takes a first name and a last name, then returns a string with both values ​​with the first letter uppercase and the rest lowercase.

```python
Algoritmo nombreYapellido
	Definir nombre Como Caracter
	Definir a,b,c Como Entero
	Escribir "Ingresa tu nombre y apellido"
	Leer nombre
	a = Longitud(nombre)
	b = 0 
	Para c = 1 Hasta a Con Paso 1 Hacer
		si c == 1 Entonces
			Escribir Mayusculas(Subcadena(nombre,c,c)) Sin Saltar	
		SiNo
			si Subcadena(nombre,c,c) == " " Entonces
				b = 1
			SiNo
				si b == 1 Entonces
					Escribir " " ,Mayusculas(Subcadena(nombre,c,c)) Sin Saltar
				b = 0
				SiNo
					Escribir Subcadena(nombre,c,c) Sin Saltar
				FinSi
			FinSi
		FinSi
	FinPara
	Escribir " "
FinAlgoritmo
```



### Exercise-3 Throw dice: make a program that simulates the roll of 2 dice 10 times, and display for each roll the values of the two dice separated by a space, in case the 2 dice throw the same value in addition to the result, add a string to the ending that says "the dice are the same".

```python
Algoritmo Dados
	Definir a,b,c Como Entero
	c = 0
	Repetir
	a = azar(6) + 1
	b = azar(6) + 1
	si a == b Entonces
		Imprimir ConvertirATexto(a) + " " + ConvertirATexto(b) +"  los dados son iguales"
	SiNo
		Imprimir ConvertirATexto(a) + " " + ConvertirATexto(b)
	FinSi
	c = c + 1
	Hasta Que c == 10
FinAlgoritmo
```



## Miercoles:

### Exercise-1 Distance to zero: Make a program that asks for 5 values and also allows us to know which one is furthest from zero, once obtained it returns that number (the numbers can be negative), showing only the integer part of the number.

```python
Algoritmo alejadoDeCero
	Escribir "Escribe un número"
	leer maximo
	Para contador = 1 Hasta 4 Con Paso 1 Hacer
		Escribir "Escribe un número"
		leer num
		SI Abs(num) > Abs(maximo) Entonces
			maximo = num
		FinSi
	FinPara
	Imprimir Trunc(maximo)
FinAlgoritmo
```



### Exercise-2 Toss coin: From the data we receive first a name and a value, then another name and another value, using the built-in function aleatorio() we simulate the flip of a coin, We must return the name of the winner in capital letters and the value I win, to avoid cheating, if a player puts a value of zero or negative, the opponent automatically wins, in case both cheat, "game canceled" is returned.

```python
Algoritmo MonedaAleatoria
	
	Escribir "Ingrese el nombre del primer jugador"
	leer jugador1
	Escribir "Ingrese el monto a apostar"
	leer monto1
	Escribir "Ingrese el nombre del segundo jugador"
	leer jugador2
	Escribir "Ingrese el monto a apostar"
	leer monto2
	
	SI monto1<=0 | monto2 <=0 Entonces
		SI monto1<=0 & monto2 <=0 Entonces
			Imprimir "Juego Cancelado"
		SiNo
			SI monto1<=0 Entonces
				Imprimir "jugador ganador: ", Mayusculas(jugador2), " monto ganado: 0"
			SiNo
				Imprimir "Jugador ganador: ", Mayusculas(jugador1), " monto ganado: 0"
			FinSi
		FinSi
	SiNo
		SI Aleatorio(1,2) = 1 Entonces
			Imprimir "jugador ganador: ", Mayusculas(jugador1), " monto ganado: ", monto2
		SiNo
			Imprimir "jugador ganador: ", Mayusculas(jugador2), " monto ganado: ", monto1
		FinSi
	FinSi
	
FinAlgoritmo
```



## Jueves:

### Exercise-2 Total price: Create a function called TotalPrice that takes 2 parameters, price and VAT, and returns the price including VAT. if the price exceeds 3000 a 10 percent discount is made on the total price.

```python
Funcion costo <- PrecioTotal (precio, iva)
		Definir costo Como Real;
		SI precio > 3000 Entonces
			costo = ( precio + (precio/100*iva) ) / 100*90
		SiNo
			costo = ( precio + (precio/100*iva) )
		FinSi
	Fin Funcion
	
	Algoritmo EjemploPrecioTotal
		Imprimir PrecioTotal(4000,15)
FinAlgoritmo
```



### Exercise-3 Reverse direction and size: Create a function called ReverseDirectionAndSize that takes some text as a parameter and reverses it, eg: "Hello" -> "olleH" and also reverses the letters if they are uppercase to lowercase and if they are lowercase to uppercase, it should do something. like this:

"HelLO" --> "olLEh"

"Leonardo" --> "ODRANOEl"

"Text" --> "TXEt"

```python
Funcion resultado <- ReverseDirectionAndSize (string)
	Definir resultado Como Caracter;
	resultado = "";
	Para contar = Longitud(string) Hasta 0 Con Paso -1 Hacer
		carta = Subcadena(string,contar,contar);
		SI carta = Mayusculas(carta) Entonces
			carta = Minusculas(carta)
		SiNo
			carta = Mayusculas(carta)
		FinSi
		resultado = Concatenar(resultado, carta)
	FinPara
Fin Funcion

Algoritmo ejemplo_ReverseDirectionAndSize
	Imprimir ReverseDirectionAndSize("Hola")
FinAlgoritmo
```
