# Ejercicios de Algoritmos

## 1.  Hola Mundo

```
Algoritmo hola_mundo
	Escribir "Hola mundo"
FinAlgoritmo
```
Prueba de escritorio:

"Hola mundo"

## 2.  A partir de un número ingresado diga si es mayor, menor o igual a 9.

```
Algoritmo MayoresIgualesMenoresA9
	N<-0 // Variable inicial
	Escribir "Escribir el numero"
	Leer N
	Si N Es Igual A 9 Entonces
		Escribir "El numero es igual a 9"
	Sino
		Si N Es Mayor Que 9 Entonces
			Escribir "El numero es mayor a 9"
		Sino
			Escribir "El numero es menor a 9"
		Fin Si
	Fin Si
FinAlgoritmo
```
Prueba de escritorio:

Leer = Entrar

N: 5

Escribir: "El número es menor a 9"

## 3.  A partir de un número ingresado diga si el mismo es par o impar.

```
Algoritmo ParidadNumeros
	Leer nro
	Si (nro mod 2 // El resto de dividir nro entre 2) = 0 entonces
		Escribir "es par"
	Sino
		Escribir "es impar"
	Fin Si
FinAlgoritmo
```
Prueba de escritorio:
```
mod = resto división

nro: 7

Escribir: "es impar"
```

## 4.  ingresar dos números y devuelva el resultado de la suma entre ambos.

```
Algoritmo SumaDosNumeros
    Num1<-0
    Num2<-0
    Escribir "Escribir el numero 1"
    	Leer Num1
    Escribir "Escribir el numero 2"
    	Leer Num2
    	Rta<-Num1+Num2 // Asignar Num1+Num2 a Rta
    Escribir "El resultado es:" Rta
FinAlgoritmo
```

Prueba de escritorio:
```
Num1: 3

Num2: 4

Rta: 7

El resultado es: 7
```

## 5. Sumar todos los números pares entre 2 y 100.

```
Algoritmo SumaDePares
	suma <- 0
	nro <- 2
	Mientras nro<=100 hacer // "Mientras que" iniciar secuencia repetitiva (bucle)
		si nro mod 2 = 0 Entonces
			suma <- suma+nro			
		FinSi
		nro <- nro+1
	FinMientras
	Escribir "la suma de los pares entre nro y 100 es " suma
FinAlgoritmo
```

Prueba de escritorio:
```
suma: 2

nro: 3

Volver a "Mientras"
```

## 6. Ingresar un número y muestre todos los divisores del mismo.

```
Algoritmo divisores_de_numero
	Escribir "Ingrese Numero"
	Leer Num
	div<-1
	Mientras div<=Num Hacer // "Mientras div sea menor o igual que Num hacer" 
		Si Num MOD div = 0 // "si el resto de dividir Num y div es O entonces" 
			Escribir div
		Fin Si
		div<-div+1
	Fin Mientras
FinAlgoritmo
```

Prueba de escritorio:

Escribir:
```
Ingrese Numero
1 2 3
```
Num: 6

div: 2

Volver a "Mientras"

## 7. Determinar si un alumno aprueba o suspende un curso, sabiendo que aprobará si su promedio de tres calificaciones es mayor o igual a 4.0; supsende en caso contrario. Deberá permitir ingresar las tres calificaciones y luego calcular su promedio.

```
Algoritmo aprueba_reprueba
	Escribir "Ingrese calificacion 1"
		Leer Cal1
	Escribir "Ingrese calificacion 2"
		Leer Cal2
	Escribir "Ingrese calificacion 3"
		Leer Cal3
	Prom<-(Cal1+Cal2+Cal3)/3 // Prom asocia la operación que engloba las tres calificaciones y su media                       
        Si Prom>=4 Entonces
		Escribir "Aprueba"
	Sino
		Escribir "Suspende"
	Fin Si
	Escribir Prom
FinAlgoritmo
```

Prueba de escritorio:
````
"Ingrese calificacion 1"
7
"Ingrese calificacion 2"
8
"Ingrese calificacion 3"
10

"Aprueba"

8,3 -> [Prom: (7+8+10)/3]
````

## 8. Crear un algoritmo que permita ingresar un nombre y una cantidad numérica para escribir este nombre tantas veces como su cantidad ingresada.

```
Algoritmo Cantidad_nombre
	Escribir "Ingresar Nombre"
	Leer nombre
	Escribir "Ingresar Cantidad"
	Leer num
	Mientras Num>0 Hacer // No sensible a May/Min
		Escribir nombre
	Num<-Num - 1
	Fin Mientras
FinAlgoritmo
```

