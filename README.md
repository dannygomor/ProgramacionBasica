# ProgramacionBasica

A continuacion se presentara el trabajo de Python, usando sus funciones basicas.

python tieene varios tipos de datos basicos y se dividen en numeros, como puede ser 3 (entero o integral),
1.75 del punto float o bien 7+5j (complejos o complex).
Para poder conocer el tipo de dato de una variable usaremos la instruccion type. Otro tipo de dato basico en 
python son las cadenas de texto. Como se puede notar a diferencia de muchos otros lenguajes en python no se
declara el tipo de variable al crearla.
Para resumir en python se puede representar numeros enteros, reales, complejos, etc. Los numeros enteros son
aquellos numeros positivos o negativos que no tienen decimales. En la mayor parte de las maquinas las variables
enteras pueden almacenaer numeros de -2 a la 31 a 2^31. En plataformas de 64 bites el rango es de -2^63 a 2^63,
en los numeros flotantes son los que tienen decimales y se representa en python mediante el tipo float.
Se pueden representar numeros de -2^64 hasta 2^64, los numeros complejos son aquellos que tienen una parte imaginaria
para definir una variable compleja se utiliza el termino complex.


1° Se hara un programa que mida la longitud y la latitud de la tierra desde un primer punto y un segundo punto y
ambas medidas se sumaran obteniendo el resultado en kilometros.

a = float(input('Insert the latitude of firts point the world: '))
b = float(input('Insert the longitude of firts point the world: '))
c = a + b
d = float(input('Insert the latitude of second point the world: '))
e = float(input('Insert the longitude of second point the world: '))
f = d + e
result = f + c
print('The distance between two points the world is: ', result, 'km')


2° Crear un programa que te indique la hora y la fecha actual.

import time 
print('La hora actual es: ', time.strftime("%I:%M:%S"))
print('La fecha actual es: ', time.strftime("%i/%m/%y"))


3° Crear un programa que te pida las medidas de el largo y ancho de una habitacion y despues obtener su area
en unidad de metros cuadrados.

largo = float(input('insertar el largo de la habitacion:'))
ancho = float(input('insertar el ancho de la habitacion:'))
area = largo * ancho 
print ('el area de tu habitacion es', area, 'metros cuadrados')


4° Crear un programa que te pida las medidas de el largo y ancho de un campo de futbol y despues obtener su area
en unidad de acres.

largo = float(input('insertar el largo de un campo de futbol:'))
ancho = float(input('insertar el ancho de un campo de futbol:'))
area = largo * ancho
print ('el area de tu habitacion es', area, 'acres')


5° Crear un programa que le pida al usuario su nombre y el numero de botellas de un litro o de 2.5 que tiene,
para luego multiplicar el numero de las botellas por la cantidad de litros que tiene y al final sumar los resultados
de las botellas de 1 L. con las 2.5 L., para saber cuanto se tendra que pagar al usuario en pesos.

nombre_cliente = input('Inserte su nombre: ')
A = float(input('Insertar numero de botellas de un 1 litro o menos: '))
B = float(input('Insertar numero de botellas de un 1 litro o mas: '))
C = (1)
D = (2.5)
total = (A*C + B*D)
print(nombre_cliente,'se le va a pagar:', total, 'pesos')


6° Probar las operaciones que se pueden realizar en el lenguaje de python.

import math
a = float(input('Escriba un valor a la variable a: '))
b =  float(input('Escriba un valor a la variable b: '))
suma = a + b
resta = a - b
producto = a * b
cociente = a / b
residuo = a // b
resultado = a ** b
print ('La suma de a y b es: ', suma)
print ('La resta de a y b es: ', resta)
print ('La producto de a y b es: ', producto)
print ('La cociente de a y b es: ', cociente)
print ('La residuo de a dividido por b es: ', residuo)
print ('El resultado de a^b es: ', resultado)
print ('La log10 de a es: ', math.log(a))


