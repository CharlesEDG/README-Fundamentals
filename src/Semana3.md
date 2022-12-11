## Lunes:

### Exercise-1 Simple calculator: For this challenge you will be performing a simple calculator, this calculator can perform the following operations:

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)
The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. Remember to use conditionals to identify which operations you should execute.

```python
Algoritmo CalculadoraSimple
		Imprimir '======= Calculadora Simple ======='
		Imprimir 'Ingrese primer numero'
		Leer a
		Imprimir 'Ingrese segundo numero'
		Leer b
		Imprimir 'Ingrese una operación: +,-,*,/'
		Leer opc
		Si opc == '+' | opc == '-' | opc == '*' | opc == '/' Entonces
			Imprimir 'Procesando: ' + ConvertirATexto(a) + ' ' + opc + ' ' + ConvertirATexto(b)
			Si opc == '+' Entonces
				Imprimir 'Resultado: ' + ConvertirATexto(a + b)
			SiNo
				Si opc == '-' Entonces
					Imprimir 'Resultado: ' + ConvertirATexto(a - b)
				SiNo
					Si opc == '*' Entonces
						Imprimir 'Resultado: ' + ConvertirATexto(a * b)
					SiNo
						Imprimir  'Resultado: ' + ConvertirATexto(a / b)
					FinSi
				FinSi
			FinSi
		SiNo
			Imprimir 'La operación no es valida'
		FinSi
FinAlgoritmo
```



### Exercise-2 Special number: You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly

This was the code from the developer:
```python
Algoritmo specialNumber
	Leer n
	Si n == 100 Entonces
		Imprimir 'This is a special number'
	FinSi
	Si n < 1000 Entonces
		Imprimir ''
	SiNo
		Imprimir 'Just a regular number'
	FinSi
	Si n % 10 == 0 Entonces
		Imprimir 'This number is multiple of 10'
	FinSi
FinAlgoritmo
```
**Solución**

```python
Algoritmo specialNumber
		Leer n
		Si n == 100 Entonces
			Imprimir 'This is a special number'
		SiNo
			Si n < 1000 & n % 10 == 0 & n <> 100 Entonces
			Imprimir 'This number is almost special'
			SiNo
				Imprimir 'Just a regular number'
			FinSi
			
		FinSi
FinAlgoritmo
```



## Martes:

### Exercise-1 Simple calculator with Switch: For this challenge you will be performing a simple calculator using Switch (Segun), this calculator can perform the following operations:

Sum (+)
Subtract (-)
Multiplication (*)
Division (/)
The calculator must ask the user for two numbers, after asking for the two numbers, you must ask for the operation to be performed, keep in mind that you must show the user the options available (+, -, *, /). The first thing that must be done is to validate that the operation that the user entered is valid, if it is not a valid option, the user must be shown an error message, for example: ⚠️ La operación no es valida and terminate the program. If the operation is valid, show the message: Procesando: <OPERACIÓN A REALIZAR> For, example: if the user has entered the numbers 10 and 15 as well as the operation *, the message should read: Procesando: 10 * 15. After this message the result of the operation must be displayed, following the previous example, the result of operating 10 * 15 is 150, so the program should return: Resultado: 150. Remember to use Switch (Segun) to identify which operations you should execute.

