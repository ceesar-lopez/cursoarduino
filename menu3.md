+++
title = "Pines Arduino"
hascode = true
rss = "A short description of the page which would serve as **blurb** in a `RSS` feed; you can use basic markdown here but the whole description string must be a single line (not a multiline string). Like this one for instance. Keep in mind that styling is minimal in RSS so for instance don't expect maths or fancy styling to work; images should be ok though: ![](https://upload.wikimedia.org/wikipedia/en/b/b0/Rick_and_Morty_characters.jpg)"
rss_title = "More goodies"
rss_pubdate = Date(2023, 2, 7)

tags = ["pin", "Digital", "Analógico"]
+++

# Pines de Arduino

Empleando los pines de Arduino se establecen las conexiones con dispositivos externos. Mediante estos dispositivos se puede recibir información del exterior, a traves del uso de sensores, o realizar una acción, empleando actuadores. En función de este criterio, los pines se clasifican como de entrada o de salida. A su vez, en función del tipo de señales que procesa, se diferencian los pines de tipo digital o analógico.

\tableofcontents

## Pines de Entrada/Salida

Los pines de entrada y salida en Arduino son los puntos de conexión que permiten que la placa interactúe con el mundo exterior a través de sensores, actuadores y otros componentes electrónicos.

* Los **pines de entrada** se utilizan para recibir información desde sensores y otros dispositivos externos, como botones, interruptores, sensores de luz, etc. En la placa Arduino, estos pines pueden ser configurados como entradas digitales o analógicas, lo que permite detectar valores discretos o continuos, respectivamente.

* Los **pines de salida** se utilizan para controlar actuadores, pantallas, luces, motores, etc. Estos pines pueden ser configurados como salidas digitales o PWM (modulación por ancho de pulso), lo que permite enviar señales digitales de encendido y apagado o señales analógicas con una resolución de 8 bits.

Supongamos que queremos alimentar un LED utilizando el pin 3 de nuestro Arduino. El primer paso será declarar que ese pin va a funcionar como salida. El código que debemos escribir es el siguiente:

```c
void setup() {
  pinMode(3,OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
}
```

El comando debe estar incluido en el bloque setup, el cual se ejecuta una única vez. Ahora, supongamos que queremos recibir datos de un sensor utilizando el pin A2 de nuestra Arduino. Se deberá declarar que ese pin va a funcionar como entrada. El código que debemos escribir es el siguiente:

```c
void setup() {
  pinMode(A2,INPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
}
```
Los posibles comandos son dos, uno para entrada (`pinMode(pin,INPUT)`) y otro para salida (`pinMode(pin,OUTPUT)`). Si no te ha quedado claro o quieres reforzar los conocimientos aprendidos tienes este video a tu disposición:

~~~
<iframe width="654" height="368" src="https://www.youtube.com/embed/oJmi1o1Gr84" title="Pines de entrada y salida | Curso Arduino" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
~~~

## Pines digitales/analógicos

En Arduino, los pines pueden ser configurados como pines digitales o analógicos. Aquí hay una breve explicación de cada tipo de pines:

* Los **pines digitales** pueden ser configurados como entradas o salidas, y pueden leer o enviar señales binarias (0 ó 1, apagado o encendido). Los pines digitales pueden detectar solo dos valores posibles: LOW (0) y HIGH (1). Estos pines se utilizan con frecuencia para detectar la presencia o ausencia de una señal, como un botón presionado o no presionado.

* Los **pines analógicos** pueden ser configurados como entradas o salidas, y pueden leer o enviar señales con una amplia gama de valores. Los pines analógicos se utilizan con frecuencia para leer sensores que proporcionan valores continuos, como sensores de luz, temperatura, humedad, etc. La placa Arduino cuenta con un conversor analógico-digital (ADC) que permite leer valores analógicos y convertirlos en valores digitales para su uso en el software.

Es importante tener en cuenta que los pines digitales solo pueden detectar y enviar señales binarias, mientras que los pines analógicos pueden detectar y enviar señales con una amplia gama de valores. Esto significa que los pines analógicos son más flexibles y pueden ser utilizados para una amplia variedad de aplicaciones, mientras que los pines digitales son más adecuados para aplicaciones que requieren una detección binaria.

Los posibles comandos a emplear son el de establecer un pin digital como salida (`digitalWrite(pin,HIGH/LOW)`) o entrada (`digitalRead(pin)`), y el de establecer un pin analógico como de salida (`analogWrite(pin,0-1023)`) o entrada (`analogRead(pin)`). A continuación se muestra un ejemplo del pin 3 alimentando un LED con 5 voltios.

```c
void setup() {
  pinMode(3,OUTPUT);
}

void loop() {
  digitalWrite(3,HIGH);
}
```

Además, a continuación se muestra el ejemplo del PIN A2, de entrada, recibiendo datos analógicos de un sensor de luz.

```c
void setup() {
  pinMode(A2,INPUT);
}

void loop() {
  analogRead(A2);
}
```

Si no te ha quedado claro o quieres reforzar los conocimientos aprendidos tienes este video a tu disposición:

~~~
<iframe width="654" height="368" src="https://www.youtube.com/embed/SKliNIB5qiQ" title="Pines digitales analógicos | Curso Arduino" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
~~~

## Resumen

En Arduino, los pines se pueden clasificar como pines de entrada, salida, digitales o analógicos: 
* Los **pines de entrada** se utilizan para recibir información del mundo exterior a través de sensores y otros dispositivos electrónicos.
* Los **pines de salida** se utilizan para controlar actuadores y otros dispositivos externos.
* Los **pines digitales** pueden detectar solo dos valores posibles (0 ó 1) y se utilizan para detectar señales binarias, como un botón presionado o no presionado.
* Los **pines analógicos** pueden detectar una amplia gama de valores y se utilizan para leer sensores que proporcionan valores continuos, como sensores de luz, temperatura, humedad, etc. Juntos, estos pines permiten que la placa Arduino interactúe con el mundo exterior y realice una amplia variedad de tareas.
