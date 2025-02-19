# Reto_8

Ejercicio 1

a)
``` Python
lista_cuadrados = list(map(lambda x: (x, x**2), range(1, 101)))
for numero, cuadrado in lista_cuadrados:
    print(f"{numero}: {cuadrado}")
```
b)
```Python
n = int(input("Ingrese un número natural n (≥2): "))

# Usamos filter con lambda para obtener los pares en un rango descendente
pares_descendentes = list(filter(lambda x: x % 2 == 0, range(n, 1, -1)))

# Imprimimos los números pares en orden descendente
print(*pares_descendentes)

```

c)
```Python
def factorial_de_numero(n):
  factorial = 1
  for i in range(1,n+1):
    factorial *=i # Se multiplica el 1 por el numero que esta dentro del rango
  return factorial

if __name__=="__main__":
  #Se define el valor n
  n = int ( input ("Ingrese un numero natural:"))
  #se define el rango para i
  for i in range(1,n+1):
    # se llama la función factorial
    Factorial_n = factorial_de_numero(i)
    # Se imprime i y su factorial
    print(str(i) + " su factorial es " + str(Factorial_n))
```

Ejercicio 2
a)
```Python

```

b)
```Python

```

c)
```Python

```
Ejercicio 3
```Python

```
