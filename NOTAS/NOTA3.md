# 1 ciclos 
Un ciclo sirve para repetir acciones sin tener que escribir el mismo código muchas veces.
En Python usamos principalmente dos ciclos:

- while

- for

¿Qué es un ciclo en el fondo?

- Un ciclo no es código.
- Un ciclo es una pregunta que se repite.
- “¿Todavía debo seguir?”

Mientras la respuesta sea sí, el ciclo continúa.
Cuando la respuesta es no, el ciclo termina.
Eso es todo.

La estructura mental de TODO ciclo

Todo ciclo, sin excepción, tiene 4 cosas:

1. Un inicio

2. Una condición

3. Una acción

4. Un cambio

Si falta una → el ciclo falla.

Ejemplo humano (sin programación)

Imagina subir escaleras:

- Inicio: estás en el escalón 1

- Condición: ¿aún no llegué arriba?

- Acción: subir un escalón

- Cambio: ahora estás en el siguiente escalón

- Cuando llegas arriba → el ciclo termina solo.

Eso ES un ciclo.

El error clásico (y por qué pasa)

La gente piensa solo en la acción:

“Quiero imprimir algo varias veces”

Pero olvida el cambio.

Si no hay cambio:

- la condición nunca se vuelve falsa

- el ciclo se queda atrapado

- ciclo infinito 😵‍💫

Lógica del while

El while es el ciclo más puro.

Mentalmente se lee así:

“Mientras esto sea verdad, sigue”

Ejemplo lógico:

Mientras no tenga la contraseña correcta, seguir preguntando.

La clave del while es:
🧠 tú controlas cuándo termina

Por eso es peligroso si no entiendes la lógica.

Lógica del for

El for es un ciclo controlado.

Mentalmente se lee así:

“Para cada elemento, haz esto”

Tú no te preocupas por:

- cuándo empieza

- cuándo termina

Eso ya viene definido (lista, rango, texto).

Por eso el for es más seguro.



## 1.2 Ciclo while

El ciclo while repite el código mientras una condición sea verdadera.

``` python
contador = 1

while contador <= 5:
    print(contador)
    contador += 1
```
📌Mientras contador <= 5 sea verdadero, el ciclo continúa.
contador += 1 evita un ciclo infinito.

Ciclo infinito (⚠️ cuidado)

```python
while True:
    print("Esto nunca termina")
```
👉 Solo se detiene si el programa se interrumpe o se usa break.

## 1.3 break (romper el ciclo)

```python
numero = 1

while True:
    print(numero)
    if numero == 3:
        break
    numero += 1
```
Cuando se ejecuta break, el ciclo termina.

¿Por qué break existe?

Porque a veces la respuesta ya llegó.

Ejemplo humano:

Busco una llave en una mesa.
La encuentro.
¿Sigo buscando? No.

break es decir:

“Ya no tiene sentido seguir”.

## 1.4 continue (saltar una vuelta)

```python
numero = 0

while numero < 5:
    numero += 1
    if numero == 3:
        continue
    print(numero)
```
👉 continue salta esa iteración y sigue con la siguiente.

¿Qué es continue en el fondo?

continue significa:

“Esta vuelta no me sirve, pasemos a la siguiente.”

No rompe el ciclo.
No lo termina.
Solo salta el resto de la iteración actual.

La lógica humana detrás de continue

Imagina esto:

Estás revisando una lista de correos
Si el correo es spam → lo ignoras
Si no → lo lees

No dejas de revisar correos (no es break),
solo saltas ese.

Eso es continue.

Estructura lógica de un ciclo con continue

1. Empieza la vuelta

2. Evalúas una condición

3. Si no sirve → continue

4. Si sirve → ejecutas el resto

5. Cambio

6. Siguiente vuelta

## 1.5 Ciclo for

El ciclo for se usa cuando sabemos cuántas veces queremos repetir algo.

```python
for i in range(5):
    print(i)
```
Resultado:

```python
0
1
2
3
4
```
📌 range(5) va de 0 a 4.

### 1.5.1 range() explicado

```python
range(inicio, fin, paso)
```
Ejemplos:

```python
for i in range(1, 6):
    print(i)

for i in range(0, 10, 2):
    print(i)

```
### 1.5.2 Recorrer texto con for

```python
palabra = "python"

for letra in palabra:
    print(letra)
```
### 1.5.3 for con condiciones

```python
for i in range(1, 11):
    if i % 2 == 0:
        print(i, "es par")
```

else en ciclos (for y while)

En Python, los ciclos pueden tener un else.

⚠️ Esto NO significa “si no” como en if.

👉 El else del ciclo se ejecuta solo si el ciclo termina normalmente,
es decir, sin usar break.

Ejemplo con for + else

```python
for i in range(3):
    print(i)
else:
    print("El ciclo terminó correctamente")
```

Salida:

```python
0
1
2
El ciclo terminó correctamente
```
📌 El else se ejecuta porque el ciclo terminó sin interrupciones.

for + break + else

```python
for i in range(5):
    if i == 3:
        break
    print(i)
else:
    print("Esto NO se ejecuta")
```
📌 El else no se ejecuta porque hubo un break.

Uso típico (muy importante)

Buscar algo.

```python

numeros = [1, 3, 5, 7]

for n in numeros:
    if n == 4:
        print("Número encontrado")
        break
else:
    print("Número no encontrado")
```
👉 El else se ejecuta solo si NO se encontró el número.

Resumen claro 🧠

El else en ciclos:

-  Se ejecuta si el ciclo termina normal

-  No se ejecuta si hay break

- Funciona tanto con for como con while

- Es útil para búsquedas y validaciones

## 1.6 Comparación rápida

Ciclo	¿Cuándo usarlo?
while	No sabes cuántas veces se repetirá
for	Sabes cuántas veces se repetirá

Cierre conceptual 🧠

Los ciclos permiten automatizar tareas repetitivas.
Gracias a ellos, el código es más corto, más claro y más poderoso.
























