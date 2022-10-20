# Entrega Laboratorio 4

El laboratorio No. 4 tiene como objetivo manipular el robot Phantom X Pincher, inicialmente mediante Dynamixel Wizard y poteriormente usando ROS y codificando las posiciones en Matlab o Python.

## Autores

- [Wilder Ofrey Bello Herrera](https://github.com/WilderBello)
- [Javier Eduardo Gutierrez Serrano](https://github.com/jaegutierrezser)

## Solución

## Mediciones

Para la implementación del laboratorio, realizaron las mediciones de longitudes de cada eslabón para posteriormente obtener el diagrama del robot y los parámetros DH, contrastando con los valores obtenidos del datasheet del fabricante del manipulador.

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/MatLab/Imagenes/Space_Work.png)

Con estos datos se procede a determinar los marcos y parámetros del manipulador de acuerdo con la convención Denavit-Hartenber estandar.

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/MatLab/Imagenes/Marcos_DH.png)

- Parámetros DH

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/MatLab/Imagenes/DH.png)

También se obtuvo el diagrama simulado en Matlab haciendo uso del Toolbox de Peter Corke:

- Posición 1: 0, 0, 0, 0, 0

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/MatLab/Imagenes/Posicion_N%C2%B001.png)

- Posición 2: -20, 20, -20, 20, 0

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/MatLab/Imagenes/Posicion_N%C2%B002_1.png)
![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/MatLab/Imagenes/Posicion_N%C2%B002_2.png)

- Posición 3: 30, -30, 30, -30, 0

![]()

- Posición 4: -90, 15, -55, 17, 0

![]()

- Posición 5: -90, 45, -55, 45, 10

![]()

## ROS

Para implementar cada una de las posiciones propuestas por la guía, se ubicó inicialmente el robot haciendo uso de Dynamixel Wizard para así corroborar que dichas posiciones fueran alcanzables, dada la posición HOME como el robot en vertical:

- Posición 1: 0, 0, 0, 0, 0

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Wizard1.png)

- Posición 2: -20, 20, -20, 20, 0

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Wizard2.jpg)

- Posición 3: 30, -30, 30, -30, 0

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Wizard3.jpg)

- Posición 4: -90, 15, -55, 17, 0

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Wizard4.jpg)

- Posición 5: -90, 45, -55, 45, 10

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Wizard5.jpg)

Mediante la codificación en Python en cada uno de los puntos anteriormente dados, se realizó la implementación de cada posición de manera espaciada para poder observar correctamente el movimiento, el código utilizado es el siguiente:

- Para ejecutar correctamente el programa se utilizaron los comandos dados en (![comandos para ROS](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Codigo/comandos.txt)).

- Se modificó el archivo basic.yaml para que ROS reconociera cada una de las articulaciones (![ver código](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Codigo/basic.yaml)).

- Se agregaron las posiciones necesarias mediante comentarios para poder enviar cada posición a la vez (![ver código en Python](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Codigo/jointPub.py)).

La implementación del código se puede observar en el video:

[![Ver el video](https://drive.google.com/file/d/1QhI-nAJg5XgqxbzmVyoA0x-kBUTsYf57/view?usp=sharing)](https://drive.google.com/file/d/1QhI-nAJg5XgqxbzmVyoA0x-kBUTsYf57/view?usp=sharing)

[Implementación del código](https://www.youtube.com/watch?v=MV9ingfI5bI&ab_channel=JavierEduardoGutierrezSerrqno)
# [![Alt text](https://img.youtube.com/vi/MV9ingfI5bI/0.jpg)](https://www.youtube.com/watch?v=MV9ingfI5bI)

