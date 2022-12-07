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
