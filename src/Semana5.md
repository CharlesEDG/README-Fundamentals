## Lunes:

### Exercise-1 Time Converter: Create a function called timeConverter that receives a positive number of seconds and returns a string based on the number. "Days: 1, Hours: 5, Minutes: 40 and seconds: 5"

4000 --> "days: 0, hours: 1, minutes: 6, and seconds: 4"

40000 --> "days: 0, hours: 11, minutes: 6, and seconds: 4"

150000 --> "days: 1, hours: 17, minutes: 40, and seconds: 0"

```python
Funcion result <- timeConverter (numero)
	Definir result Como Caracter;
	Definir dias, horas, minutos, seconds Como Entero;
	seconds = numero % 60;
	minutos = Trunc(numero/60) % 60;
	horas = Trunc(numero/3600) % 24;
	dias = Trunc(numero/86400);
	result = Concatenar('dias: ', ConvertirATexto(dias));
	result = Concatenar(result, ', horas: ');
	result = Concatenar(result, ConvertirATexto(horas));
	result = Concatenar(result, ', minutos: ');
	result = Concatenar(result, ConvertirATexto(minutos));
	result = Concatenar(result, ', and seconds: ');
	result = Concatenar(result, ConvertirATexto(seconds));
Fin Funcion

Algoritmo eTimeConverter
	Imprimir timeConverter(4000)
FinAlgoritmo
```



### Excerise-2 Compare distances: Create a function called compareDistances that asks for 5 numbers, these can be positive or negative, add the positives with positives and negatives with negatives, the function should return true if there is more distance to 0 with positives or false if the distance is greater with negatives .

4, 12 , 100, 8, -60 --> true

40, 120 , 10, -80, -91 --> false

```python
Funcion result <- compareDistances ()
	Definir result Como Logico;
	Definir numeroNegativo, numeroPositivo Como Real;
	numeroNegativo = 0;
	numeroPositivo = 0;
	Para contar=1 Hasta 5 Con Paso 1 Hacer
		Escribir "Ingrese un número"
		leer num
		SI num > 0 Entonces
			numeroPositivo = numeroPositivo + num;
		SiNo
			numeroNegativo = numeroNegativo + num;
		FinSi
	FinPara
	result = numeroPositivo > Abs(numeroNegativo)
Fin Funcion

Algoritmo eCompareDistances
	Imprimir compareDistances()
FinAlgoritmo
```



## Martes:

### Exercise-2 Sum of pairs: write a function called sumOfPairs that asks for a number from 1 to 100 indefinitely, if a negative number or greater than 100 is entered, it stops asking for more numbers and returns the sum of all the even numbers entered.

4, 12 , 100, 11, -60 --> 116

40, 121 --> 40

```python
Funcion result <- sumOfPairs ()
	Definir result Como Real;
	Definir suma Como Real;
	suma = 0;
	Repetir
		Escribir "Ingrese un numero entre 1 y 100"
		leer num
		SI  num < 1  | num > 100 Entonces
			Imprimir 'Numero inválido'
		SiNo
			SI num % 2 = 0
				suma = suma + num;
			FinSi
		FinSi
	Mientras Que num >= 1  & num  <= 100
	result = suma;
Fin Funcion

Algoritmo eSumOfPairs
	Imprimir sumOfPairs()
FinAlgoritmo
```



### Exercise-3 Mid point: write a function called midpoint that given 2 values (can be negative) does not return the value of the midpoint between them

-50,50 --> 0

40, 80 --> 60

