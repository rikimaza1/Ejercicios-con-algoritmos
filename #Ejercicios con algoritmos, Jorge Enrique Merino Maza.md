# Ejercicios con algoritmos

## Primeros 3 ejercicios 

### Ejercicio 1

*Calcular la letra del DNI Español* 

**Paso 1:** Definir el problema, a partir de un numero de DNI hemos de calcular la letra.

¿Como se calcula la letra del DNI?

Numero del DNI dividirlo entre 23 y el resto será el `resultadoResto`

El `resultadoResto` lo compararemos con la lista de códigos de la siguiente tabla de letras `tablaLetrasDni`

| resultadoResto | Letra |
| -------------- | ----- |
| 0              | T     |
| 1              | R     |
| 2              | W     |
| 3              | A     |
| 4              | G     |
| 5              | M     |
| 6              | Y     |
| 7              | F     |
| 8              | P     |
| 9              | D     |
| 10             | X     |
| 11             | B     |
| 12             | N     |
| 13             | J     |
| 14             | Z     |
| 15             | S     |
| 16             | Q     |
| 17             | V     |
| 18             | H     |
| 19             | L     |
| 20             | C     |
| 21             | K     |
| 22             | E     |

**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `DNI` , `tablaLetraDNI`, `resultado` = ""

Proceso: 

- Validar que el `DNI` tenga 8 dígitos, y que sean todos numéricos.
  - Si es errónea asignar a la variable resultado "DNI Invalido"

- Dividimos el `DNI` entre 23 y el resto lo asignamos a `resultadoResto`.
- Comparar el `resultadoResto` con los valores de la tabla, asignamos a `resultado` el valor equivalente en la tabla.

Salida:

- Escribir `resultado`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo calculoDNI
	# Entrada
	DNI <-leer()
	tablaLetrasDNI<-"TRWAGMYFPDXBNJZSQVHLCKE"
	resultado<-""
	# Proceso
	Si DNI es valido Entonces#
		resultadoResto<-DNI mod 23 #mod es el resto de dividir
		resultado<-recuperarLetra(resultadoResto,tablaLetrasDNI)
	Sino
		resultado<-"DNI Invalido"
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo

DNI: 333,36982589,

resultado:b,"S"

resultadoResto:15

tablaLetrasDNI:"TRWAGMYFPDXBNJZSQVHLCKE"

Salida: DNI Invalido, S

### Ejercicio 2
*Calcular el salario de un empleado* 

**Paso 1:** Definir el problema, a partir de un numero de DNI hemos de calcular la letra.

El salario en España se calcula a partir del salario bruto anual, que incluyen todas las percepciones económicas que recibe un trabajador durante el año, incluyendo salario base, pagas extras, complementos y otros conceptos retributivos.

Numero del DNI dividirlo entre 23 y el resto será el `resultadoResto`

El `resultadoResto` lo compararemos con la lista de códigos de la siguiente tabla de letras `tablaLetrasDni`

**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `salarioBase` , `pagasExtra`, `complementos` , `otrosConceptosRetributivos` ,`IRPF`, `seguridadSocial`

Proceso:  

- Sumar `salarioBase` , `pagasExtra`, `complementos` , `otrosConceptosRetributivos` y lo asigno a `salarioBruto`.

- Sumar `IRPF`, `seguridadSocial` y lo asigno a `deduciones`
  
- `salarioNeto  ` asigna `salarioBruto`- `deduciones`

Salida:

