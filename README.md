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

### Prácticas comunes de comentarios: 

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
variable_true = True
```