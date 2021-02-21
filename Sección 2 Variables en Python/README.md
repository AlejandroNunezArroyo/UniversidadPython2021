# Sección 2: Variables en Python

## 6. Declaración de Variables en Python

Una variable es la información que vamos a guardar en nuestro equipo, en python no es necesario identificar el tipo de variable (Entero, flotante, bool, etc).

**Comandos importantes:**

`=`→ Nos sirve para asignar valores

Cada variable en nuestro programa hace referencia a un valor en específico en la memoria de nuestra computadora. 

```python
a = 10 # Crea una variable de nombre "a" con valor de "10" 
b = 2 # Crea una variable de nombre "b" con valor de "2" 
```

No solamente se utilizan letras, si no también palabras completas sin espacios. 

```python
primer_numero = 10 # Crea una variable de nombre "primer_numero" con valor de "10" 
segundo_numero = 2 # Crea una variable de nombre "segundo_numero " con valor de "2" 
```

> Desafío: Cree un programa que cumpla los siguiente requerimientos

Realizar la adición de todos los números y almacenarlos en una variable llamada: `total`

Posteriormente utilizar la función `print(total)` para mostrar el resultado.

```python
a = 1
b = 2 
c = 3
d = 4
```

Realizar la adición, resta, multiplicación y división de las variables `a,b` y almacenarlos en una variable llamada: `total`

Posteriormente utilizar la función `print(total)` para mostrar el resultado de cada operación. 

NOTA: Se recomienda primero hacer una operación, mostrar el resultado y luego seguir con la siguiente operación. 

```python
a = 8
b = 2
# Ejemplo de la división
total = 8/2
print(total)
```

## 8. Tipos de Datos Básicos en Python

Variable tipo entera → 10, 20 ,3 , 14, cualquier número entero

Variable tipo flotante → 1.3, 13.13, 123.1231, cualquier número con decimal

Variable tipo booleana → False o True, solo esos dos valores (Falso o Verdadero) la primera letra debe ser mayúscula. 

> Desafío

Deberá utilizar la función `type()` (la cual sirve para saber que tipo de dato es nuestra variable) para comprobar el tipo de dato de los siguientes números. 

```python
# Copiar el siguiente código y comprobar que es el mismo tipo de dato
a = 10 # Esta variable es entera
print(type(a)) # El tipo de dato deberá ser una entera
b = 9.13 # Esta variable es flotante
print(type(a)) # El tipo de dato deberá ser una flotante
c = False # Esta variable es booleana 
print(type(a)) # El tipo de dato deberá ser una booleana
```

## 9. Tipos Numéricos en Python

Variable tipo entera → 10, 20 ,3 , 14, cualquier número entero

Variable tipo flotante → 1.3, 13.13, 123.1231, cualquier número con decimal

> Desafío

Ejecutar el siguiente programa:

```python
numero_uno = 10
numero_dos = 20
resultado = numero_uno + numero_dos
print(resultado)
print(type(resultado))

numero_uno = 10.0
numero_dos = 20.0
resultado = numero_uno + numero_dos
print(resultado)
print(type(resultado))

numero_uno = 10.0
numero_dos = 20
resultado = numero_uno + numero_dos
print(resultado)
print(type(resultado))
```

Pensar: ¿Por qué el valor de `resultado` es una variable tipo flotante cuando se suma un número entero y un número flotante?

## 10. Tipos String (Cadena) en Python

Variable de tipo cadena → "Cualquier nombre o texto en una oración"

Concatenación: Es la union de dos strings o dos cadenas de texto

```python
cadena = "Alejandro "
print("Hola, mi nombre es: " + cadena)
```

Recordar que solamente estamos trabajando con la parte literal de las palabras, si intentamos hacer alguna operación matemática solo unirá ambas cadenas.

```python
numero_uno = "1"
numero_dos = "2"
resultado = numero_uno + numero_dos
print(resultado)
```

```python
RESULTADO: 12
```

> Desafío

Debe utilizar la función `print()` y concatenación para mostrar la siguiente información:

```python
Hola, mi nombre es: Alejandro
Tengo 20 años
Soy de Bolivia
```

Los siguiente datos son variables, deberá concatenar los datos para obtener un mensaje similar al anterior paso. 

```python
nombre = "Alejandro"
edad = "20 años"
pais = "Bolivia"
```

## 11. Tipo Bool (Verdadero o Falso) en Python

Solo tiene dos estado lógicos, verdadero o falso. 

```python
variable = True
variable = False
```

NOTA: Una función que nos permite hacer la "lógica de si un suceso pasa" es la función `if`, la estructura es la siguiente. 

```python
if (accion es verdadera):
	Se hace esta línea de código
else:
	Se hace esta línea de código
```

Ejemplo: Si tenemos dos variables y comparamos cual de ellas es mayor el código sería de la siguiente forma.

```python
numero_uno = 13
numero_dos = 8
# Código para saber cual número es mayor
# Se hace la siguiente pregunta: Si numero_uno es mayor que numero_dos
if (numero_uno > numero_dos):
	# Si la respuesta es verdadera se ejecuta la siguiente condición
	print("El numero: " + str(numero_uno) +" es mayor.")
# En caso que la primera instrucción no sea verdadera se ejecuta toda la sección de "else"
else:
    print("El numero: " + str(numero_dos) +" es mayor.")
```

> Desafío

Crear una variable tipo bool, si la variable es True, deberá imprimir el siguiente mensaje: "La variable es True", caso contrario si no se cumple la función debe imprimir el mensaje: "La variable es False". Puede jugar cambiando la declaración de la variable por True y False respectivamente para ver que el programe funcione. 

## 12. Entrada de Datos en Python, 13. Entrada de Datos en Visual Studio Code

`input()` → Nos sirve para ingresar valores externos de nuestro programa, pero si colocamos solo ese comando el dato de entrada por más de ser un número estará en cadena de texto "string".

`int(input())` → Nos sirve para ingresar datos numéricos enteros.