- Escribir `(salarioBruto,salarioNeto)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo calculoDNI
	# Entrada
	salarioBase <-leer()
	pagasExtra <-leer()
	complementos <-leer()
	otrosConceptosRetributivos <-leer()
	IRPF <-leer()
	seguridadSocial <-leer()
	# Proceso
	salarioBruto <- salarioBase+pagasExtra+complementos+otrosConceptosRetributivos
	deduciones <- IRPF+seguridadSocial
	salarioNeto<- salarioBruto - deduciones
	# Salida
	Escribir (salarioBruto,deduciones)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 3(falta)
*Determinar la ruta para llegar a una ciudad por avión.* 

**Paso 1:** Definir el problema, a partir de un numero de DNI hemos de calcular la letra.

El salario en España se calcula a partir del salario bruto anual, que incluyen todas las percepciones economicas que recibe un trabajador durante el año, incluyendo salario base, pagas extras, complementos y otros conceptos retribitivos.

Numero del DNI dividirlo entre 23 y el resto será el `resultadoResto`

El `resultadoResto` lo compararemos con la lista de códigos de la siguiente tabla de letras `tablaLetrasDni`


**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `salarioBase` , `pagasExtra`, `complementos` , `otrosConceptosRetributivos` ,`IRPF`, `seguridadSocial`

Proceso:  

- Sumar `salarioBase` , `pagasExtra`, `complementos` , `otrosConceptosRetributivos` y lo asigno a `salarioBruto`.

- Sumar `IRPF`, `seguridadSocial` y lo asigno a `deduciones`
  
- `salarioNeto  ` asigna `salarioBruto`- `deduciones`

Salida:

- Escribir `(salarioBruto,salarioNeto)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo calculoDNI
	# Entrada
	salarioBase <-leer()
	pagasExtra <-leer()
	complementos <-leer()
	otrosConceptosRetributivos <-leer()
	IRPF <-leer()
	seguridadSocial <-leer()
	# Proceso
	salarioBruto <- salarioBase+pagasExtra+complementos+otrosConceptosRetributivos
	deduciones <- IRPF+seguridadSocial
	salarioNeto<- salarioBruto - deduciones
	# Salida
	Escribir (salarioBruto,deduciones)
Fin Algoritmo
```

## Prueba del algoritmo

## Siguientes 7 ejercicios

### Ejercicio 4
*Calcula el área y perímetro de un círculo dado su radio* 

**Paso 1:** Definir el problema, a partir del radio de un circulo calcular área y perímetro.

El área de un circulo se calcula de la siguiente manera: **π r²**

El perímetro de un circulo se calcula de la siguiente manera: **2 π  r**



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `radio` 

Proceso:  

- Multiplicar π `radio`² y lo asigno a `area`.
- Multiplicar 2 π `radio` y lo asigno a `perimetro`.

Salida:

- Escribir `(area,perimetro)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo areaPerimetroCirculo
	# Entrada
	radio <-leer()
	# Proceso
	area <- π radio² 
	perimetro <- 2 π radio
	# Salida
	Escribir (area,perimetro)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 5
*Dada una lista de números enteros, determina cuál es el mayor y cuál es el menor.* 

**Paso 1:** Definir el problema, a partir de una lista de numero determinar el mayor y menor.

En primer lugar asignaremos el primero numero de la lista a `mayor` y `menor`, y recorreremos la lista comparando y asignando valores a estas variables.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeros[]` 

Proceso:  

- Asignamos a `mayor` y `menor` el valor de `numeros[0]`
- iteramos para recorrer y comprobar la lista de números comprobando si `numero[i]` es mayor que `mayor`  o menor que `menor`

Salida:

- Escribir `(menor,mayor)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo mayorMenor
	# Entrada
	numeros[] <-leer()
	mayor <- numeros[0]
	menor <- numeros[0]
	Escribir "Cantidad de numeros de la lista"
	cantidad <-leer()
	numeros[cantidad]
	Para i<-0 hasta i<=cantidad Hacer
		Ecribir "Ingrese numero "+i
		numeros[i]<-leer()
	FinPara	
	# Proceso
	
	Para i <-1 hasta i<=numeros[fin] paso 1 hacer
	Si numeros[i] < menor Entoces 
		menor <- numeros[i]
	FinSi
	Si numeros[i] > mayor Entoces 
		mayor <- numeros[i]
	FinSi
	
	# Salida
	Escribir (mayor,menor)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 6
*Crea un algoritmo que convierta grados Celsius a Fahrenheit.* 

**Paso 1:** Definir el problema, pasar de grados Celsius a Fahrenheit.

Para pasar de Celsius a Fahrenheit se usa la siguiente formula **ºF = ºC x 1.8 + 32**



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `gradosCelsius` 

Proceso:  