7° Crear un programa que le pida al usuario insertar cuantas millas por galon puede recorrer un auto en
kilometros.

a = float(input('inserte cuantas millas por galon recorre por su auto: '))
b = 1.609
c = a * b
print ('su auto recorre: ', c, 'kilometros')


8° El usuario debe isertar el radio de un circulo, calcular su area para despues calcular el radio de una
esfera y al final conseguir su area.

a = float(input('Inserte el radio del circulo: '))
pi = 3.1416
area = pi * a * a
print('El area del ciculo es: ', area)
b = float(input('Inserte el radio de una esfera: '))
area_circulo = (4/3*pi)*b**3
print('El area de la esfera es: ', area_circulo)


9° Insertar un programa para calcular los segundos de los dias, horas y minutos y luego sumar la cantidad total
de segundos.

a = float(input('Inserte el numero de dias: '))
b = float(input('Inserte el numero de horas: '))
c = float(input('Inserte el numero de minutos: '))
d = float(input('Inserte el numero de dias: '))
ad = a * 86400
bd = b * 3600
cd = c * 60
total = ad + bd + cd + d
print('El tiempo total es de: ', total, 'segundos')


10° Insertar en el programa la longitud y la altura de un traingulo y obtener el area.

ExamenC_Ejercicio1
Area de un triangulo

b = float(input('Insertar la longitud de la base del triangulo: '))
h = float(input('Insertar la altura del triangulo: '))
area = b * h / 2
print('El area del triangulo es: ', area)


11° Insertar en el programa el radio y la altura del cilindro y calcular su volumen en
decimales.

ExamenC_Ejercicio2
Cilindro

a = float(input('Insertar el radio del cilindro: '))
b = float(input('Insertar la altura del cilindro: '))
pi = 3.1416
volumen = pi*a**2*b
print('El volumen del clindro es: ', volumen, 'decimales')


# Sistemas condicionales

Si un programa no fuera mas que una lista de ordenes a ejecutar de forma secuencial, una por una, no tendria
mucha utilidad. Las condicionales no permiten comprobar condiciones y hacer que nuestro programa se comporte
de una formau otra, que ejecute un fragmento de codigo u otro, dependiendo de esta condicion, aqui es donde
cobran su importancia el tipo boliano y los operadores logicos.

# Condicional "if"

La forma mas simple de una setencia condicional es el "if" (del ingles si) seguido de la condicion a evaluar,
dos puntos (:) y en la siguiente linea e indentado el codigo a ejecutar en caso de que se cumpla dicha condicion.

else: codigo a ejecutar en caso de que la condicion sea falsa
variante "if"...else
mantener 2 resultados

if comparacion 1:
    codigo de la comparacion 1

elif comparacion 2:
    codigo de la comparacion 2

elif comparacion 3:
    codigo de la comparacion 3

else
en caso de que las comparaciones, de arriba no sean ciertas


# Ciclo for...in

Se utiliza de forma generica de iterar sobre una frecuencia es decir recorrer una secuencia.

secuencia = ["uno", "dos", "tres"]
for elemento in secuencia:
    print(elemento)


12° Escribe un programa que dspliegue una tabla de conversion de temperaturas para celsius y grados
farengei, la tabla debe contener filas para todas las temperaturas desde 0 a 100 °C, en multiplos de 10 grados
celsius.

for celsius in range (0,101,10):
    farenheit = 1.8 * celsius + 32
    print(celsius, 'gC', '|', farenheit, 'gF')


13° Escribe un programa que repita la palabra "miau" y "guau" cierto numero de veces.

def ladra(num_veces):
    i=0
    while i < num_veces:
        print('guau, guau')
        i = i + 1

def maulla():
    print('miau, miau')

cuerpo principal del programa
ladra(5)
maulla()


14° Escribir un programa que calcule el area de los triangulos.

def areatriangulo(base, altura):
    return (base * altura)/2

cuerpo principal del programa

