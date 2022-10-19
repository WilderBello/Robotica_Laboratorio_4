# Entrega Laboratorio 4

El laboratorio No. 4 tiene como objetivo manipular el robot Phantom X Pincher, inicialmente mediante Dynamixel Wizard y poteriormente usando ROS y codificando las posiciones en Matlab o Python.

## Autores

- [Wilder Ofrey Bello Herrera](https://github.com/WilderBello)
- [Javier Eduardo Gutierrez Serrano](https://github.com/jaegutierrezser)

## Solución

## Mediciones

Para la implementación del laboratorio, realizaron las mediciones de longitudes de cada eslabón para posteriormente obtener el diagrama del robot y los parámetros DH.

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Diagrama.jpg)
![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Parametros.jpg)

También se obtuvo el diagrama simulado en Matlab haciendo uso del Toolbox de Peter Corke:

![](https://github.com/WilderBello/Robotica_Laboratorio_4/blob/main/Imagenes/Diagrama_Matlab.jpg)

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

Mediante la codificación en Python en cada uno de los puntos anteriormente dados, se realizó la implementación de cada posición de manera espaciada para poder observar correctamente el movimiento, como se puede observar en el video:

[![Ver el video](https://drive.google.com/file/d/1QhI-nAJg5XgqxbzmVyoA0x-kBUTsYf57/view?usp=sharing)](https://drive.google.com/file/d/1QhI-nAJg5XgqxbzmVyoA0x-kBUTsYf57/view?usp=sharing)
