# 1. Condicionales en python 🐍

En programación, los condicionales sirven para tomar decisiones.
Básicamente le decimos al programa:

- Si pasa algo, haz esto.
- Si no, haz otra cosa.

``` python
edad = 18

if edad >= 18:
    print("Eres mayor de edad")

```

📌 if significa si

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

## 1.1 Comparadores más comunes
| Operador| Edad |
|--------|------|
| == | igual  | 
| != | diferente  | 
| < | menor  | 
| > | mayor  | 
| <=| menor o igual   | 
| >=| mayor o igual  | 

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


Resumen

- if permite tomar decisiones

- else cubre el caso contrario

- elif agrega más opciones

- Las condiciones se basan en comparaciones

- La indentación es obligatoria