```python
Algoritmo CalculadoraSimple
	Definir op Como Entero
	Definir suma, resta, multiplicación, división, n1, n2 Como Real
	Escribir "Calculadora Básica"
	Escribir "1 Suma:"
	Escribir "2 Resta:"
	Escribir "3 Multiplicación:"
	Escribir "4 División:"
	Escribir "Ingrese la operación requerida:"
	Leer op
	Segun op Hacer
		1:
			Escribir "Ingrese el primer número:"
			Leer n1
			Escribir "Ingrese el segundo número:"
			Leer n2
			suma <- n1 + n2
			Escribir "Procesando: ", n1, " + ", n2
			Escribir "Resultado: ", suma
		2:
			Escribir "Ingrese el primer número:"
			Leer n1
			Escribir "Ingrese el segundo número:"
			leer n2
			resta <- n1 - n2
			Escribir "Procesando: ", n1, " - ", n2
			Escribir "Resultado: ", resta
		3:
			Escribir "Ingrese el primer número:"
			Leer n1
			Escribir "Ingrese el segundo número:"
			Leer n2
			multiplicación <- n1 * n2
			Escribir "Procesando: ", n1, " * ", n2
			Escribir "Resultado: ", multiplicación
		4:
			Escribir "Ingrese el primer número:"
			Leer n1
			Escribir "Ingrese el segundo número:"
			Leer n2
			división <- n1 / n2
			Escribir "Procesando: ", n1, " / ", n2
			Escribir "Resultado: ", división
		De Otro Modo:
			Escribir "La operación no es válida"
		
	Fin Segun
FinAlgoritmo
```



### Exercise-2 Multi Option Program: For this challenge you will create a program with multiple options using Switch (Segun), the options available are the following:

Sum two numbers
Print the day of the week given the day number
Print the length of a given text
This program must have a start menu where the user must select one of the previously described options. When the user selects each of the options, the program will perform the following:

Sum. The user enters two numbers and the result of the sum of both is printed
Print day of the week. The user enters a day of the week using numbers and the name of the day must be printed. For example, if the number 1 is entered, the program prints the text Lunes.
Calculate text length. The user enters a text and the length of the text should be printed. I was able to use the Pseint Longitud function to get the length.
When the user enters an incorrect option, a message should be printed saying that the option is not available.

```python
Algoritmo MultiOpcion
	Escribir "Calculadora Básica"
	Escribir "Opciones Disponibles:"
	Escribir "1. Suma de 2 números:"
	Escribir "2. Imprimir día de la semana:"
	Escribir "3. Imprimir longitud del texto:"
	Escribir "Ingrese la opción requerida:"
	Leer op
	Segun op Hacer
		1:
			Escribir "Ingrese el primer número:"
			Leer n1
			Escribir "Ingrese el segundo número:"
			Leer n2
			suma <- n1 + n2
			Escribir "Resultado: ", suma
		2:
			Escribir "Ingrese el día de la semana en números:"
			Leer día
			Segun día Hacer
				1:
					Imprimir "Lunes"
				2:
					Imprimir "Martes"
				3:
					Imprimir "Miercoles"
				4:
					Imprimir "Jueves"
				5:
					Imprimir "Viernes"
				6:
					Imprimir "Sábado"
				7:
					Imprimir "Domingo"
				De Otro Modo:
					Imprimir "Día incorrecto"
			Fin Segun
		3:
			Escribir "Calcular longitud de texto:"
			Escribir "Ingrese un texto:"
			Leer cadena
			n = Longitud(cadena)
			Escribir "Resultado ", cadena , " Tiene ", n, " carácteres"
		De Otro Modo:
			Escribir "Opción incorrecta"
		
	Fin Segun
FinAlgoritmo
```



## Miercoles:

### Exercise-1 Multiplication Tables: For this challenge you will create a program to calculate the multiplication tables for a given number using While (Mientras). The user must enter a number and then the multiplication table for the number must be printed.

```python
Algoritmo TablaMultiplicar
	Definir x, n Como Entero
	Imprimir "== Tabla de Multiplicar =="
	Escribir "Ingrese un número"
	Leer n
	x = 1
	Mientras x <= 10 Hacer
		Escribir n, " x ", x, " = ", n * x
		x = x + 1
		
	FinMientras
FinAlgoritmo
```



### Exercise-2 Simple Calculator with Do While: For this challenge we are going to use the simple calculator that we made in the challenge 02 but now adding the functionality to perform a calculation again without finishing the program. The program should ask us if we want to use another operation and if the user answers yes then we can perform a new operation. To solve this challenge remember to use Do while (Repetir Hasta Que).