area1 = areatriangulo(2.4, 4.3)
area2 = areatriangulo(5.4, 3.2)
area3 = areatriangulo(5.4, 4.2)
print('el area es: ', area)


# Bucles

Mientras que las condicionales permiten ejecutar distintos fragmentos de codigo dependiendo de ciertas
condiciones, los bucles permiten ejecutar un mismo fragmento de codigo un cierto numero de veces mientras se
cumpla una determinada condicion.

# While

El bucle "while" (mientras) ejecuta un fragmento de codigo mientras se cumpla la condicion. El bucle while
tiene la siguiente estructura:
while condicion : 
    fragmento de codigo que se repite

# Funciones

una funcion es un fragmento de codigo con un nombre asociado que realiza una serie de tareas y devuelve un
valor ademas de ayudarnos a programar y depurar dividiendo el programa en partes ademas las funciones tambien permiten 
reutilizar otros codigos.
Las funciones ayudan al programador a dividir un problema en pequeñas piezas que pueden ser reusados, tambien ayudan 
al programador a concentrarse en una pequeña parte del programa a la vez como resultado es una parte importante del
desarrollo. En nuestro caso debemos aprender a definiendo una funcion para usarla despues.
Pasar uno o mas valores a una funcion.
Desarrollar un calculo complejo en una funcion.
Regresar uno o mas resultados a una funcion.
Llamar una funcion previamente ya hecho.


15° Escribe un programa que le pida al usuario su edad siendo menor que 19 el numero que se tiene que colocar.

edad = 0
while edad < 19:
    print('Tienes ', edad)
    edad = edad + 1

print('Fin del programa')


16° Escribe un programa que le pida al usuario insertar un numero cualquiera y este le indique si es un numero par 
o impar.

numero = int(input('Inserte un numero: '))
if numero%2==0:
    print('El numero es par')
else:
    print('El numero es impar')


17° Escribe un programa que le pida al usuario que inserte un nuevo password y confirme este, si pone algo diferente
a lo solicitado sea marcado el error.

password_user1 = input('Inserte un nuevo password: ')
password_user2 = input('Confirme su password: ')

if password_user1 == password_user2:
    print('Su password ha sido establecido')
else:
    print('Lo siento, ha introducido mal los datos')


18° Escribe un programa que le solicite al usuario insertar la masa y la altura, despues que calcule 
el IMC y con respecto al resultado que salga marque si tiene delgadez severa, delgadez moderada, delgadez leve, 
tiene el IMC correcto, tiene preobesidad y obesidad leve.  

calculo del indice de masa corporal

masa = float(input('Introduce tu peso en kg: '))
altura = float(input('Introduce tu altura en metros: '))

imc = masa/altura**2

if imc < 16: 
    print('Tienes delgadez severa')
elif imc >= 16 and imc < 17:
    print('Tienes delgadez moderada')
elif imc >= 17 and imc < 18.5:
    print('Tienes delgadez leve')
elif imc >= 18.5 and imc < 25:
    print('Tienes el IMC correcto')
elif imc >= 25 and imc < 30:
    print('Tienes preobesidad')
elif imc >= 30 and imc < 35:
    print('Tienes obesidad leve')


Sentencias "if"


19° Escribe un programa que usando los valores de "x" y "y" cree una grafica.

import numpy as np
import matplotlib.pyplot as plt
x = np.arange(100)
y = np.sin(x)
graficando
plt.plot (x,y)
plt.show () 


20° Escribe un programa que a traves de los valores dados para seno, coseno y tangente, se cree una 
grafica y si se usan otros valores, salga la respuesta de 'No hay resultado'.

import numpy as np
import matplotlib.pyplot as plt
opcion=int(input('Introduzca 1 para Seno, 2 para Coseno y 3 para Tangente (para graficar)'))
x=np.arange(100)
if opcion == 1:
    y=np.sin(x)
elif opcion == 2:
    y=np.cos(x)
