
#### Variable:

```py
var1 = 1
print("El valor es: {}".format(var1))
```

#### Asignación múltiple de variables

```py
(x, y, z) = (1, 2, 3)
print(str(x), str(y), str(z))
```

#### Ejemplo de switch case:

```py
x = 10
if x == 10:
    print("El valor es diez")
elif x == 20:
    print("El valor es veinte")
elif x == 30:
    print("El valor es treinta")
else:
    print("Valor no coincide")
```

#### Ejemplo de comentario:

```py
# Comentario en linea

'''
Comentario
multiples lineas
o documentacion
'''
```

#### Operadores aritméticos:

```py
print("Suma: " + str(2 + 2))
print("Resta: " + str(10 - 4))
print("Division sin decimales: " + str(40 // 35))
print("Division con decimales: " + str(40 / 35))
print("Multiplicacion: " + str(4 * 4))
print("Potencia: " + str(4 ** 4))
print("Modulo: " + str(10 % 2))
```

#### Operador ternario:
```py
print("Diez es par") if 10 % 2 == 0 else print("Diez es impar")
print("Once es par") if 11 % 2 == 0 else print("Once es impar")
```

#### Ejemplo de diccionario (Hash):

```py
diccionario = { "Nombre": "Javi", "Edad": 34 }
print("El nombre es: " + diccionario["Nombre"])
diccionario["Nombre"] = "Javier"
print("El nombre ahora es: " + diccionario["Nombre"])
del diccionario["Nombre"]
print("\nImprimiendo diccionario:")
for clave, valor in diccionario.items():
    print(clave, valor)
diccionario["Nombre"] = "Javi"
print("El nombre ahora es: " + diccionario["Nombre"])
# Vaciar diccionario:
diccionario.clear()
```

#### Ejemplo de lista (Array dinámico):

```py
lista = [1, 2, 3, 4, 5, "perro", 4.55]
print("\nLa última posición de la lista es: " + str(lista[-1]))
# Añadir un valor al final de la lista:
lista.append("Pelota")
print("\nLa última posición de la lista es: " + str(lista[-1]))
# Insertar un valor en la tercera posicion de la lista:
lista.insert(2, "Zanahoria")

lista2 = [10, 20, 30]
print("Eliminando ultimo valor de lista2: " + str(lista2.pop()))
# Concatenar listas:
lista.extend(lista2)

print("El valor perro esta en la posicion: " + str(lista.index("perro")))
print("Existe el valor 34 en la lista? " + str(34 in lista))
print("\nImprimiendo la lista de apuntes:")
for lis in lista:
    print(lis)
```

#### Ejemplo de tupla (lista constante):

```py
# Ejemplo de tupla (similar a array, pero constante)
tupla = (1, 2, "Perro", "Atún", 3.45667)
print("\nImprimiendo tupla:")
for tu in tupla:
    print(tu)
```

#### Ejemplo creación de clase:

```py
class Equipo:
    # constructor
    def __init__(self, nombre):
        self.nombre = nombre

    # getters
    def getNombre(self):
        return self.nombre

    # setters
    def setNombre(self, nombre):
        self.nombre = nombre

equipo1 = Equipo("Barcelona")
print("El nombre del equipo es: " + equipo1.getNombre())
equipo1.setNombre("FC Barcelona")
print("El nombre del equipo es: " + equipo1.getNombre())
```

#### Ejemplo de comparación de objetos:

```py
# Comparando dos objetos para ver si son el mismo en memoria:
equipo2 = Equipo("FC Barcelona")
print("El equipo1 es el mismo que el equipo 2? " + str(equipo1 is equipo2))

# Comparando dos objetos para ver si son el mismo valor:
print("El equipo1 tiene el mismo valor que el equipo 2? " + str(equipo1.getNombre() == equipo2.getNombre()))
```


#### Ejemplo de excepción:

```py
# El bloque try se comprueba si el codigo tiene errores
try:
    resultado = 10 / 0
# El bloque except se ejecuta si hay algun error en el bloque try
except ZeroDivisionError: # Podría añadirse varios separados por coma
    print("Error: No dividas por cero")
# El bloque else se ejecuta al finalizar el bloque try sin errores
else:
    print("La división salió bien")
# El bloque finally se ejecuta siempre, falle o no (usado normalmente para limpiar recursos)
finally:
    print("Operación terminada")
```

#### Ejemplo excepción manual:

```py
raise ValueError("La edad no puede ser negativa")
```