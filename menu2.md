+++
title = "Protoboard"
hascode = true
date = Date(2023, 2, 06)
rss = "Una protoboard es una placa de pruebas que se utiliza para probar y desarrollar circuitos electrónicos. Permite la creación temporal de circuitos sin tener que soldar los componentes en una placa definitiva."

tags = ["Protoboard", "Arduino"]
+++


# La Protoboard

Los circuitos empleados durante el curso serán montados sobre una **protoboard**, la cual es un dispositivo que nos permite completar circuitos de manera temporal, sin necesidad de recurrir a soldaduras.

\toc

## Función de las protoboards

Las **protoboards** son herramientas esenciales para cualquier persona que trabaje con electrónica. Son un medio eficaz para **probar** y desarrollar circuitos electrónicos antes de producirlos a gran escala. Estas placas tienen un patrón de agujeros y pistas que permiten conectar componentes electrónicos con cables temporalmente, lo que las hace ideales para la **creación temporal de circuitos** sin tener que soldar los componentes en una placa definitiva.

Además, las protoboards son fáciles de usar y no requieren ningún tipo de habilidad de soldadura. Pueden ser utilizadas para probar diferentes configuraciones de circuitos y hacer ajustes hasta que se logre el resultado deseado. También son **útiles para la educación** y el aprendizaje de electrónica, ya que permiten experimentar con diferentes componentes y ver cómo interactúan entre sí.

## Conexiones en Protoboard

![Protoboard](/protoboard.png)

Se puede diferenciar dos zonas principales de la protoboard, las cuales presentan formas de conexión diferentes:

* La zona de los extremos superiores e inferiores (la que tiene los símbolos + y -) son los buses de alimentación.
* La zona central, cuyas posiciones se caracterizan por una letra y un número (ejemplo: posición g23).

### Buses de alimentación

Las conexiones en los buses de alimentación se llevan a cabo de manera longitudinal, como se representa mediante las lineas de color rojo. Varios dispositivos que se encuentren introducidos en la misma linea longitudinal, estarán conectados mutuamente.

![Conexión en los buses de alimentación](/buses.png)

### Zona central

Las conexiones en la zona central se llevan a cabo de manera transversal, como se representa mediante las lineas de color azul. Varios dispositivos que se encuentren introducidos en la misma linea transversal, estarán conectados mutuamente.

![Conexión en la zona central](/central.png)

## Conexiones de ejemplo

Para verificar si se han adquirido los conocimientos sobre las conexiones en protoboard, se va a proponer dos ejemplos de conexiones que deberán realizarse en la protoboard. Es recomendable intentarlo y luego visualizar el resultado (los resultados pueden variar, ya que las celdas seleccionadas de la protoboard no tienen por que coincidir).

### Ejemplo 1: Circuito RLC en serie

Los circuitos RLC son circuitos electrónicos que combinan resistencias (R), inductancias (L) y capacitores (C) en un sistema. A continuación se muestra un esquema del circuito.

![Circuito RLC](/RLC.png)

Ahora, trate de recrear este circuito utilizando una protoboard. Puede realizarlo de manera digital visitando la web de [Tinkercad](https://www.tinkercad.com). A continuación, se muestra la solución en una protoboard.

![Circuito RLC resuelto](/solucion_RLC.png)

### Ejemplo 2: Resistencias en paralelo

Las conexiones de componentes electrónicos en paralelo supone un nivel de dificultad alto para las personas completamente novatas, no obstante, es de vital importancia saber llevarlas a cabo. Tómese su tiempo. El circuito a recrear en una protoboard es el siguiente.

![Circuito paralelo](/paralelo.png)

Ahora, trate de recrear este circuito utilizando una protoboard. Puede realizarlo de manera digital visitando la web de [Tinkercad](https://www.tinkercad.com). A continuación, se muestra la solución en una protoboard.

![Circuito paralelo resuelto](/solucion_paralelo.png)