Prueba de escritorio:
````
"Ingresar nombre"
nombre<-"David"

"Ingresar cantidad"
N/num<-3,2,1,0

David
David
David
````

## 9. Sumar todos los números naturales comprendidos entre 1 y 50.

```
Algoritmo suma_numerosnaturales_1y50 
	Num<-1
	Resul<-0
	Repetir
	    Resul<-Resul+Num
	    Num<-Num+1 	                           
        Hasta Que Num>5 // El valor real es 50
	Escribir Resul
Fin algoritmo
```

Prueba de escritorio:
````
Num<-1
Resul<-0

2, 3, 4, 5, 6
1, 3, 6, 10, 15

15
````

## 10. Leer tres números; si el primero es negativo, debe imprimir la multiplicación de los tres y si no lo es, imprimirá la suma.

```
Algoritmo tresnumeros
	Escribir "Ingrese numero 1"
		Leer Num1
	Escribir "Ingrese numero 2"
		Leer Num2
	Escribir "Ingrese numero 3"
		Leer Num3
	Si Num1<0 Entonces
		Resul<-Num1 * Num2 * Num3
	Sino
		Resul<-Num1+Num2+Num3
	Fin Si
	Escribir Resul
FinAlgoritmo
```

Prueba de escritorio:
````
"Ingrese numero 1"
Num1<-2
"Ingrese numero 2"
Num2<-3
"Ingrese numero 3"
Num3<-4

Resul<-9
9
````

## 11. Si un número ingresado es primo o no. (Un número es primo si es divisible únicamente por 1 y por sí mismo).

```
Algoritmo NumerosPrimos
	Escribir "Ingrese un número: "
	Leer nro
	div <- 2
	band <- Verdadero 	         
        Si nro=1 Entonces 		            
             Escribir "Es primo" 	         
        Sino 		             
             Mientras band=Verdadero y nro>div Hacer
		Si nro MOD div = 0 Entonces
		    band <- Falso
		FinSi
		    div <- div +1
	     FinMientras
	     si band= Verdadero Entonces
		Escribir "Es primo"
	     Sino
		Escribir "No es primo"
	     FinSi
	FinSi
FinAlgoritmo
```

Prueba de escritorio:
````
"Ingrese un numero: "
nro<-5
div<-2, 3, 4, 5
band<-Verdadero

"Es primo"
````

## 12. Sumar los dígitos de un número ingresado. Ejemplo: Si se ingresa 123, debería devolver 6.

```
Algoritmo SumaDigitos
	Escribir "Ingrese un nro: "
	Leer nro
	resul <- 0
	Mientras nro <> 0 Hacer
		resul <- resul + nro MOD 10
		nro <- trunc(nro/10) // En este caso, trunc se refiere a coger solo la parte entera del resultado de la división (sin resto)
	FinMientras
	Escribir "El resultado es: " resul
FinAlgoritmo
```

Prueba de escritorio:
````
"Ingrese un nro: " // Coger prueba de escritorio de GitHub de Billy (22/04)

````

## 13. Ejercicios Propuestos
1. Calcular y mostrar el cuadrado de los números del 1 a 30.
2. Números primos
3. Construir un avión de papel
4. Realizar las cuatro operaciones básicas (Suma, Resta, Multiplicación, División)

```
    Algoritmo Calculadora
        Escribir "Inserte operacion: "
        Leer Num1
        Leer Op
        Leer Num2

        Si Op es igual '+' Entonces
            Escribir Num1 + Num2
        Otro si Op es igual '-'
            Escribir Num1 - Num2
        Otro si Op es igual '*'
            Escribir Num1 * Num2
        Sino
            Escribir Num1 / Num2
        FinSi
    FinAlgoritmo
```

5. Volumen y Area de un Cilindro

````
Algoritmo Cilindro
    pi<- 3.14
    Escribir "Ingrese el radio del cilindro"
    Leer r
    Escribir "Ingrese la altura del cilindro"
    Leer h

    area <- 2*(pi* r * r) + 2*(pi * r * h)
    volumen <-pi * r *r *h

    Escribir "El area del cilindro es:" + area
    Escribir "El volumen del cilindro es:" + volumen
FinAlgoritmo
````

6. Pedir un libro en una biblioteca
7. Encontrar el mayor número de tres números
8. Factorial de cualquier número
9. Encontrar si un numero en mayor o menor a un número dado.
10. Adivinar una palabra.