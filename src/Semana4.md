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
