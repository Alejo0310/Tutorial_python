# Introduccion_python
# # Tutorial de Python

# ## Contenido 
# 

# ### Introducción a Python
# * ¿Qué es Python?
# * Iniciación en Python
# 
# ### Tipos de datos y variables 
# * Variables
# * Tipos de datos básicos 
# * Conversiones entre tipos de datos 
# * Identificación de tipo de dato
# 
# ### Operaciones entre datos 
# * Operaciones aritmeticas 
# * Operaciones con cadenas 
# * Operadores lógicos 
# * Operadores de comparación 
# 
# ### Indexación de estructuras de datos
# * Listas
# * Tuplas
# * Diccionarios 
# * Conjuntos(Sets)
# 
# ### Estructuras de control 
# * Condicionales 
# * Bucles 
# * Control de bucles 
# ### Funciones 
# * Definición de funciones 
# * Valores de retorno
# * Alcance de las variables 
# * Funciones anónimas 
# 
# ### Modulos e importaciones 
# * Importación de módulos 
# * Módulos estándar 
# * Creación de módulos propios 
# * Uso de __name__ == '__main__'

# # Introducción a Python 
# ### ¿Qué es Python? 
# Python es un lenguaje de programación que se caracteriza por ser fácil de leer y escribir ya que tiene una sintaxis simple y clara. Python tiene aplicaciones en áreas como desarrollo web, ciencia de datos y análisis, IA y aprendizaje automático, automatización de tareas y desarrollo de software.
# 
# 
# 
# 

# ### Iniciación en Python
# * Cómo escribir y ejecutar un programa simple en Python  

# %%
print("Hola mundo")

# * Usar la consola para probar lineas de código y obtener retroalimentación instantánea 

# %%
2+2


# %%
print("Hola," + "Python")

# * Uso de comentarios para explicar código

# %%
# Esto es un comentario

# * Errores frecuentes en Python 
#     - Sintaxis incorrecta 
#     - Errores de tipografía 

# # Tipos de datos y variables 
# ### Variables 
# * Definición de variables 
#    - Es un nombre que se utiliza para almacenar datos. Las variables actuan como etiquetas que hacen referencia a valores almacenados en la memoria. Las variables se pueden reasignar con un nuevo valor a los largo del código.
#    - Las variables pueden ser númericas o de texto
# 

# %%
mi_variable = 20 #La variable es igual a 20
mi_variable #Al llamar la variable se visualiza el 20

# %%
texto = "Hola mundo" #Las variables pueden contener texto 
texto

# ## Reglas para nombrar variables 
#    - Debe comenzar con una letra o un guion bajo(_), nunca con número
#    - No puede contener espacios, se usan guiones bajos para separar palabras(mi_variable en vez de mi variable)
#    - No se pueden usar palabras reservadas de Python(if,ifelse,while,etc)
#    - Nombres de variables sensibles a mayúsculas(mi_variable y Mi_variable son diferentes)
# 

# %%
#Ejemplo correcto 

edad=10
nombre_completo = "Alejandro Pérez"

# %%
#Ejemplo incorrecto

3nombre = "Inválido" #No puede comenzar con número 
mi variable = 5 #No puede tener espacios 

# * Asignación de valores 
#    - El valor de la derecha se asigna al nmbre de la variable de la izquierda. Los valores de una variable se asiganan con el operador `=`

# %%
a = 3
a
b= "Adiós"
b

# ## Tipos de datos básicos 

# ### Enteros `(int)`
# * Números sin decimales 

# %%
numero_entero = 150

# ### Flotantes `(float)`
# * Números con decimales

# %%
numero_flotante = 3.1416

# ### Cadenas de texto `(str)`
# * Texto, encerrado entre comillas simples o dobles

# %%
texto = 'Buenas tardes'

# ### Booleanos `(bool)`
# * Grado de verdad, `True` o `False`

# %%
es_verdadero = True 
es_falso = False

# ### Tipos de datos complejos `(complex)`
# * Números reales con parte real e imaginaria 

# %%
numero_complejo = 2 + 4j 

# ## Conversiones entre tipos de datos
# * Te permite convertir entre distintos tipos de datos utilizando funciones como `int()`,`float()`,`str()`y `bool()`

# %%
numero = "100"  # Es una cadena
numero_entero = int(numero)  # Se convierte en un entero
numero_flotante = float(numero)  # En un número flotante
es_verdadero = bool(1)  # True, porque 1 se evalúa como verdadero
texto = str(100)  # Convierte el número entero 100 a una cadena "100"