```python
Algoritmo CalculadoraSimple
	Imprimir '======= Calculadora Simple ======='
	Repetir
	Imprimir 'Ingrese primer numero'
	Leer a
	Imprimir 'Ingrese segundo numero'
	Leer b
	Imprimir 'Ingrese una operación: +,-,*,/'
	Leer opc
	Si opc == '+' | opc == '-' | opc == '*' | opc == '/' Entonces
		Imprimir 'Procesando: ' + ConvertirATexto(a) + ' ' + opc + ' ' + ConvertirATexto(b)
		Si opc == '+' Entonces
			Imprimir 'Resultado: ' + ConvertirATexto(a + b)
		SiNo
			Si opc == '-' Entonces
				Imprimir 'Resultado: ' + ConvertirATexto(a - b)
			SiNo
				Si opc == '*' Entonces
					Imprimir 'Resultado: ' + ConvertirATexto(a * b)
				SiNo
					Imprimir  'Resultado: ' + ConvertirATexto(a / b)
				FinSi
			FinSi
		FinSi
	SiNo
		Imprimir 'La operación no es valida'
	FinSi
	Imprimir 'Deseas continuar con otra operacion ? S / N'
	Leer Continuar
	Hasta Que 	Continuar == "N" | Continuar == "n"
FinAlgoritmo
```



## Jueves

### Exercise-1 Multiplication Tables with For: For this challenge you will create a program to calculate the multiplication tables for a given number using the For(Para) loop. The user must enter a number and then the multiplication table for the number must be printed.

```python
Algoritmo TablaMultiplicar
	Escribir "Ingrese un número: ";
	Leer tabla;
	Para n <- 1 Hasta 10 Hacer
		Escribir tabla," x ", n, " = ", n*tabla;
	FinPara
FinAlgoritmo
```



### Exercise-2 Ascending and Descending Numbers: For this challenge we are going to print numbers in ascending or descending order. The user must enter a number, then he must enter if he wants to print the numbers in ascending or descending order. If the user chooses ascending, the numbers will be printed from the number 0 to the number entered, otherwise the numbers will be printed descending from the number entered to the number 0.To solve this challenge remember to use the For(Para) loop.

```python
Algoritmo TabMultiAsc
	Escribir "Ingrese un número: ";
	Leer num;
	Escribir "1. Ascendente"
	Escribir "2. Descendente"
	Leer opc
	si opc == 1 Entonces
		Para n <- 0 Hasta num Hacer
			Escribir Número, n
			
		FinPara
	SiNo
		Si opc == 2 Entonces
			
			Para n <- num Hasta 0 con paso -1 Hacer
				Escribir Número, n
				
			FinPara
		SiNo
			Escribir "Opción incorrecta"
		FinSi
	FinSi
FinAlgoritmo
```



### Exercise-3 Greetings: For this challenge, you need to create a program that prints a greeting based on an hour entered. The program should do the following:

Print Buenos dias! if the hour is from 0 to 12
Print Buenas tardes! if the hour is from 13 to 18
Print Buenas noches! if the hour is from 19 to 23
Ask the user if he wants to perform another greeting. If the answer is Si, the program must start again.
At the end of the program, print out the number of times the program has greeted.

```python
Algoritmo Saludos
	Definir continuar Como Cadena
	Definir cantidadSaludos Como Entero
	cantidadSaludos <- 0
	continuar <- 'Si'
	Repetir
		Escribir "Ingrese la hora actual"
		
	Leer hora
	si hora <= 12 Entonces
		Imprimir "Buenos días!"
	SiNo
		si hora = 13 | hora <= 18 Entonces
			Imprimir "Buenos tardes!"
		SiNo
			si hora = 19 | hora <= 23 Entonces
				Imprimir "Buenos noches!"
			FinSi
			
		FinSi
	FinSi
	cantidadSaludos <- cantidadSaludos + 1
	Escribir "Desea realizar otro saludo? Si/No"
	Leer continuar
	Hasta Que continuar == "N" | continuar == "n"
	Imprimir "Cantidad de Saludos realizados: " + ConvertirATexto( cantidadSaludos)

FinAlgoritmo
```
