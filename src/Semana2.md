## Lunes

### Exercise-1: Logic Problem: The teacher asks his 5 students if they studied mathematics yesterday.

Alice: "Nobody studied math yesterday".  
Bob: "1 person studied math yesterday".  
Charlie: "2 people studied math yesterday".  
Dan: "3 people studied mathematics yesterday".  
Eva: "4 people studied mathematics yesterday".  

The teacher knows that only those who studied would be telling the truth and those who didn't would be lying. Who is telling the truth?

    Bob está diciendo la verdad ya que la respuesta de los demás no concuerda con que todos hayan estudiado
    
    
    
    
### Exercise-2: Cereal vrs Milk: Create an algorithm to prepare a bowl of cereal with milk. Represent the result in pseudocode and in a flowchart.

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



## Martes

### Exercise-2: Print my name: This will be a guided challenge, the idea is for you to use PSeInt. For this challenge, we will print your name on the screen, a simple task that will help us to review the way PSeInt works.

```python
Algoritmo MyName
	Imprimir "Charles Diaz"
FinAlgoritmo
```




### Exercise-3: Print my name & age: This challenge is similar to the previous guided challenge, but now you will try alone. For this challenge, you will need to create an algorithm in Pseudocode using PSeInt that prints your name and your age in separate lines, remeber that your name should be a string and your age a number

```python
Algoritmo MyNameAndAge
	Imprimir "Charles Diaz"
	Imprimir 30
FinAlgoritmo
```



## Miercoles

## Exercise-2: Mod: The challenge for you now is to create a PSeInt program that will receive a number from the user and add the mod operator using the even/odd case ( X % 2 ) where X is the user input.

```python
Algoritmo evenOdd
	Leer X
	Imprimir X % 2
FinAlgoritmo
```



## Exercise-3: Register form: You are given the task to create a registration form for new users, this form should ask the user for the following information:

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


