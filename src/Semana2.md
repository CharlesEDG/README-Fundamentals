## Lunes:

### Exercise-1 Logic Problem: The teacher asks his 5 students if they studied mathematics yesterday.

Alice: "Nobody studied math yesterday".  
Bob: "1 person studied math yesterday".  
Charlie: "2 people studied math yesterday".  
Dan: "3 people studied mathematics yesterday".  
Eva: "4 people studied mathematics yesterday".  

The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?

    Bob está diciendo la verdad ya que la respuesta de los demás no concuerda con que todos hayan estudiado
    
    
    
    
### Exercise-2 Cereal vrs Milk: Create an algorithm to prepare a bowl of cereal with milk. Represent the result in pseudocode and in a flowchart.

    Datos
    * Un plato
    * Cereal
    * Leche
    1- Agarrar el plato
       1.1 Ponerlo en la mesa
    2- Abrir el cereal
    3- Colocar el cereal
       3.1 Repetir hasta llenar 3/4 partes del plato
    4- Abrir la leche
    5- Colocar la leche
       5.1 Repetir hasta que el cereal llegue al tope
       
![ Diagrama de flujo ](https://github.com/CharlesEDG/README-Fundamentals/blob/main/Diagrama.PNG?raw=true)



## Martes:

### Exercise-2 Print my name: This will be a guided challenge, the idea is for you to use PSeInt. For this challenge, we will print your name on the screen, a simple task that will help us to review the way PSeInt works.

```python
Algoritmo MyName
	Imprimir "Charles Diaz"
FinAlgoritmo
```




### Exercise-3 Print my name & age: This challenge is similar to the previous guided challenge, but now you will try alone. For this challenge, you will need to create an algorithm in Pseudocode using PSeInt that prints your name and your age in separate lines, remeber that your name should be a string and your age a number

```python
Algoritmo MyNameAndAge
	Imprimir "Charles Diaz"
	Imprimir 30
FinAlgoritmo
```



## Miercoles:

## Exercise-2 Mod: The challenge for you now is to create a PSeInt program that will receive a number from the user and add the mod operator using the even/odd case ( X % 2 ) where X is the user input.

```python
Algoritmo evenOdd
	Leer X
	Imprimir X % 2
FinAlgoritmo
```



## Exercise-3 Register form: You are given the task to create a registration form for new users, this form should ask the user for the following information:

First name
Last name
Age
Email
Address
At the end of the program, you should print all the information added from the user in a friendly way.

```python
Algoritmo Formulario
	Escribir "Ingrese su nombre"
	Leer nombre
	Escribir "Ingrese su apellido"
	Leer apellido
	Escribir "Ingrese su edad"
	Leer edad
	Escribir "Ingrese su correo eletronico"
	Leer correo 
	Escribir "Ingrese su dirección"
	Leer Dirección
	Imprimir "Nombre completo:" +" "+ nombre + " "+ apellido 
	Imprimir "Edad: " + edad
	Imprimir "Correo electrónico: " + correo
	Imprimir "Dirección: " + dirección
FinAlgoritmo
```



## Jueves:

## Exercise-1 Truth tables: You are going to learn about three main logical operations used in programming, these operations are called AND, OR, and NOT. Each of the operations uses booleans as operands, and when applying the operations a result is generated, which is also a boolean, this is easier to check using the Truth Tables for each of the operations, now your task is for you to learn, and add the Truth Tables for each of the operations add them to your README and check if the following operations are correct by answering ✅ or ❌ at the end of each operation.

1. T & T = T ✅
2. T & F = F ✅
3. F & T = T ❌
4. F & F = F ✅
5. T | T = T ✅
6. T | F = F ❌
7. F | T = T ✅
8. F | F = F ✅
9. ~T = T ❌
10. ~F = T ✅
11. (T & F) | (~F) = T ✅
12. (T | F ) & (F | F) = T ❌
13. ~((T | F ) & (F | F)) & F = T ❌
14. ~((T | F ) & (F | F)) & T = F ❌



## Exercise-2 Boolean results: You have been assigned to verify and explain a code created by one of your colleagues, the idea is that you can describe the value that each variable has within the code as well as what was done for each line. What is expected of you is that you add comments below each line showing the value that the variable would have and a short explanation of how that value is reached.

This is the code:

```python
Algoritmo boolean
	a <- 5 == 3 // Falso
	b <- 4 <> 3 // Verdadero
	c <- 7 > 7 // Falso
	d <- 4 < 4 // Falso
	e <- 100 <= 90 // Falso
	f <- 40 >= 40 // Verdadero
FinAlgoritmo
```



## Exercise-3 Identify odd and even numbers: Remember the last challenge about the Mod operator? well, today your task will be to create a program that will be able to detect based on the user input if the number is odd or even. The process should be the following:

The user enters a number
Your algorithm detects if the number is odd or even (remember to use conditional statements Si...Entonces)
Print ‘Número: x es par’ if the number is even (x is the number the user enters)
Print ‘Número: x es impar’ if the number is odd (x is the number the user enters)

```python
Algoritmo ParImpar
	Escribir "Ingrese un numero"
	Leer num
	si num mod 2=0 Entonces
		Imprimir num, " Es un numero par"
	sino 
		Imprimir num, " Es un numero impar"
	FinSi
FinAlgoritmo
```