```python
Funcion result <- midPoint (num1,num2)
	Si num1 > 0 Entonces
		Si num2 > 0 Entonces
			SI num1 > num2 Entonces
				result = num2 + ((num1 - num2) / 2); 
			SiNo
				result = num1 + ((num2 - num1) / 2);
			FinSi
		SiNo
			result = num1 - ( (num1 + Abs(num2))/2);
		FinSi
	SiNo
		SI num2 > 0 Entonces
			result = num1 + ( (num2 + Abs(num1))/2)	;
		SiNo
			SI Abs(num1) > Abs(num2) Entonces
				result = num1 + ((Abs(num1) - Abs(num2)) / 2); 
			SiNo
				result = num2 + ((Abs(num2) - Abs(num1)) / 2); 
			FinSi
		FinSi
	FinSi
	
Fin Funcion

Algoritmo eMidpPoint
	Imprimir midPoint(40,80)
	Imprimir midPoint(40,-80)
	Imprimir midPoint(50,50)
	Imprimir midPoint(-50,50)
FinAlgoritmo
```



## Miercoles:

### Exercise-1 Cashier: create a function called "cashier" that pretends to be a panel of a bank should display the text: "select an option: a. to deposit. b. withdraw. c. go out." and have a value called balance that will return when finished and will print it on the screen, its initial value will be 1000. You must repeat the menu until you select the option 'c'

if we select 'a' it invokes another function called 'deposit' that will display a text on the screen that will say 'how much do you want to deposit:' it will add that value to the balance and end the function.

if we select 'b' it invokes another function called 'withdraw' that will display a text on the screen that will say 'how much do you want to withdraw:' it will subtract that value from the balance and end the function.

"select an option: a. to deposit. b. withdraw. c. go out."

a -->

"how much do you want to deposit:"

500 -->

"select an option: a. to deposit. b. withdraw. c. go out."

b -->

"how much do you want to withdraw:"

1400 -->

"select an option: a. to deposit. b. withdraw. c. go out."

c -->

100

```python
Funcion balance <- cashier ()
	Definir balance Como Real;
	balance = 1000;
	Repetir
		Imprimir "Selecciona una opción:";
		Imprimir "a. depositar.";
		Imprimir "b. retirar.";
		Imprimir "c. salir.";
		leer option
		Si option = 'a' Entonces
			balance = balance + depositar()
		FinSi
		Si option = 'b' Entonces
			balance = balance - retirar()
		FinSi
	Mientras Que option = "a" | option = "b"
Fin Funcion

Funcion value <- depositar()
	Imprimir "Que cantidad quiere depositar:";
	leer value
FinFuncion

Funcion value <- retirar()
	Imprimir "Que cantidad quiere retirar:";
	leer value
FinFuncion

Algoritmo eCashier
	Imprimir cashier()
FinAlgoritmo
```



### Exercise-2 Weather average: write an algorithm that loops indefinitely until 'x' is entered which will calculate an average of the weather, note that for each value entered it should ask if it is fahrenheit or celsius, then ask for the value. add everything up and divide by the number of values entered. The result must be returned in celsius, have a function that, in case fahrenheit is entered, transforms it to celsius in order to add them.

```python
Funcion celsius <- fahrenheitaCelsius (fahrenheit)
	Definir celsius Como Real;
	celsius = (fahrenheit - 32 ) / 1.8
Fin Funcion

Algoritmo eWeatherAverage
	conteo = 0;
	total = 0;
	Repetir
		Imprimir "seleciona una opción:";
		Imprimir "a. ingrese grados celsius.";
		Imprimir "b. ingrese grados fahrenheit.";
		Imprimir "x. salir.";
		leer option
		Si option = "a" | option = "b" Entonces
			leer grado
			conteo = conteo + 1;
		FinSi
		Si option = 'a' Entonces
			total = total + grado;
		FinSi
		Si option = 'b' Entonces
			total = total + fahrenheitaCelsius(grado);
		FinSi
	Mientras Que option = "a" | option = "b"
	Imprimir total / conteo;
FinAlgoritmo
```



## Jueves:

### Exercise-1 If: Create an if statement with the JavaScript syntax

```JavaScript
if (10 < 5) {
    console.log ("Verdadero")

 } else {
    console.log("Falso")

}
```



### Exercise-2 While: Create a while loop statement with the JavaScript syntax

```JavaScript
let i = 1;

while (i <= 10) {
	console.log ("El valor del bucle es: " + i) ;
	i++;
}
```