- Multiplicar `gradosCelsius` **x**1.8**+**32 y lo asigno a `gradosFahrenheit`.

Salida:

- Escribir `(gradosFahrenheit)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo celsiusFahrenheit
	# Entrada
	gradosCelsius <-leer()
	# Proceso
	gradosFahrenheit <- gradosCelsius 1.8 + 32
	# Salida
	Escribir (gradosFahrenheit)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 7
*Dado un número entero, crea un algoritmo que determine si es par o impar.* 

**Paso 1:** Definir el problema, determinar si un numero entero es par o impar.

Un numero entero es par si el resto de la división entre 2 es 0.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeroEntero` 

Proceso:  

- modulo de `numeroEntero`% 2  y lo asigno a `resto`.
- comparar resto con 0

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo numeroParImpar
	# Entrada
	numeroEntero <-leer()
	# Proceso
	resto <- numeroEntero % 2
	Si resto == 0
		resultado = "Es par"
    Sino
   		resultado = "Es impar"
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 8

*Crea un algoritmo que determine si un año es bisiesto o no.* 

**Paso 1:** Definir el problema, determinar si un año es bisiesto o no

Un año bisiesto es si es divisible entre 4, 100 y 400



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `anyo` 

Proceso:  

- modulo de `numeroEntero`%4   y lo asigno a `resto`.
- comparar resto con 0
- modulo de `numeroEntero`%100   y lo asigno a `resto`.
- comparar resto con 0
- modulo de `numeroEntero`%400   y lo asigno a `resto`.
- comparar resto con 0

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo bisiesto 
	# Entrada
	anyo <-leer()
	# Proceso
	resto <- numeroEntero % 4
	Si resto == 0
		resto <- numeroEntero % 100
			Si resto == 0
				resto <- numeroEntero % 400
					Si resto == 0
						resultado = "Es bisiesto"
    Sino
   		resultado = "No es bisiesto"
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 9
*Crea un algoritmo que determine si una cadena de texto es un palíndromo o no.* 

**Paso 1:** Definir el problema.

Debemos determinar si  una cadena de texto es palíndromo o no, es palíndromo cuando una palabra o cadena de texto se lee igual tanto como de izquierda y de derecha.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `cadena` 

Proceso:  

- En primer lugar, le quitaremos los espacio a `cadena` asignando el valor a `cadenaSinEspacios`  , acto seguido con el uso de la función `minusculas` convertimos a todo carácter de la cadena en minúscula asignando el resultado a `cadenaSinEspacios`.
- Definiremos un booleano `palindromo = true`, con la iteración `Para ` recorremos la cadena evaluando si las palabras del inicio coinciden con las del final.
- Evaluando el booleano `palindromo` asignaremos a `resultado` un valor

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo palindromo
	# Entrada
	cadena <-leer()
	# Proceso
		#Quitamos espacion de la cadena
            Para i<-0 hasta i<-longitud(cadena) hacer
            	Si subcadena(cadena,i,i) distinto " " entonces
            		cadenaSinEspacios<-cadenaSinEspacios+subcadena(cadena1,i,i)
            	Finsi
            Fin Para
        #Todo a minusculas
            cadenaSinEspacios <- minusculas(cadenaSinEspacios)
        #comprobados si se leen igual de iquierada a derecha
        palindromo = true
        	Para i<-0 hasta i<-longitud(cadena) hacer
            	Si subcadena(cadenaSinEspacios,i,i) distinto subcadena(cadenaSinEspacios,i,i) entonces
            		palindromo = false
           		Finsi
            Fin Para
        #Asignamos a resultado un valor
        Si palindromo entonces
        	resultado = "Es palindromo"
        Sino
        	resultado = "No es palindromo"
        Finsi
	
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo

### Ejercicio 10
*Dada una lista de nombres, crea un algoritmo que ordene la lista alfabéticamente.* 

**Paso 1:** Definir el problema, determinar si un año es bisiesto o no

Diversos lenguajes tienen funciones para ordenar una lista, sin embargo al tratarse de un pseudo código, una forma de ordenando seria compara con menor que o mayor que ya que los caracteres o palabras se pasas a código ASCII o a binario.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `listaNombres[]` 

