# 1. Variables y tipos de datos en Python 🐍

Esta nota explica qué son las variables y los tipos de datos en Python de una forma sencilla,
con ejemplos claros y sin complicaciones.

---

## 1.1 ¿Qué es una variable?

Una variable es **una forma de guardar información** para usarla después.

Puedes imaginarla como una **cajita con nombre** donde guardas un valor.

```python
edad = 23
```
Aquí:

- edad → es el nombre de la variable

- = → significa “guardar”

- 23 → es el valor que se guarda


## 1.2 ¿Por qué se llaman variables?

Porque pueden cambiar.

```python
edad = 23
edad = 24
```
El valor cambió, pero la variable sigue siendo la misma.

## 1.3 Reglas simples para nombrar variables

- No pueden empezar con números

- No pueden tener espacios

- Se recomienda usar nombres claros

Ejemplos correctos:

```python
nombre = "Juan"
altura = 1.73
es_estudiante = True
```
Ejemplos incorrectos:

```python
1edad = 23      # empieza con número
mi nombre = "A" # tiene espacio
```
## 1.4 Tipos de datos básicos

En Python, los valores tienen tipos.
El tipo depende de qué clase de información se guarda.

### 1.4.1 Números enteros (int)
Son números sin decimales.

23 → es el valor que se guarda


```python
edad = 23
cantidad = 10
```
### 1.4.2 Números decimales (float)

Son números con decimales.

```python
altura = 1.73
precio = 19.99
```

### 1.4.3 Texto (str)

Se usan para palabras o frases.
Siempre van entre comillas.

```python
nombre = "Juan"
mensaje = "Hola mundo"
```

## 1.4.4 Valores lógicos (bool)

Solo pueden ser:

-True

-False

Sirven para representar sí / no, verdadero / falso.

```python
es_estudiante = True
tiene_trabajo = False
```

## 1.5 Ver el tipo de una variable

Puedes usar type() para saber qué tipo tiene una variable.

```python
edad = 23
print(type(edad))
```
Esto mostrará:

```python
<class 'int'>
```
## 1.6 Ejemplo completo y sencillo

```python
nombre = "Juan"
edad = 23
altura = 1.73
es_estudiante = True

print(nombre)
print(edad)
print(altura)
print(es_estudiante)
```
Este programa:

-guarda información y luego la muestra en pantalla

## 1.7 Idea clave para recordar 🧠

Una variable no es complicada.
Es solo un nombre que guarda algo.

Si entiendes eso, ya entendiste lo más importante.

## 1.8 Entrada de datos con input()

En Python podemos pedirle información al usuario usando la función input().

```phyton
nombre = input("Ingresa tu nombre: ")
print("Hola", nombre)
```
📌 Importante:
Todo lo que entra por input() siempre es texto (str), aunque el usuario escriba números.

## 1.9 Conversión de tipos

A veces necesitamos convertir los datos para poder trabajar con ellos correctamente.

Ejemplo con números

```phyton
edad = input("Ingresa tu edad: ")
edad = int(edad)

print("El próximo año tendrás", edad + 1)
```

Ejemplo con decimales

```phyton
precio = input("Ingresa el precio del producto: ")
precio = float(precio)

print("El precio con descuento es:", precio * 0.9)
```
Resumen rápido

-input() sirve para recibir datos del usuario.

-Los datos que entran por input() son de tipo str.

-Podemos convertir los datos usando:

  -int() para números enteros

  -float() para números decimales

-La conversión nos permite hacer cálculos y tomar decisiones

[NOTAS 2- CONDICIONALES](NOTAS2.md)