elif opcion == 3:
    y=np.tan(x)
else:
    print ('No hay resultado')
plt.plot(x,y)
plt.show()


21° Escribe un programa que le solicite al usuario calcular el precio final con el 60% descuento.


for precio_original in range (4,201,5):
    precio = (precio_original + 0.95)
    descuento = 60
    precio_final = precio * 60/100
    print(precio, '|', descuento, '|', precio_final)


22° Escribir un programa que le solicite al usuario calcular una tabla hasta un rango especificado. 

for tabla in range (1,11):
    a = tabla * 1
    b = tabla * 2
    c = tabla * 3
    d = tabla * 4
    e = tabla * 5
    f = tabla * 6
    g = tabla * 7
    h = tabla * 8
    i = tabla * 9
    j = tabla * 10
    print(a, '|', b, '|', c, '|', d, '|', e, '|', f, '|', g, '|', h, '|', i, '|',j)


23° Escribe un programa que calcule la tarifa de un taxi, pidiendole al usuario que inserte los kilometros
recorridos y calcularlo para obtener el precio.

def tarifa (kilometro):
    tarifa = 7 * kilometros + 7.25
    if tarifa < 40: 
        return 40
    return tarifa
kilometros = float(input('Inserte los kilometros recorridos: '))
precio = tarifa(kilometros)
print ('El precio es de' , precio )


24° Escribir un programa que le pida al usuario insertar el numero de productos y calcule su envio y precio. 

def envio(producto):
    envio= (producto-1)*45+150
    return envio


producto=int(input('ingrese el numero de productos: '))
precio=envio(producto)
print(precio)


25° Escribir un programa que le pida al usuario insertar el rango y que el programa le de numeros impares como 
resultado.

for numero in range (2,201,2):
    numeros_impares = (numero - 1)
    print(numeros_impares)


26° Escribir un programa que le pida al usuario insertar un numero aleatorio, tratando de adivinar el numero correcto, 
si acierta el programa le dira "lo lograste has adivinado", si el numero insertado es menor o mayor que el correcto se le 
notificara al usuario.

print('Adivina adivinador')
numero_correcto = 2345:
juego = input('Inserte el numero:')

if juego == numero:
    print('Lo lograste has adivinado :v ')
elif juego > numero:
    print('Tu numero es menor que el numero correcto :o ')
elif juego < numero:
    print('Tu numero es mayor que el numero correcto :o ')


Hay modulos en python que proveen caracteristicas poderosas que podemos usar en nuestros
programas. Algunos de estos pueden enviar correos electronicos y algunos extraen informacion
de paginas de internet para el manejo de graficos usaremos un modulo que permite crear figuras 
sin patrones.
El modulo que se usara desarrollar nuestro pensamiento computacional.


27° Escribe un programa que le crea una ventana en blanco junto a un objeto llamado "turtle", 
este se movera avanzara hacia adelante, dara media vuelta a la izquierda y nuevamente hacia delante 
finalizando con cerrar la ventana.

import turtle
Crea una ventana en blanco
ventana = turtle.Screen()
Crea un objeto de la clase turtle
alex = turtle.Turtle()
 A vanza 30 unidades
alex.forward(50)
Gira a la izquierda 90 grados
alex.left(90)
 Avanza 30 unidades
alex.forward(30)
Hasta que el usuario cierre la ventana el programa termina
ventana.mainloop()


28° Se escribira un programa que cree una ventana en donde un objeto se movera hacia un lado.

import turtle

ventana = turtle.Screen()
ventana.setup(500,500)
ventana.tracer(0)
ventana.addshape("mario.gif")

mario = turtle.Turtle()
mario.speed(0)
mario.shape("mario.gif")
mario.penup()
mario.gota(-350, 0)

while True :
    ventana.update()
    mario.forward(0.01)


29° Se escribira un programa que creara una ventana y un objeto con una imagen, el cual se movera 
hacia el lado y se detendra justo antes de salir de la pantalla.

