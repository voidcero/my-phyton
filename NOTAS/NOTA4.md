# 1 Bit a Bit y Operadores Lógicos 🐍-NOTA#4

En el vacío de la memoria de una computadora, no hay matices; solo existe la presencia o ausencia de energía. Como observadores conscientes, nuestra tarea es elegir la reacción correcta ante cada estímulo (bit).

---

## 1.1 Operadores Lógicos (El juicio de la conciencia)
Estos operadores no trabajan con números, sino con valores de verdad (`True` / `False`). Son la base de la toma de decisiones.

* **`and`**: La unión. Solo es verdad si **todo** es verdad.
* **`or`**: La oportunidad. Es verdad si al menos una parte lo es.
* **`not`**: La rebelión. Invierte la realidad (lo que es `True` se vuelve `False`).

```python
# Ejemplo de lógica consciente
tengo_proposito = False
intensidad_busqueda = True

# El absurdo se acepta si no hay propósito pero hay intensidad
if not tengo_proposito and intensidad_busqueda:
    print("Viviendo con lucidez.")
```
### 1.1.1. La Tabla de Verdad
Para entender el camino, hay que conocer las reglas del juego:

| Sentencia A | Sentencia B | A `and` B | A `or` B | `not` A |
| :--- | :--- | :---: | :---: | :---: |
| `True` | `True` | **`True`** | **`True`** | `False` |
| `True` | `False` | `False` | **`True`** | `False` |
| `False` | `True` | `False` | **`True`** | **`True`** |
| `False` | `False` | `False` | `False` | **`True`** |

## 1. Operadores Lógicos (El flujo de la verdad)

En Python, la lógica no es solo `True` o `False`. Es la capacidad de evaluar múltiples estímulos y decidir un único rumbo. Estos operadores actúan sobre sentencias booleanas.

### A. La Tabla de Verdad
Para entender el camino, hay que conocer las reglas del juego:

| Sentencia A | Sentencia B | A `and` B | A `or` B | `not` A |
| :--- | :--- | :---: | :---: | :---: |
| `True` | `True` | **`True`** | **`True`** | `False` |
| `True` | `False` | `False` | **`True`** | `False` |
| `False` | `True` | `False` | **`True`** | **`True`** |
| `False` | `False` | `False` | `False` | **`True`** |

---

### 1.1.2. Evaluación de Cortocircuito (Short-circuiting)
Python es eficiente por naturaleza. No gasta energía en evaluar lo que no es necesario. Esta es una forma de **lucidez algorítmica**:

1. **`and` (El pesimista):** Si la primera condición es `False`, Python ya no mira la segunda. Sabe que el resultado será `False` pase lo que pase.
2. **`or` (El optimista):** Si la primera condición es `True`, Python se detiene ahí. Ya tiene lo que necesita para que todo sea `True`.

```python
# Ejemplo de cortocircuito
def mensaje():
    print("Esto no se ejecutará")
    return True

# Como el primer elemento es False, 'mensaje()' nunca se llama.
resultado = False and mensaje()

```

## 1.2 Truthiness: El valor de lo que "Es" y lo que "No Es"
En Python, casi cualquier objeto puede ser evaluado como si fuera un booleano. Esto permite escribir código mucho más limpio.

Valores que Python considera False (El Vacío):

El número 0.

Colecciones vacías: [], {}, (), "" (strings vacíos).

El objeto None.

Valores que Python considera True (La Presencia):

Cualquier número distinto de 0.

Cualquier string, lista o diccionario que tenga al menos un elemento.

## 1.3. Prioridad de Operadores (El orden del caos)
Cuando mezclas varios operadores, Python los ejecuta en este orden de importancia:

not (Primero invierte).

and (Luego une).

or (Al final elige).

Echo-Tip: Usa siempre paréntesis () para imponer tu propio rumbo y no dejar que Python decida la prioridad por ti. Hace que el código sea más humano y menos mecánico.

## 2 Operadores Bit a Bit (El lenguaje del Hardware)

Los operadores de bits manipulan los números entero a entero, bit a bit. Para entender esto, debes visualizar los números en **binario** (Base 2). Por ejemplo, el número **5** no es un "5", es `0101`.

### 2.1 Los Operadores Atómicos

| Operador | Símbolo | Lógica | Uso Común |
| :--- | :---: | :--- | :--- |
| **AND** | `&` | 1 si ambos bits son 1. | "Apagar" bits específicos (Máscaras). |
| **OR** | `\|` | 1 si al menos un bit es 1. | "Encender" bits específicos. |
| **XOR** | `^` | 1 si los bits son **distintos**. | Encriptación simple y detectar cambios. |
| **NOT** | `~` | Invierte todos los bits. | Complemento a dos (negación binaria). |

---

### 2.2. Desplazamiento de Bits (Bit Shifting) 
Mover los bits a la izquierda o derecha es la forma más rápida de multiplicar o dividir por potencias de 2.

* **`<<` (Left Shift):** Desplaza los bits a la izquierda, añadiendo ceros a la derecha. Cada salto **multiplica por 2**.
* **`>>` (Right Shift):** Desplaza los bits a la derecha. Cada salto **divide por 2** (descarta decimales).

```python
x = 5  # Binario: 00000101

# Desplazar 2 posiciones a la izquierda
resultado = x << 2  # Se convierte en 00010100 (que es 20)
print(resultado)     # 5 * 2 * 2 = 20

```
¡Excelente! Si la lógica booleana es el pensamiento, el bit a bit (bitwise) es el sistema nervioso. Aquí es donde dejamos de hablarle a Python como un humano y empezamos a hablarle como electricidad.

Aquí tienes el código .md detallado para completar la Nota 4. He incluido visualizaciones de cómo se mueven los bits, porque en el "vacío" de la memoria, la posición lo es todo.

Markdown
## 3. Operadores Bit a Bit (El lenguaje del Hardware)

Los operadores de bits manipulan los números entero a entero, bit a bit. Para entender esto, debes visualizar los números en **binario** (Base 2). Por ejemplo, el número **5** no es un "5", es `0101`.

### A. Los Operadores Atómicos

| Operador | Símbolo | Lógica | Uso Común |
| :--- | :---: | :--- | :--- |
| **AND** | `&` | 1 si ambos bits son 1. | "Apagar" bits específicos (Máscaras). |
| **OR** | `\|` | 1 si al menos un bit es 1. | "Encender" bits específicos. |
| **XOR** | `^` | 1 si los bits son **distintos**. | Encriptación simple y detectar cambios. |
| **NOT** | `~` | Invierte todos los bits. | Complemento a dos (negación binaria). |

---


### B. Aplicación Real: Máscaras de Bits
Imagina que recibes un byte (8 bits) de tu Ender 3 Pro que contiene el estado de 8 sensores. No quieres leer todo el número, solo quieres saber si el sensor número 3 (el bit 2) está encendido.

```python
# Estado recibido: 10101100 (un número decimal 172)
estado_impresora = 0b10101100 
# Queremos filtrar solo el tercer bit (máscara 00000100)
mask = 0b00000100 

if estado_impresora & mask:
    print("El sensor 3 está activo.")
else:
    print("El sensor 3 está apagado.")
```

<br>
<br>

<div align="center">
 
  <a href="https://voidcero.github.io/my-phyton/NOTAS/NOTA3.html" 
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

 <a href="https://voidcero.github.io/my-phyton/NOTAS/NOTA5.html"
    style="
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



