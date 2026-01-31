# 1. Condicionales en python 🐍



En programación, los condicionales sirven para tomar decisiones.
Básicamente le decimos al programa:

- Si pasa algo, haz esto.
- Si no, haz otra cosa.


## 1.1 - Comparadores más comunes

| Operador | Significado |
|--------|------------|
| == | igual |
| != | diferente |
| < | menor que |
| > | mayor que |
| <= | menor o igual |
| >= | mayor o igual |

Ejemplo:

``` python

numero = 10

if numero == 10:
    print("El número es diez")
```

Condiciones con texto

``` python

password = input("Ingresa la contraseña: ")

if password == "python123":
    print("Acceso concedido")
else:
    print("Contraseña incorrecta")
```
📌 Las comparaciones de texto distinguen mayúsculas y minúsculas.



 
## 1.2 - Condicionales

- La condición debe ser verdadera o falsa

- Los dos puntos : indican que empieza un bloque

- Lo que está indentado pertenece al if

if + else

``` python

edad = int(input("Ingresa tu edad: "))

if edad >= 18:
    print("Puedes ingresar")
else:
    print("No puedes ingresar")
```

- else significa si no

- Solo se ejecuta una de las dos opciones


elif (otra condición)

Se usa cuando hay más de dos posibilidades.

``` python

nota = int(input("Ingresa la nota: "))

if nota >= 4:
    print("Aprobado")
elif nota == 3:
    print("Regular")
else:
    print("Reprobado")
```

👉 elif significa si no, pero si…


## 1.3 - Condicionales anidados

Un if dentro de otro if.

``` python
edad = int(input("Edad: "))

if edad >= 18:
    if edad >= 65:
        print("Adulto mayor")
    else:
        print("Adulto")
else:
    print("Menor de edad")
```

📌 Úsalos con moderación para no enredar el código.


Resumen

- if permite tomar decisiones

- else cubre el caso contrario

- elif agrega más opciones

- Las condiciones se basan en comparaciones

- La indentación es 



## 1.4 - Operadores lógicos

Sirven para combinar varias condiciones.

and (y)

``` python

edad = 20
tiene_id = True

if edad >= 18 and tiene_id:
    print("Puedes ingresar")

```
👉 Ambas condiciones deben cumplirse.

or (o)

``` python

dia = "sabado"

if dia == "sabado" or dia == "domingo":
    print("Es fin de semana")
```

👉 Basta con que una condición sea verdadera.

not (negación)

``` python

lloviendo = False

if not lloviendo:
    print("Puedes salir")
```

👉 Invierte el valor lógico.

Valores booleanos (True y False)


````python

activo = True

if activo:
    print("El sistema está activo")
````

📌 No hace falta escribir == True.


Cierre conceptual 🧠

Los condicionales permiten que el programa reaccione a distintas situaciones.
Gracias a ellos, el código deja de ser lineal y empieza a comportarse de forma inteligente.