import turtle

ventana = turtle.Screen()
ventana.setup(500,500)
ventana.tracer(0)
ventana.addshape("unicornio.jpg")

unicornio = turtle.Turtle()
unicornio.speed(0)
unicornio.shape("unicornio.gif")
unicornio.penup()
unicornio.gota(-350, 0)

while True :
    ventana.update()
    unicornio.forward(0.01)


30°  Se escribira un programa que creara una ventana y un objeto con una imagen, el cual se movera 
hacia el lado y al llegar rebotara con el borde de la pantalla, cambiando su direccion.

import turtle

ventana = turtle.Screen()
ventana.setup(500,500)
ventana.tracer(0)
ventana.addshape("estrella.gif")

estrella = turtle.Turtle()
estrella.speed(0)
estrella.shape("estrella.gif")

estrella.penup()
estrella.goto(-350, 0)

while True :
    ventana.update()
    estrella.forward(0.01)


31° Se escribira un programa, creando una ventana elijiendo su color, con un objeto con su propio
color que se movera y creara una figura.

import turtle
ventana = turtle.Screen()
ventana.bgcolor('lightgreen')
ventana.title('Hola, Jessie')

Jessie = turtle.Turtle()
Jessie.color('blue')
Jessie.pensize(3)
Jessie.forward(50)
Jessie.left(120)
Jessie.forward(50)

ventana.mainloop()


32° Se escribira un programa, creando una ventana elijiendo su color, con un objeto con su propio
color que se movera y creara una figura, finalizando con cerrar la ventana.

import turtle
ventana = turtle.Screen()
ventana.bgcolor('lightgreen')
ventana.title('Hola, Jessie')

Jessie = turtle.Turtle()
Jessie.shade('turtle')
Jessie.color('blue')
Jessie.pensize(3)
Jessie.forward(50)
Jessie.left(120)
Jessie.forward(50)

ventana.mainloop()


33° Se escribira un programa, creando una ventana eligiendo su color, con un objeto con su propios
colores cada vez que haga un trayecto que se movera y creara una figura de forma constante.

import turtle
m=input('inserte el color de la ventana')
ventana = turtle.Screen()
ventana.bgcolor('m')
ventana.title('Hola, Jessie')

Jessie = turtle.Turtle()
Jessie.color('blue, pink, red, darkgray, green, snow, brown, steel blue, red1, darkgreen')
Jessie.pensize(3)
Jessie.forward(50)
Jessie.left(120)
Jessie.forward(50)

ventana.mainloop()


# Programacion

Al principio del curso comentabamos que python es un lenguaje multiparadigma en el que se podia 
trabajar con programacion estructurada, como veniamos haciendo hasta ahora o con programacion
orientada en objetos el cual es un paradigma de programacion en el que en el que los conceptos 
del mundo real relevantes para nuestro problema se modelan atraves de clases y objetos, y del nuestro
programa consiste en una serie de interacciones de nuestro sistema.

# Clases y objetos

Un objeto es una entidad que agrupa un estado y una funcionalidad relacionada. El estado del objeto se 
define a traves de variables llamadas atributos, mientras que la funcionalidad se modela a traves de funciones
a las que se les conoce con el nombre de metodos del objeto.

Un ejemplo de objeto podria ser un coche en el que tendriamos atributos como la marca, el numero de puertas o el 
color, metodos de como arrancar y parar. O bien cualquier otra combinacion de atributos y metodos segun lo que 
fuera relevante para nuestro programa.

# Clases

Una clase no es mas que una plantilla generica de la cual instancia a los objetos. Es la plantilla que define que
atributos y metodos tendran los objetos de la clase. En python las clases se definen mediante la palabra clave 
"class" seguido del nombre de la clase, seguido ":" y a continuacion identado el cuerpo de la clase.
Class Automovil : 
def __init__(self, atributos1)
 self.atributo1 = atributo1
def arrancar(self)