Proceso:  

- Utilizaremos la iteración `Para` y dentro de este asignaremos a la variable `min` el valor del primer elemento, usaremos una iteración `para ` anidado en el anterior, dentro de este evaluaremos si es mayor o no, si lo es asignaremos a `min` el valor de `j`.
- Después de la iteración anidada `para` usaremos una variable `aux ` para ordenar el array e intercambiar valores en la posiciones

Salida:

- Usaremos iteración `para `para escribir los valores del array ordenado.

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo ordenarLista
	# Entrada
	listaNombres[] <-leer()
	# Proceso
	Para i <- 1 hasta 5 con paso 1 Hacer
		min <- i
		Para j<-i+1 Hasta 5 Con Paso 1 Hacer
			Si a[j] < a[min] Entonces  //con < ordena ascendente, con > ordena descendente
				min <- j
			Fin Si
		FinPara
		aux <- a[i]
		a[i] <- a[min]
		a[min] <- aux
	FinPara
	# Salida
	Escribir "La lista ordena es:"
	para i <- 1 hasta 5 con paso 1 Hacer	
		Escribir a[i] " "
	FinPara
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 11
*Crea un algoritmo que calcule el factorial de un número entero.* 

**Paso 1:** Definir el problema, determinar el factorial de un numero.

El factorial se obtiene mediante la multiplicación de cada uno de los números positivos comenzando desde el uno hasta el numero dado. 



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeroEntero` 

Proceso:  

- Calcularemos el factorial del numero dado mediante el uso de una iteración desde el 1 hasta el `numeroEntero` dado 

Salida:

- Escribir `(factoria)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo factorial
	# Entrada
	resultado<-1
	numeroEntero <-leer()
	# Proceso
	Para i<-1 hasta i<=numeroEntero Paso 1 hacer
	resultado=resultado*i
	FinPara
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 12
*Dado un número entero, crea un algoritmo que determine si es primo o no.* 

**Paso 1:** Definir el problema, determinar si un numero es primo o no

Un numero es primo si únicamente es divisible entre si mismo o 1.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeroEntero` 

Proceso:  

- Modular recursivamente `numeroEntero` siendo divisores del 1 hasta `numeroEntero`

- Contabilizar la los resultados del mod sean igual a 0 en `divisiones`

- Evaluar si divisiones es igual a 2 (primo) o no

  

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo numeroPrimo
	# Entrada
	numeroEntero <-leer()
	contador<-0
	# Proceso
	Para i <- hasta i <= numeroEntero paso 1 hacer
		Si num%i == 0 entonces
			contador<-contador+1
			
		FinSi
	FinPara
	Si contador == 2 entonce
		resultado<-"Es primo"
	Sino 
    	resultado<-"NO es primo"
    FinSi
    
	# Salida
	
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 13
*Crea un algoritmo que calcule el área y volumen de un cubo dado su lado.* 

**Paso 1:** Definir el problema, calcular área y volumen de un cubo mediante su lado.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `ladoCubo` 

Proceso:  

- Calculamos el área del cubo mediante la siguiente formula `6*ladoCubo*ladocubo` y se lo asignamos a `area`.
- Calculamos el volumen del cubo mediante la siguiente formula `ladoCubo*ladoCubo*ladocubo` y se lo asignamos a `volumen`.

Salida:

- Escribir `(area,volumen)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo areaVolumenCubo
	# Entrada
	ladoCubo <-leer()
	# Proceso
	area <-6*ladoCubo*ladoCubo
	volumen <-ladoCubo*ladoCubo*ladoCubo
	Escribir (area,volumen)
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 14
*Dada una lista de números enteros, crea un algoritmo que calcule la suma de todos los números  pares de la lista.*

**Paso 1:** Definir el problema, calcular los números pares de una lista.

