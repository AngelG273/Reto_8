# Reto_8

Ejercicio 1

a)
``` Python
def Impares():
    impares = [num for num in range(1, 1000) if num % 2 != 0]
    return impares

def Pares():
    pares = [num for num in range(2, 1001) if num % 2 == 0]
    return pares

if __name__ == "__main__":
    # Imprimimos los números impares
    print("Números impares:")
    print(Impares())
    
    # Imprimimos los números pares
    print("Números pares:")
    print(Pares())
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
def Impares(*args):
    impares = [num for num in args if num % 2 != 0]
    return impares

def Pares(*args):
    pares = [num for num in args if num % 2 == 0]
    return pares

if __name__ == "__main__":
    # Generamos los números del 1 al 1000
    numeros = list(range(1, 1001))
    
    # Imprimimos los números impares
    print("Números impares:")
    print(Impares(*numeros))
    
    # Imprimimos los números pares
    print("Números pares:")
    print(Pares(*numeros))
```

b)
```Python
import math

def print_factorials(*args):
    for num in args:
        print(f"{num}! = {math.factorial(num)}")

if __name__ == "__main__":
    # Se evalua que el numero ingresado sea mayor o igual a 2
    while True:   
        n = int(input("Ingrese un numero mayor a 2:"))
        if n >= 2:
            break
        else:
            print("Ingrese un numero mayor a 2:")

    # Generar una lista de números de 1 a n
    numbers = list(range(1, n + 1))
    
    # Imprimir los números y sus factoriales
    print_factorials(*numbers)
```

Ejercicio 3
```Python
def potencia(base, exponente):
    # Caso base: cualquier número elevado a la potencia de 0 es 1
    if exponente == 0:
        return 1
    # Caso recursivo: multiplicar la base por la potencia de la base con el exponente reducido en 1
    else:
        return base * potencia(base, exponente-1)

if __name__ == "__main__":
  # Se ingresa la base
  a = int(input("Ingrese la base:"))
  # Se ingresa la potencia
  b = int(input("Ingrese el exponente al cual va a elevar la base:"))
  # Se llama la funcion 
  resultado = potencia(a, b)
  print(resultado)  
```
Stackoverflow
![image](https://github.com/user-attachments/assets/1715562a-d336-4ccf-97de-151bd36e7b4f)
linkedin
![image](https://github.com/user-attachments/assets/6c437dec-17fc-4bff-aeb8-4d99568a1970)
