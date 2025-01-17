# Aprende un lenguaje de programación en un día (ejercicio voluntario para subir nota).

## Introducción

Cuando te sacaste el carnet de conducir, aprendiste las normas de circulación así como los fundamentos básicos para manejar un coche: volante, marchas, freno, acelerador, embrague, retrovisores... Seguramente, el coche que conduces ahora es diferente al que utilizaste para aprender a conducir, no obstante, lo puedes llevar sin problema. Cada coche tiene sus peculiaridades, pero quien sabe manejar un automóvil, puede adaptarse a las medidas, tacto y comportamiento de un vehículo en cuestión de horas.

Aprender a programar es como aprender a conducir. Si tienes una base sólida de programación y sabes manejar con soltura los tipos de datos, bucles, arrays, clases, métodos, etc. podrás pasar de un lenguaje a otro en un período relativamente corto, simplemente tendrás que adaptarte a la sintaxis y a las peculiaridades del nuevo lenguaje.

Con este ejercicio se pretende despertar el interés por otros lenguajes de programación distintos al que el alumno está estudiando como primer lenguaje.

Sigue los pasos que se indican a continuación.

## Creación del equipo

Este ejercicio se debe hacer en grupos de 3 alumnos. Uno de ellos será el representante del grupo.

## Forkea forkea

El representante del grupo debe hacer un *fork* de este repositorio para utilizarlo como base.

## Añadiendo colaboradores

El encargado del grupo deberá añadir como colaboradores del repositorio *forkeado* a los otros dos miembros, para trabajar todos sobre los mismos archivos. Cuando alguien es colaborador en un repositorio, puede hacer *push* a él sin necesidad de pedir permiso o hacer *pull request*.

Para añadir colaboradores hay que hacer click en la pestaña *Settings* y seleccionar luego *Collaborators* en el menú.

## Miembros del grupo

Escribe aquí los miembros del grupo. El primero es el representante o encargado.

* Diego Rodríguez
* Álvaro Linero
* Diego Aguilera

## Lenguaje de programación

El profesor llevará una cajita llena de papelitos con los nombres de distintos lenguajes de programación. Los encargados de cada grupo meterán la mano en la caja y sacarán dos papelitos, de los cuales el grupo elegirá uno. No se permite hacer intercambio de papelitos entre grupos.

Escribe el lenguaje de programación elegido por el grupo.

* Python

Los papelitos se han recortado de este [documento](lenguajes_de_programacion.pdf).

## Información sobre el lenguaje