Un numero par es el numero que al realizar el modulo entre 2 el resultado es 0,



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeros[]` ,`cantidad`

Proceso:  

- Pediremos por pantalla cuantos números quiere introducir, asignando a `cantidad`
- Mediante una iteración **para** para ir pidiendo y asignando los valores de la lista `numeros[]`
- Con otra iteración iremos evaluando cada elemento de la lista si es par la asignaremos dicho valor a `suma`

- Escribir `(suma)`

Salida:

- Escribir `(suma)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo sumaPares
	# Entrada
	Escribir "Cantidad de numeros de la lista"
	cantidad <-leer()
	numeros[cantidad] #Definimos una lista de numeros del valor de cantidad leida
	
	Para i<-0 hasta i<=cantidad Hacer
		Ecribir "Ingrese numero "+i
		numeros[i]<-leer()
	FinPara		
	# Proceso
	suma <-0
	Para i<-0 hasta i<=cantidad Hacer
		Si numeros[i] mod 2 es Igual 0 entonces
			suma <- suma + numeros[i]
		FinSi	
	FinPara	
	# Salida
	Escribir (suma)
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 15
*Crea un algoritmo que determine si un número es positivo, negativo o cero.* 

**Paso 1:** Definir el problema, si un número es positivo, negativo o cero.

Un numero es positivo si es mayor que 0, un numero es negativo si es menor que cero, y un numero es cero si equivale a cero.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numero` 

Proceso:  

- compara numero si es mayor a 0, menor a 0, o es cero

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo positivoNegativoCero
	# Entrada
	numero <-leer()
	# Proceso
	resultado <- ""
	Si numero > 0 Entonces
		resultado <- "Es positivo"
	Sino
		Si numero < 0 Entonces
			resultado <- "Es negativo"
		Si no
        	resultado <- "Es cero"
        FinSi
    Finsi    
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 16
*Dada una lista de números enteros, crea un algoritmo que calcule la media de la lista.* 

**Paso 1:** Definir el problema, calcular la media aritmética de una lista de números.

La media aritmética se obtiene mediante la suma de todos sus numero y la división de la cantidad de numero que haya.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeros[]` .`cantidad`

Proceso:  

- Pediremos por pantalla cuantos números quiere introducir, asignando a `cantidad`
- Mediante una iteración **para** para ir pidiendo y asignando los valores de la lista `numeros[]`
- Con otra iteración iremos sumando cada elemento de la lista y asignaremos dicho valor a `suma`
- Asignaremos a `media` el valor de la suma total de los números de la lista y la división de la cantidad de elementos.

- Escribir `(media)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo mediaAritmetica
	# Entrada
	Escribir "Cantidad de numeros de la lista"
	cantidad <-leer()
	numeros[cantidad]
	Para i<-0 hasta i<=cantidad Hacer
		Ecribir "Ingrese numero "+i
		numeros[i]<-leer()
	FinPara		
	# Proceso
	suma <-0
	Para i<-0 hasta i<=cantidad Hacer
		suma <- suma + numeros[i]
	FinPara	
	media<- suma/cantidad
	# Salida
	Escribir (media)
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 17
*Crea un algoritmo que genere un número aleatorio entre 1 y 100, y le pida al usuario adivinarlo. El  algoritmo deberá indicar si el número introducido es mayor o menor que el número aleatorio, hasta  que el usuario adivine el número correcto.* 

**Paso 1:** Definir el problema, obtener un numero azar entre 1 y 100, y luego pedir al usuario valores para adivinar.

Para dar un numero aleatorio usaremos una función random en este caso `AZAR()`



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numero` ,`adivinado`=falso

Proceso:  

- En primer lugar asignaremos a `aleatorio` el numero obtenido por `AZAR()`
- Mediante una iteración mientras, iremos pidiendo un `numero` y lo evaluaremos con `aleatorio` diciendo si es mayor o menor que el aleatorio. 

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo adivinarNumero
	# Entrada
	 aleatorio <- AZAR(1,100)
	# Proceso
	Mientras adivinado == falso Hacer
		Escribir "Adivina el numero"
		numero <- leer
		Si numero == aleatorion entonces 
			resultado = "Has adivinado, bravo!"
			adivinado <- verdadero
		Sino
			Si numero > aleatorio entonces
				resultado = "El numero introducido es mayor"
			Sino 
				resultado = "El numero introducido es menor"
		FinSi
    
	FinMientras
	# Salida
	Escribir (resultado)
