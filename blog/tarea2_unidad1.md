# Tarea 2 - Ejercicios Unidad 1

## Reto 1 simula el comportamiento de la tortuga usando solo print() e input()

```python
pasos = 50
print("creando tortuga simulada que da...", pasos, "pasos")
print("-" * pasos + ">")
```

## Reto 2 Tortuga bajando

```python
pasos = 10
for i in range(pasos):
    print("|")   
print("V")

print("La tortuga bajo",pasos,"pasos.")
```

## Reto 3 Girar y dibujar usando solo print() e input()

```python
pasos_bajada = 15
pasos_adelante = 10

print("-" * pasos_adelante + ">")

for i in range(pasos_bajada):
    print(" " * pasos_adelante + "|")   

print(" " * pasos_adelante + "V")


pasos_totales = pasos_adelante + pasos_bajada

print("La tortuga avanzo", pasos_adelante,"pasos.")
print("La tortuga bajo", pasos_bajada, "pasos.")
```

## Reto 4 Encapsula los comportamientos anteriores usando funciones

```python
def adelante(pasos):
    global pasos_adelante
    pasos_adelante = pasos
    print("-" * pasos + ">")


def abajo(pasos):
    for i in range(pasos):
        print(" " * pasos_adelante + "|")

    print(" " * pasos_adelante + "V")

adelante(9)
abajo(7)
```

## Reto 5 La tortuga baja las escalones

```python
posicion_x = 0
posicion_y = 0

def adelante(pasos):
    global posicion_x, posicion_y
    print(" " * posicion_x + "-" * pasos + ">")
    posicion_x += pasos

def abajo(pasos):
    global posicion_x, posicion_y

    for i in range(pasos):
        print(" " * posicion_x + "|")
    
    print(" " * posicion_x + "V")

    posicion_y += pasos

adelante(8)
abajo(9)
```
        
