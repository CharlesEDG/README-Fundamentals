## Lunes

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
