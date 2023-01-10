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
