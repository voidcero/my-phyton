# 1. Variables y tipos de datos 🐍-NOTA#1

Esta nota explica qué son las variables y los tipos de datos en Python de una forma sencilla,
con ejemplos claros y sin complicaciones.

---

## 1.0 ¿Qué es una variable?

Una variable es **una forma de guardar información** para usarla después.

Puedes imaginarla como una **cajita con nombre** donde guardas un valor.

```python
edad = 23
```
Aquí:

- edad → es el nombre de la variable

- = → significa “guardar”

- 23 → es el valor que se guarda


## 1.1 ¿Por qué se llaman variables?

Porque pueden cambiar.

```python
edad = 23
edad = 24
```
El valor cambió, pero la variable sigue siendo la misma.

## 1.2 Reglas simples para nombrar variables

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
## 1.3 Tipos de datos básicos

En Python, los valores tienen tipos.
El tipo depende de qué clase de información se guarda.

### 1.3.1 Números enteros (int)
Son números sin decimales.

23 → es el valor que se guarda


```python
edad = 23
cantidad = 10
```
### 1.3.2 Números decimales (float)

Son números con decimales.

```python
altura = 1.73
precio = 19.99
```

### 1.3.3 Texto (str)

Se usan para palabras o frases.
Siempre van entre comillas.

```python
nombre = "Juan"
mensaje = "Hola mundo"
```

## 1.3.4 Valores lógicos (bool)

Solo pueden ser:

- True

- False

Sirven para representar sí / no, verdadero / falso.

```python
es_estudiante = True
tiene_trabajo = False
```

## 1.4 Ver el tipo de una variable

Puedes usar type() para saber qué tipo tiene una variable.

```python
edad = 23
print(type(edad))
```
Esto mostrará:

```python
<class 'int'>
```
## 1.5 Ejemplo completo y sencillo

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

- guarda información y luego la muestra en pantalla

## 1.6 Idea clave para recordar 🧠

Una variable no es complicada.
Es solo un nombre que guarda algo.

Si entiendes eso, ya entendiste lo más importante.

## 1.7 Mostrar información con print()

La función print() sirve para mostrar información en pantalla.


```python
print("Hola mundo")
```
También puede mostrar variables:
```python
print("Hola mundo")
```
O texto junto con variables:
```python
print("Hola mundo")
```

Separador sep

Cuando print() muestra varios valores, por defecto los separa con un espacio.

```python
print("Hola", "Juan", "Fernando")
```

Resultado:

```python
 Hola Juan Fernando
```

Podemos cambiar ese separador usando sep.

``` python
print("Hola", "Juan", "Fernando", sep="-")
```
Resultado:
``` python
Hola-Juan-Fernando
```

📌 sep significa separator (separador).

Final de línea end

Por defecto, print() hace un salto de línea al final.

```python
print("Hola")
print("Mundo")
```

Resultado:
```python
Hola
Mundo
```
Podemos cambiar ese comportamiento usando end.

``` python
print("Hola", end=" ")
print("Mundo")
```

Resultado:

```python
Hola Mundo
```

📌 end define qué se imprime al final del print.

Resumen rápido

- print() muestra información en pantalla

- sep cambia el separador entre valores

- end cambia el final del print

- print() y input() trabajan juntos para interactuar con el usuario


## 1.8 Entrada de datos con input()

En Python podemos pedirle información al usuario usando la función input().

```python
nombre = input("Ingresa tu nombre: ")
print("Hola", nombre)
```
📌 Importante:
Todo lo que entra por input() siempre es texto (str), aunque el usuario escriba números.

## 1.9 Conversión de tipos

A veces necesitamos convertir los datos para poder trabajar con ellos correctamente.

Ejemplo con números

```python
edad = input("Ingresa tu edad: ")
edad = int(edad)

print("El próximo año tendrás", edad + 1)
```

Ejemplo con decimales

```python
precio = input("Ingresa el precio del producto: ")
precio = float(precio)

print("El precio con descuento es:", precio * 0.9)
```
Resumen rápido

- input() sirve para recibir datos del usuario.

- Los datos que entran por input() son de tipo str.

- Podemos convertir los datos usando:

  - int() para números enteros

  - float() para números decimales

- La conversión nos permite hacer cálculos y tomar decisiones
<br>
<br>

<div align="center">
 
  <a href="https://voidcero.github.io/my-phyton/" 
   style="background-color: #da3633;
   color: white; 
   padding: 12px 24px; 
   text-decoration: none; 
   border-radius: 10px; 
   font-weight: bold; 
   display: inline-block;
   left: 100px;">
   🐍NOTA ANTERIOR
  </a>

 <a href="https://voidcero.github.io/my-phyton/NOTAS/NOTA2.html" style="
    background-color: #2f81f7; 
    color: white; 
    padding: 12px 24px; 
    text-decoration: none; 
    border-radius: 10px; 
    font-weight: bold; 
    display: inline-block;
    margin: 5px;">
    SIGUIENTE NOTA🐍
    </a>

</div>
