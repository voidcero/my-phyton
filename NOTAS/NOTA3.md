# 1 ciclos 
Un ciclo sirve para repetir acciones sin tener que escribir el mismo código muchas veces.
En Python usamos principalmente dos ciclos:

- while

- for

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

## 1.6 Comparación rápida

Ciclo	¿Cuándo usarlo?
while	No sabes cuántas veces se repetirá
for	Sabes cuántas veces se repetirá

Cierre conceptual 🧠

Los ciclos permiten automatizar tareas repetitivas.
Gracias a ellos, el código es más corto, más claro y más poderoso.
