# ## Identificación del tipo de dato 
# * La función `type()` permite verificar el tipo de una variable

# %%
a = 5
b = 3.14
c = "Python"
d = True
e = 2 + 3j

print(type(a))  # <class 'int'>
print(type(b))  # <class 'float'>
print(type(c))  # <class 'str'>
print(type(d))  # <class 'bool'>
print(type(e))  # <class 'complex'>


# # Operaciones entre datos 

# ## Operaciones aritméticas 
# 

# * Suma(`+`), resta(`-`), multiplicación(`*`), división(`/`), división entera(`//`), módulo(`%`), exponenciación(`**`)

# %%
#Suma
suma = 5 + 3  # Resultado: 8

# %%
#Resta
resta = 10 - 7  # Resultado: 3

# %%
#Multiplicación
multiplicacion = 4 * 3  # Resultado: 12

# %%
#División 
division = 10 / 3  # Resultado: 3.3333...
#Retorna un número flotante

# %%
#División entera 
division_entera = 10 // 3  # Resultado: 3
#Retorna el resultado entero de la división

# %%
#Módulo
modulo = 10 % 3  # Resultado: 1
#Retorna el residuo de una división

# %%
#Potenciación 
potencia = 2 ** 3  # Resultado: 8
#Eleva un número a la potencia de otro

# ## Operaciones con cadenas 
# Las cadenas de texto (`str`) también pueden ser operadas 

# ### Concatenación
# * Sirve para combinar dos cadenas usando el operador `+`

# %%
cadena1 = "Hola a"
cadena2 = " todos"
resultado = cadena1 + cadena2 
resultado

# ### Repetición 
# * Repite la cadena un número específico  de veces usando el operador `*`

# %%
saludo = "Hola, que tal? " * 5
saludo

# ### Acceso a caracteres 
# * Puedes acceder a un carácter específico de una cadena. Se logra usando los números desde el cero

# %%
palabra = "Python"
primera_letra = palabra[0]  
primera_letra

# ### Slicing
# * Extrae una porción de la cadena utilizando los índices 

# %%
parte = palabra[0:3] 
parte

# ## Operadores lógicos 
# Se utilizan para combinaer condiciones booleanas (`True`o `False`)
# * `and`: Retorna `True` si ambas coniciones son verdaderas

# %%
resultado = True and False  #Resultado: False
resultado

# * `or`: Retorna `True`si al menos una condición es verdadera
# 

# %%
resultado = True or False  # Resultado: True
resultado

# * `not`: Invierte el valor de la condición

# %%
resultado = not True  # Resultado: False
resultado

# ## Operadores de comparación 
# Estos operadores se usan para comparar valores y que estos tomen un grado de verdad según la condición 
# * Igual a (`==`)

# %%
resultado = 5 == 5  # Resultado: True
resultado

# * Diferente de (`!=`)

# %%
resultado = 5 != 3  # Resultado: True
resultado

# * Menor que (`<`)

# %%
resultado = 3 < 5  # Resultado: True
resultado

# * Mayor que (`>`)

# %%
resultado = 7 > 5  # Resultado: True
resultado

# * Menor o igual que (`<=`)

# %%
resultado = 3 <= 3  # Resultado: True
resultado

# * Mayor o igual que (`>=`)

# %%
resultado = 5 >= 2  # Resultado: True
resultado

# # Indexación de estrucuras de datos
# ## Listas 
# Las listas son colecciones ordenadas y mutables
# ### Acceso a elementos por índice 
# * Los elementos de una lista se acceden usando índices, iniciando desde el cero 

# %%
mi_lista = [10, 20, 30, 40, 50]
primer_elemento = mi_lista[0]  # Resultado: 10
ultimo_elemento = mi_lista[-1]  # Resultado: 50 (índice negativo accede desde el final)
primer_elemento
ultimo_elemento

# ### Slicing de listas 
# * Puedes acceder a sublistas utilizando el slicing. Se debe especificar un rango de índices 

# %%
sublista = mi_lista[1:4]  
sublista2 = mi_lista[:3]  # desde el inicio hasta el índice 2
sublista3 = mi_lista[2:]  # desde el índice 2 hasta el final
sublista
sublista2
sublista3

# ## Tuplas 
# Las tuplas son inmutables a diferencia de las listas 
# ### Acceso a elementos de tuplas 
# * También se accede a sus elementos por medio de índices 
# 

