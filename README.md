# exmane_ordinario_2023_2024_AGF

import random
import sys

# creamos el bucle y le decimos que lo itere de 2 en 2 


#creación de la función para crear la pirámide de asteriscos
def construir_piramide (numero_usuario):
    for i in range (1,numero_usuario+1, 2 ):
        espacios = (numero_usuario-i) // 2 
        print(' ' * espacios + '*' * i + ' ' * espacios)

# Creación de la función que solicite el número al usuario y verifique que es mayor que 1
    
def numero():
    try:
        numero_usuario = int(input("Ingrese un número entero mayor o igual a 1: "))
        if numero_usuario < 1:
            raise ValueError("El número debe ser mayor o igual a 1.")
        
        construir_piramide(numero_usuario)

    except:
        print ("Por favor seleccione un número mayor que 1")


# llamamos a la función para que se ejecute de principal
if __name__ == "__main__":
    numero()

