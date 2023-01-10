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
	Imprimir timeConverter(1500000)
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