### Breve descripción de Python.
![image](https://user-images.githubusercontent.com/91873599/146731638-cd1a9b66-e1b8-462d-9bf7-26787127e9fd.png)

Python es un lenguaje de programación interpretao que se creó entre la década de los 80 y los 90 y se puede usar para un gran abanico de desarrollo (interfaces gráficas, bases de datos y páginas web). También es ampliamente usado y aceptado por la comunidad científica. 

A diferencia de otros lenguajes de programación, Python es reconocido por tener una sintaxis poco restrictiva. Otra característica que lo define es que a diferencia de Java solo necesitamos el código en sí, ya que puede ser ejecutado tal cuál.

### Comentarios.

_Comentario de una línea:_


![image](https://user-images.githubusercontent.com/91873599/146732844-73963d1e-65d8-40c7-a825-95daae075117.png)

_Comentario de bloque_


![image](https://user-images.githubusercontent.com/91873599/146732865-cf1ea983-4df9-44d0-8cd9-a86555ce9035.png)

Tampoco es necesario poner ";" al final del código, de hecho con un salto de línea nos basta

![WhatsApp Image 2021-12-20 at 09 15 46](https://user-images.githubusercontent.com/91873618/146735730-9cc1ca2b-08ad-43c9-a4fd-63f58a156b00.jpeg)

Incluso podríamos declarar varias variables en la misma línea poniendo ";" entre ellas

![WhatsApp Image 2021-12-20 at 09 16 37 (1)](https://user-images.githubusercontent.com/91873618/146735770-5c3f9d7e-8124-458b-8d63-62ebccfa54fd.jpeg)


## Herramientas de desarrollo

Indica aquí qué software has tenido que instalar para programar en este lenguaje. Añade enlaces y/o capturas de pantalla.

Hemos tenido que descargar Python desde su página oficial. Su última versión es la 3.10.

https://www.python.org/downloads/

![WhatsApp Image 2021-12-20 at 09 06 34](https://user-images.githubusercontent.com/91873618/146734543-975dd68a-650a-4711-a20a-b5950d0a3553.jpeg)


Hemos también tenido que instalar la extensión de Python en VSC para poder ejecutar el código de una manera más cómoda.


![WhatsApp Image 2021-12-20 at 09 08 06](https://user-images.githubusercontent.com/91873618/146734638-33b66c6a-c30c-48a7-9709-790ee3c94e07.jpeg)

Para el ejercicio de Arrays, hemos tenido que instalar el IDE "Spyder". 

![fd8bce49301ba3f37ad24341383fe71f](https://user-images.githubusercontent.com/91873618/146739445-f38fb4e4-4a7c-4f0a-80cb-efface913192.png)




## Poniendo en práctica el lenguaje

Pon en práctica el lenguaje de programación realizando los siguientes ejercicios. Para cada uno de los ejercicios, pega el código fuente de la solución y una captura de pantalla.

### 1. ¡Hola mundo!

Realiza un programa que muestre por pantalla la frase **¡Hola mundo!**.

```python
print("Hola Mundo");
```

![WhatsApp Image 2021-12-20 at 08 52 25](https://user-images.githubusercontent.com/91873618/146733946-0500aca3-ae63-4fa0-ad02-45e3b8d3718e.jpeg)


### 2. Pirámide

Dada una altura introducida por el usuario, realiza un programa que pinte una pirámide a base de asteriscos con la altura indicada.

```python
lineas = int (input ('Numero de lineas'))
for numero_linea in range(lineas):
    espacios = lineas - numero_linea -1
    asteriscos = 1 + numero_linea *2
    print (" "espacios+""*asteriscos)
```

![WhatsApp Image 2021-12-20 at 09 43 26](https://user-images.githubusercontent.com/91873618/146738188-1bda3b49-f104-4984-b535-cca75b737c7d.jpeg)



### 3. Arrays y números aleatorios

Realiza un programa que rellene un array (o una estructura similar) con 20 números enteros aleatorios entre 1 y 100 y que seguidamente los muestre por pantalla. A continuación, se deben pasar los números primos a las primeras posiciones del array y los no primos a las posiciones restantes. Muestra finalmente el array resultado.

```python
import numpy as np
import random

n = 20
aleatorios = [random.randint(1, 100) for _ in range(n)]
print("Esta lista contiene 20 números aleatorios del 1 al 100: ")
print(aleatorios)


def esPrimo(l):
    primos = []
    for i in l:
        p = 0
        if i == 1:
          primos.append(i)
        else:
          for j in range(1,i+1):
            if i % j == 0:
              p += 1
          if p == 2:
            primos.append(i)
    return primos

lista = aleatorios
primos = esPrimo(lista)

for x in range(len(lista)):
    c=0
    control = False
    for y in range(len(primos)):
        if lista[x]!=primos[c]:
           control=True
           c+=1
        else:
            control=False

    if control== True:
        primos.append(lista[x])
print("\nEsta es la lista con los primos al principio")
print (primos)
```

![WhatsApp Image 2021-12-20 at 09 45 42](https://user-images.githubusercontent.com/91873618/146739583-ba2ba69c-1dec-422c-a0c8-ff162493cf0a.jpeg)









## Presentación de resultados

Cada equipo explicará al resto de la clase lo aprendido durante la realización del ejercicio. Todos los miembros de cada equipo deben participar en la explicación. Se puede utilizar como material de base para la presentación el repositorio de GitHub.

## Recompensa

* Todos los alumnos que realicen correctamente la actividad tendrán 0'25 puntos extra en la nota del trimestre.

* Los miembros del equipo más votado ganarán un premio.

:star: Si te ha gustado este ejercicio, dale una estrellita al [repositorio original](https://github.com/LuisJoseSanchez/aprende-un-lenguaje-en-un-dia).