Fin Algoritmo

```

## Prueba del algoritmo
### Ejercicio 18
*Crea un algoritmo que determine si una cadena de texto es un anagrama de otra cadena de texto.* 

**Paso 1:** Definir el problema.

Tendremos dos cadenas de texto y deberemos determinar si son anagramas o no, dos cadenas son anagramas cuando tienen la misma cantidad de le tras del mismo tipo pero de diferente distribución.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `cadena1`, `cadena2`.

Proceso:  

- En primer lugar ambas cadenas pasaran por un proceso mediante el uso de la iteración `Para`  en la que eliminaremos los espacios de ambas cadenas asignado el nuevo valor a `cadena1Procesada` y `cadena2Procesada`.
- mediante la función `minusculas ()` cada elemento de ambas cadenas se pasaran a ser minúsculas y volveremos a reasignar el valor a `cadena1Procesada` y `cadena2Procesada`.
- Definiremos el Abecedario en una cadena `abecedario`
- En este proceso mediante el uso de `abecedario` y el uso de la iteración `Para` ordenaremos ambas cadenas asignado el nuevo valor a `cadenaProcesadaOrdenada1` y `cadenaProcesadaOrdenada2`.
- Mediante el uso de un condicional evaluaremos si ambas cadenas tienen la misma longitud si no la tienen el programa asignara que no es una anagrama a `resultado` y acabara el programa, pero si tienen el mismo numero continuara el programa y acabara en una iteración `Para` que comprobara cada índice de ambas palabra si son iguales si no lo es asignara a el booleano `anagrama` el valor de falso y se evaluara por ultimo este booleano para asignar a resultado un mensaje de si es o no anagrama

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo anagrama
	# Entrada
	cadena1 <- leer()
	cadena2 <- leer()
	# Proceso
	cadena1Procesada=""
	cadena2Procesada=""
	# Eliminando los espacios de ambas cadenas
	Para i<-0 hasta i<-longitud(cadena1) hacer
	Si subcadena(cadena1,i,i) distinto " " entonces
	cadena1Procesada<-cadena1Procesada+subcadena(cadena1,i,i+1)
	Finsi
	Fin Para
	Para i<-0 hasta i<-longitud(cadena2) hacer
	Si subcadena(cadena,i,i) distinto " " entonces
	cadena2Procesada<-cadena2Procesada+subcadena(cadena2,i,i+1)
	Finsi
	Fin Para
	# usamos la funcion minusculas para dejar ambas cadenas unicamente con misnusculas
	cadena1Procesada <- minusculas(cadena1Procesada)
	cadena2Procesada <- minusculas(cadena2Procesada)
	#definimos el abecedario en una cadena
	abecedario <- "abcdefghijklmnñopqrstuvwxyz"
	#ordenamos ambas cadenas y nos ayudamos de otra variable para guardar el resultado
	cadenaProcesadaOrdenada1 <- ""
	cadenaProcesadaOrdenada2 <- ""
	Para i<-0 hasta i<-longitud(abecedario) hacer
		Para j<-0 hasta i<-longitud(cadena1Procesada) hacer
			Si subcadena(abecedario,i,i) es igual  subcadena(cadena1Procesada,i,i) entonces
			cadenaProcesadaOrdenada1 <- cadenaProcesadaOrdenada1+subcadena(cadena1Procesada,i,i)
			SiFin
		FinPara
	Fin Para
	Para i<-0 hasta i<-longitud(abecedario) hacer
		Para j<-0 hasta i<-longitud(cadena2Procesada) hacer
			Si subcadena(abecedario,i,i) es igual  subcadena(cadena2Procesada,i,i) entonces
			cadenaProcesadaOrdenada2 <- cadenaProcesadaOrdenada2+subcadena(cadena2Procesada,i,i)
			SiFin
		FinPara
	Fin Para
	#Por ultimo comprobaremos si ambas cadenas son iguales si cada uno de los indeces coinciden es anagrama.
	resultado<-""
	Si longitud(cadenaProcesadaOrdenada1) es distinto  longitud(cadenaProcesadaOrdenada2) entonces
		resultado <- "No es anagrama"
	Sino
		anagrama = true
		Para j<-0 hasta i<-longitud(cadena2Procesada) hacer
			Si subcadena(cadenaProcesadaOrdenada1,i,i) es distinto  subcadena(cadenaProcesadaOrdenada2,i,i) entonces
			anagrama <- false
			SiFin
		FinPara
		Si anagrama entonces
		 resultado <- "Es anagrama"
		Sino
			resultado <- "No es anagrama"
        FinSi
	FinSi
	
	
	# Salida
	Escribir (resultado)
Fin Algoritmo

```