# %%
mi_tupla = (100, 200, 300)
elemento = mi_tupla[1]  
elemento

# ## Diccionarios 
# Los diccionarios son colecciones de pares clave-valor. Se accede a los valores usando las claves 
# ### Acceso a valores por clave 
# * Los valores en los diccionarios se recuperan mediante su clave 

# %%
mi_diccionario = {"nombre": "Ana", "edad": 25, "ciudad": "Bogotá"}
nombre = mi_diccionario["nombre"]  
edad = mi_diccionario["edad"]  
edad


# * Tambien se puede acceder a los valores mediante el método `.get()`. si la clave no existe, no arroja un error, sino `None`

# %%
ciudad = mi_diccionario.get("ciudad", "Desconocida")  # Resultado: "Bogotá"
profesion = mi_diccionario.get("profesion", "Desconocida")  # Resultado: "Desconocida"
profesion

# ## Conjuntos (`Sets`)
# Los conjuntos son colecciones desordenadas de elementos únicos. No permiten duplicados y no tienen indices 
# ### Operaciones básicas 
# * Los conjuntos permiten operaciones como la unión, intersección y diferencia 

# %%
conjunto1 = {1, 2, 3, 4}
conjunto2 = {3, 4, 5, 6}

union = conjunto1 | conjunto2 
interseccion = conjunto1 & conjunto2  
diferencia = conjunto1 - conjunto2  
interseccion


# ### Verificación de pertenencia con `in`
# * Permite verificar si un elemento esta o no en un conjunto

# %%
elemento_en_conjunto = 3 in conjunto1
elemento_no_en_conjunto = 5 in conjunto1  
elemento_no_en_conjunto

# # Estructuras de control 
# ## Condicionales 
# Permiten ejecutar bloques de código dependiendo del cumplimiento de una condición 
# * `if`: Ejecuta un bloque de código si la condición es verdadera
# * `elif`: Permite verificar condiciones adicionales si la anterior fue falsa
# * `else`: Ejecuta un bloque de código cuando todas las condiciones anteriores son falsas 

# %%
edad = 20

if edad < 18:
    print("Eres menor de edad")
elif edad == 18:
    print("Tienes 18 años")
else:
    print("Eres mayor de edad")

# ## Bucles 
# Los bucles permiten ejecutar un bloque de código varias veces, ya sea recorriendo una colección de elementos o mientras una condición sea verdadera 
# `for`(iteración sobre listas,rangos,cadenas)
# * Un bucle `for` recorre secuencias (listas,tuplas,cadenas,diccionarios,etc.)

# %%
#Listas
mi_lista = [1, 2, 3, 4, 5]
for numero in mi_lista:
    print(numero)

# %%
#Rangos
for i in range(5):
    print(i)

# %%
#Cadenas 
for letra in "Python":
    print(letra)

# `while`(Bucle basado en condiciones)
# * Un bucle `while`se ejecuta siempre que la condición sea verdadera 

# %%
contador = 0

while contador < 5:
    print(contador)
    contador += 1  # Incrementa el contador

# ## Control de bucles 
# Se usan instrucciones como `break`,`continue` y `else` para controlar el bucle
# `break`
# * Termina el bucle instantáneamente 

# %%
for numero in range(10):
    if numero == 5:
        break  # Se detiene cuando llega al 5
    print(numero)

# `continue`
# * Salta a la siguiente iteración sin ejecutar el resto del código dentro del bucle

# %%
for numero in range(5):
    if numero == 3:
        continue  # Salta el número 3
    print(numero)

# `else`en bucles
# * Se ejecuta cuando el bucle termina de manera normal
# 

# %%
for numero in range(5):
    print(numero)
else:
    print("El bucle terminó")

# %% [markdown]
# # Funciones

# %% [markdown]
# 
# ## Definición de funciones 
# * Las funciones se definen con `def`, seguidas por un nombre, paéntesis y dos puntos

# %%
def saludar():
    print("¡Hola, Mundo!")
    saludar()  # Llama a la función y la ejecuta

# ### Parámetros y argumentos 
# * Los parámetros son variables que una función espera recibir cuando se llama. Los argumnetos son los valores que se pasan a la función 

# %%
def saludar(nombre):
    print(f"¡Hola, {nombre}!")
    saludar("Ana")  # Salida: ¡Hola, Ana!

# ## Valores de retorno
# * Se pueden devolver valores usando la palabra clave `return`.

# %%
def suma(a, b):
    return a + b

