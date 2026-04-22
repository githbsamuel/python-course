# Python Course

---

## Comentarios

Los comentarios se utilizan para añadir notas explicativas 
dentro del código. Son ignorados por el compilador y están
destinados a la comprensión humana. 

En **Python**, hay dos formas de escribir comentarios: 

Comentarios de una sola línea usando el símbolo `#`:

```python
# Este es un comentario
print("Hola!") # Esto imprime "Hola!"

# Usar comentarios para explicar tu código
print("Python is easy") # Esto se mostrara en la pantalla 
```

Comentarios multilínea usando comillas triples(`"""`)

```python
"""
Este es un comentario multilínea.
Puedes escribir múltiples líneas
de explicación aquí.
"""
print("Bienvenido!")
```

### Prácticas comunes de comentarios

1. Comentarios TODO - Marcar tareas futuras

```python
# TODO: Optimizar este bucle para conjuntos de datos grandes
for i in range(1000):
    print(i)
```

2. Desactivar código temporalmente: 

```python
# print("Esta linea esta desactivada")
print("Esta linea esta activada")
```

3. Explicando lógica compleja: 

```python
# Calcular el promedio de la lista
total = sum(numbers)
average = total / len(numbers)
print(avarege)
```
---

## Variables 

En python, `None` representa "ningún valor" o "nada":

```python
caja_vacia = None
```

Convenciones de nomenclatura de variables en Python:

- Usa snake_case palabras separadas por guiones bajos
- Sé descriptivo y usa palabras significativas

```python
# Buenos ejemplos
age = 10
greeitng = "Hola"
is_active = True

# Malos ejemplos
isActive = False # No es snake case
a = 10  # no es descriptivo
```

Un tipo bool(Boolean) tiene solo 2 valores posibles: `True` o
`False`.

Estos valores distinguen entre mayúsculas y minúsculas, lo 
que significa que deben comenzar con una letra mayúscula.

Asignación de valores bool a variables:

```python
"""
Los booleanos son fundamentales para crear lógica
en los programas.
"""
variable_true = True
variable_false = False
```

Un *char* es un solo carácter (por ejemplo, 1, 6, %, b, p, ., T).

Un *str* (cadena) es una secuencia de múltiples caracteres.

Para crear una variable de cadena, encierra el texto entre comillas
simples o dobles:


```python
"""
Tanto las conillas simples como las dobles son válidas
para crear cadenas en Python.
"""
s1 = 'Esto es un string'
s2 = "Esto es un string"
```

### Varibles en Python

- Contenedores que contienen valores o datos
- Se utilizan para almacenar, manipular y mostrar información
- Tienen un nombre único y un valor
- Python detecta automáticamente el tipo de variable

Formato de inicialización de variables:

```python
variable_name = value
```

Tipos de números: 

- `int`: enteros (p, ej., 1,-2)
- `float`: números reales (p. ej., 1.32, 0.98)

Ejemplos

```python
a = 3       # int
b = 13.2    # float
```

---

## Operadores 

### Atajos aritméticos y operador módulo

Python proporciona atajos para operaciones de auto-aritmética:

| Operación      | Atajo | Ejemplo                              |
|----------------|-------| -------------------------------------|
| Suma           | +=    | `a += 3` (equivalente a `a = a + 3`) |
| Resta          | -=    | `a -= 3`                             |
| Multiplicación | *=    | `a *= 3`                             |
| División       | /=    | `a /= 3`                             |
| Módulo         | %=    | `a %= 3`                             |

EL operador módulo `%` devuelve el residuo de una división:

```python
"""                      
17626  <---  dividendo              ___235_   <--- cociente
-                                75| 17626    
75     <---  divisor                  262
                                       376
                                        01    <--- residuo
"""
residuo = dividendo % divisor 
```

Ejemplo: 

```python
residuo = 10 % 3  # el resltado es 1
```

Uso común: comprobar si un número es par o impar: 

- Número par: `numero % 2 == 0`
- Número impar: `numero % 2 == 1`

---

### Operadores lógicos y de comparación

Tablas de verdad para los operadores lógicos en Python:

#### Operador AND

| a     | b     | a `and` b |
|-------|-------|-----------|
| False | False | False     |
| False | True  | False     |
| True  | False | False     |
| True  | True  | True      |

#### Operador OR

| a     | b     | a `or` b |
|-------|-------|-----------|
| False | False | False     |
| False | True  | True      |
| True  | False | True      |
| True  | True  | True      |

#### Operador NOT

| a     | `not` a |
|-------|---------|
| False | True    |
| True  | False   |


Operadores lógicos: 

| Operador | Significado                           | Ejemplo   |
|----------|---------------------------------------|-----------|
| `and`    | True si todos los operadores son True | `a and b` |
| `or`     | True si cualquier operador es TRue    | `a or b`  |
| `not`    | True si el operador es False          | `not a`   |

Ejemplos: 

```python
b1 = (5 > 3) and (1 == 1)  # True
b2 = not 5 == 4 or 5 == 2  # True
b3 = not 1 == 1 or False   # False
b4 = not (3 > 4)           # True
b5 = not (5 > 10 or 5 > 1) # False
```

### Operadores de comparación:

| Operador | Significado       | Ejemplo                 |
|----------|-------------------|-------------------------|
| ==       | Igual             | `1 == 1` devuelve False |
| !=       | No es igual       | `1 != 1` devuelve True  |
| >        | Mayor que         | `1 > 2` devulve False   |
| <        | Menor que         | `1 < 2` devuelve True   |
| >=       | Mayor o igual que | `1 >= 2` devuelve False |
| <=       | Menor o igual que | `1 <= 2` devuelve True  |

Los operadores de comparación devuelven `True` o `False` 
(valores booleanos).

Ejemplo 1:

```python
var1 = 13
var2 = 12
var3 = var1 != var2  # var3 será True
```

Ejemplo 2:

```python
var1 = 13
var2 = 13
var3 = var1 == var2 # var3 será True
```

---