## Prueba del algoritmo
### Ejercicio 19
*Dada una lista de números enteros, crea un algoritmo que elimine los números duplicados de la  lista* 

**Paso 1:** Definir el problema, eliminar numero duplicados de una lista.

Para comprobar si un numero esta repetido o no deberemos de usar una lista auxiliar para poder modificar el array original.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numeros[]` ,`Cantidad`

Proceso:  

- Declararemos un array auxiliar para poder realizar el proceso `auxiliar[]`, también inicializaremos una variable a 0 `j`   
- Usando una iteración `Para` y con una evaluación comprobaremos si el valor a continuación es distinto que  si se da el caso asignaremos a auxiliar el valor del array `numeros` en la posición i
- Almacenaremos el ultimo el ultimo elemento en el auxiliar[]
- Usaremos `para` para modificar el array `numeros`.

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo arraySinRepetidos
	# Entrada
	Escribir "Cantidad de numeros de la lista"
	cantidad <-leer()
	numeros[cantidad]
	Para i<-0 hasta i<=cantidad Hacer
		Ecribir "Ingrese numero "+i
		numeros[i]<-leer()
	FinPara	
	# Proceso
	auxiliar[cantidad]
	j <- 0
	Para i <- 0 hasta i < cantidad-1 con paso 1 Hacer
    	Si numeros[i] es distinto numeros[i+1] Entonces
			auxiliar[j++] <- numeros[i]
		Fin Si
	FinPara
	auxiliar[j++] = numeros[cantidad-1]
	auxiliar[cantidad]
	Para i <- 0 hasta i < j con paso 1 Hacer
    	numeros[i] <- auxiliar[i]
	FinPara
	# Salida
	Para i <- 0 hasta i < numeros[].lenght con paso 1 Hacer
    	Escribir numeros[i]+" "
	FinPara
Fin Algoritmo
```

## Prueba del algoritmo
### Ejercicio 20
*Crea un algoritmo que determine si un número es capicúa o no.* 

**Paso 1:** Definir el problema, determinar si un numero es capicúa o no.

Un numero capicúa es un numero que se lee igual de izquierda o derecha, los numero de 0 a 9 son capicúas.



**Paso 2:** Poner la entrada, el proceso y la salida.

Entrada: `numero` 

Proceso:  

- En primer lugar comprobaremos si `numero` esta en el rango de 0 a 9 

- Para comprobar si un numero mayor a 9 es capicúa tendremos que invertirlo para ello usaremos una iteración mientras para realizar la operación donde mediante la ayuda de `axuliar ` y `auxiliar2` nos ayudaremos a mantener los valores y darle la vuelta al numero.

  

Salida:

- Escribir `(resultado)`

**Paso 3:** Escribir el Seudocódigo

```
Algoritmo numeroCapicua
	# Entrada
	numero <- leer()
	auxiliar <- numero
	auxiliar2 <- 0
	numeroInvertido <- 0
	resultado <- 0
	# Proceso
	Si numero >=0 Y numero <=9  Entonces
        resultado <- "Es Capicua"
	Sino 
		Mientras aux != 0 Hacer
			auxiliar2 <- auxiliar mod 10
			numeroInvertido <- numeroInvertido * 10 + auxiliar2
			auxiliar <- trunc(auxiliar/10)
		FinMientras
		Si numero == numeroInvertido Entonces
        	resultado <- "Es Capicua"
		Sino 
			resultado <- "No es Capicua"
		Finsi
	Finsi
	# Salida
	Escribir (resultado)
Fin Algoritmo
```

## Prueba del algoritmo