# %%
resultado = suma(5, 3)
print(resultado)  # Salida: 8

# ## Alcance de las variables 
# * Las variables locales son aquellas definidas dentro de una función y no son accesibles fuera de ella 
# * Las variables globales están definidas fuera de cualquier función y pueden ser accesibles en cualquier parte del código

# %%
# Ejemplo de variables locales 
def ejemplo():
    x = 10  
    print(x)

ejemplo()
# print(x)  # Esto generaría un error, ya que 'x' no es accesible fuera de la función

# %%
# Ejemplo de variables globales 
x = 10  # Variable global

def mostrar():
    print(x)  # Accede a la variable global

mostrar()  # Salida: 10

# * Se pueden modificar las variables globales dentro de una función usando la palabra `global`

# %%
y = 5

def modificar_global():
    global y
    y = 20

modificar_global()
print(y) 

# ## Funciones anónimas (uso de `lambda`)
# * Las funciones anónimas son funciones pequeñas que no necesitan un nombre y se definen con la palabra clave `lambda`. Son funciones de una sola linea 

# %%
suma = lambda a, b: a + b
print(suma(5, 3))  

# ## Funciones con argumentos predeterminados 
# * Se usan si no se pasa ningún argumento durante la llamada a la función 

# %%
def saludar(nombre="Amigo"):
    print(f"¡Hola, {nombre}!")

saludar()  
saludar("Ana")  

# ## Funciones con argumentos por nombre 
# * Son útiles cuando la función tiene muchos parámetros. Se puede pasar por poscición o por nombre.

# %%
def describir_persona(nombre, edad, ciudad):
    print(f"Nombre: {nombre}, Edad: {edad}, Ciudad: {ciudad}")

# Llamada con argumentos por posición
describir_persona("Carlos", 30, "Bogotá")

# Llamada con argumentos por nombre
describir_persona(edad=30, ciudad="Bogotá", nombre="Carlos")

# # Módulos e importaciones 
# ## Importación de módulos 
# Se puede dividir en código en archivos `.py`. Esto facilita la reutilización del código y la organización del proyecto
# 

# ### Uso de `import`
# * Puedes importar un módulo completo usando la instrucción `import`

# %%
import math  # Importa todo el módulo math

resultado = math.sqrt(16)  
print(resultado)  

# ### Uso de `from ... import`
# * Se importan funciones o variables específicas usando `from ... import`

# %%
from math import sqrt  

resultado = sqrt(25)  
print(resultado)  

# ### Alias para módulos 
# * Se usa el operador `as`para dar un alias al modulo importado 

# %%
import math as m  

resultado = m.sqrt(9)
print(resultado)  

# ## Módulos estándar 
# Son módulos proporcionados por python que tienen funciones útiles 
# 

# Módulo `math`
# * Este módulo proporciona funciones matemáticas avanzadas 

# %%
import math

print(math.pi)  # Valor de pi
print(math.pow(2, 3))  # 2 elevado a la 3

# Módulo `random`
# * Se utiliza para crear una serie de números aleatorios 

# %%
import random

numero_aleatorio = random.randint(1, 10)  
print(numero_aleatorio)

# Módulo `datetime`
# * Define fechas y horas

# %%
import datetime

fecha_actual = datetime.datetime.now()  
print(fecha_actual)

# ## Creación de módulos propios 
# Se crean guardando funciones y variables en archivos `.py`

# %%
# Supongamos un archivo llamado mimodulo.py
def saludar(nombre):
    print(f"¡Hola, {nombre}!")

def despedirse():
    print("¡Adiós!")


# Luego, en otro archivo se puede importar y usar la función de este módulo

# %%
# Archivo principal.py
import mimodulo

mimodulo.saludar("Ana")  
mimodulo.despedirse()  

# ### Uso de `__name__== "__main__"`
# Esta permite ejecutar un archivo como un script o importarlo como módulo sin que se ejecute el código
# * Cuando un archivo es ejecutado directamente, la variable `__name__` se establece en `"__main__"`. Si el archivo es importado, `__name__` toma el valor del nombre del módulo.

# %%
# archivo prueba.py
def saludar():
    print("¡Hola!")

if __name__ == "__main__":
    saludar()  # Esta línea solo se ejecutará si se ejecuta directamente este archivo

# Si se ejecuta `prueba.py`directamente, se imprime ¡Hola!. Si se importa de otro archivo, la función saludar no se ejecutará automáticamente # Tutorial_python
