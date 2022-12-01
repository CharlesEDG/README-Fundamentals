## Miercoles

### Exercise-1 Pizza: Design an algorithm to prepare a pizza from scratch. Define the ingredients, what will be the flavor and the preparation.
# Algoritmo preparación de una pizza de pepperoni

#### Elementos de entrada:

* Masa plana
* Bandeja
* Queso
* Rebanadas de Pepperoni 
* Salsa de Tomate 
* Horno

#### Proceso:

### Inicio
* Tomar la masa
* Colocar la masa sobre la bandeja
* Pre-calentar el horno
* Comenzar a colocar la salsa de tomate hasta que quede totalmente cubierta
* Comenzar a colocar el queso sobre la masa hasta cubrir la superficie con salsa
* Colocar rebanadas de Pepperoni hasta cubrir la superficie del queso
* Llevar la bandeja con la pizza hacia el horno
* Colocar con mucho cuidado la pizza en el horno
* Esperar tiempo suficiente hasta que la pizza esté perfectamente horneada
* Revisar que la pizza esté perfectamente horneada
* Apagar el horno y esperar hasta que se enfríe un poco
* Sujetar la bandeja con la pizza con mucho cuidado y comenzar a sacar la pizza
* Colocar en un lugar seguro
* Esperar que se enfríe la pizza
* Empezar a cortar la pizza hasta alcanzar las rebanadas optimas
* Servir las rebanadas de pizza
* Comenzar a degustar la pizza
### Fin





### Exercise-2 Hot N Cold: Define an algorithm that is able to convert temperatures from Celsius to Fahrenheit and vice versa.

### Inicio
* Tomar en cuenta la formula para cambiar de Celsius a fahrenheit 
* Toma la cantidad de Celsius y aplica la formula "F = (C * 1.8) + 32"
* Guardar los resultados de la cantidad de Fahrenheit
### Fin

### Inicio
* Tomar en cuenta la formula para cambiar de Fahrenheit a Celsius
* Tomar la cantidad de Fahrenheit y aplicar la formula "C = (F - 32) * 0.5556
* Guardar los resultados de la cantidad de Celsius
### Fin




### Exercise-3 Geometry: Design an algorithm to calculate the volume of a pyramid, a cube and a sphere

### Inicio
* Investigar la formula de cada figura
* Elegir una figura ( Piramide, Cubo, Esfera )
* Aplicar la formula para calcular el volúmen de la figura ( Piramide ) V = AB * H / 3
* Guardar resultados
* Aplicar la formula para calcular el volúmen de la figura ( Cubo ) V = L * L * L = L ^ 3
* Guardar resultados
* Aplicar la formula para calcular el volúmen de la figura ( Esfera ) V = 4 / 3 * pi * r ^ 3
* Guardar resultados
### Fin




## Jueves

### Exercise-1 Numbers: Design an algorithm to check if a number is even or odd. If it is even, write that it is even, otherwise write that it is odd. Represent the algorithm in a flowchart.

![image](https://aprendeitonline.com/wp-content/uploads/2019/10/test.par_.impar_.png)




### Exercise-2 Date of birth: Write pseudocode for an algorithm that calculates the age of a person based on date of birth

```
Algoritmo EdadActual
	Definir edad, diaActual, mesActual, añoActual Como Entero
	Definir diaNacimiento, mesNacimiento, añoNacimiento Como Entero
	Escribir "Dame la fecha actual, en día, mes y año" 
	Leer diaActual, mesActual, añoActual	
	Escribir "Dame la fecha de nacimiento en día, mes y año"
	Leer diaNacimiento, mesNacimiento, añoNacimiento
	edad = añoActual - añoNacimiento
	si mesNacimiento > mesActual Entonces
		edad = edad - 1
	SiNo
		si mesNacimiento == mesActual Entonces
			si diaNacimiento > diaActual Entonces
				edad = edad - 1
			FinSi
			
		FinSi
		si diaNacimiento == diaActual Entonces
			Escribir "Felicidades estas cumpliendo años"
		FinSi
	FinSi
	Escribir "Tu edad actual es: ", edad," años"
FinAlgoritmo
```




### Exercise-3 Treasures: We are in a room with three chests. We know that at least one has a treasure in it. Each chest has a message, but all the messages are lies.

Left chest: The middle chest has a treasure
Middle chest: All these chests have treasures in them
Right chest: Only one of these chests has treasures.

Which chests have treasures?

Tomando en cuenta que el de la izquierda dice que el del medio tiene un tesoro sabemos que es mentira, el del medio dice que todos tienen un tesoro y el de la derecha dice que sólo uno tiene un tesoro, ya que todas las respuestas son mentira significa que hay dos cofres con tesoro. Entonces quiere decir que los que tienen un tesoro son el A y el C
