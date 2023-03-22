---
title: INTRODUCCIÓN A RASPBERRY PI PICO
date: 2023-03-22 15:30:00 +0100
categories: [RASPBERRY PI, PICO]
tags: [RASPBERRYPIPICO PICO RASPBERRY]     # TAG names should always be lowercase
---

## ¿QUÉ ES RASPBERRY PI PICO?

Raspberry Pi Pico es una placa de desarrollo, la cual integra el primer microcontrolador creado por la fundación Raspberry Pi. Se trata de una placa de precio reducido, enfocada a diseños de sistemas embebidos, tanto en el ámbito industrial como en el ámbito personal.

<img src="https://assets.raspberrypi.com/static/hero-desktop-0be741ca0b96c13025520975475b902c.png">

Podríamos decir, que se trata de una placa muy similar a un Arduino y en cierto modo, es ciero, pero también cuenta con una gran diferencia frente a un Arduino Uno, que es a lo que la gran mayoría está acostumbrado. Esta placa cuenta con un microcontrolador ARM, en concreto un Cortex M0+, el cual cuenta con dos núcleos y 264kB de memoria RAM. Puede parecer muy poco en comparación a un ordenador común, pero tenemos que tener en cuenta que estamos ante un microcontrolador más pequeño que muchas monedas.

Toda esta información de golpe puede ser bastante abrumadora, así que vamos a organizar las ideas y ataquemos esta placa por varios puntos.

## ¿QUÉ ES UN MICROCONTROLADOR?

Según [Wikipedia](https://es.wikipedia.org/wiki/Microcontrolador):

>Un **microcontrolador** (abreviado µC, UC o mCU) es un circuito integrado programable, capaz de ejecutar las órdenes grabadas en su memoria. Está compuesto de varios bloques funcionales que cumplen una tarea específica. Un microcontrolador incluye en su interior las tres principales unidades funcionales de una computadora: unidad central de procesamiento, memoria y periféricos de entrada/salida.

Parece bastante complejo de entender, así que vamos a intentar interpretarlo con **nuestras palabras**. 

>Un **microcontrolador** es un "chip" que posee todos los componentes básicos para formar un ordenador, los cuales son: un procesador, un sistema de memoria, puertos de entrada/salida y un bus que interconecte todos los elementos. 

Si nos ponemos a pensarlo, el dispositivo desde el que estamos leyendo esto integra todos estos componenes. Tanto si estamos en un ordenador o en un teléfono móvil, ambos cuentan con un procesador principal, un sistema de memorias y puertos de entrada salida, que en estos casos corresponderán a los puertos USB y similares. Pero en un microcontrolador, todo esto se encuentra en un único chip.

<img src="https://www.golem.de/2106/156966-276138-276137_rc.jpg"/>
<br>
<br>

## HARDWARE Y PRECIO

Como hemos comentado anteriormente, la principal característica diferenciadora de esta placa es que cuenta con un procesador ARM. El procesador es el primer procesador que ha desarrollado la [Fundación Raspberry Pi](https://www.raspberrypi.com/), concretamente su nombre es [RP2040](https://www.raspberrypi.com/products/rp2040/).

Poniéndonos técnicos y extrayendo la información que nos aporta el fabricante acerca de este dispositivo, encontramos la siguiente información:

- Factor de forma: 21 mm × 51 mm
- Microcontrolador RP2040 diseñado por Raspberry Pi
- Procesador Dual-core Arm Cortex-M0+, con un reloj que llega hasta 133 MHz
- 264kB on-chip SRAM
- 2MB on-board QSPI flash
- 2.4GHz 802.11n wireless LAN (Solo disponible para las Raspberry Pi Pico W y Pico WH)
- 26 pines GPIO, incluyendo 3 pines analógicos
- 2 × UART, 2 × controladores SPI, 2 × controladores I2C, 16 × canales PWM 
- 1 × controlador USB 1.1 y PHY, con soporte para Host y Device
- 8 × Programable I/O (PIO) maquinas de estado para soporte customizado de perifericos
- Soporta un voltaje de entrada de 1.8–5.5V DC
- Temperatura de operación -20°C to +85°C (Raspberry Pi Pico y Pico H); -20°C to +70°- C (Raspberry Pi Pico W y Pico WH)
- Modo de programación "Arrastrar y soltar" mediante conexión USB 
- Modos de bajo consumo
- Reloj on-chip de precisión
- Sensor de temperatura
- Librerias de operaciones matemáticas aceleradas on-chip

Como podemos ver, son muchas las características con las que cuenta esta placa, las cuales son muy prometedoras por el precio y tamaño que tiene, ya que su precio se encuentra en torno a los 4 euros en su [versión normal](https://www.tiendatec.es/raspberry-pi-pico/1371-raspberry-pi-pico-5056561801445.html) y en torno a los 7 euros en su [versión Wi-Fi](https://www.tiendatec.es/raspberry-pi-pico/1918-raspberry-pi-pico-w-5056561803173.html).


## PROGRAMACIÓN

Un aspecto bastante resaltable es su forma de programación y facilidad. Esta placa puede ser programada utilizando dos leguajes diferentes: [C/C++](https://visualstudio.microsoft.com/es/vs/features/cplusplus/) y [MicroPython](https://micropython.org/). 

La forma de cargar el programa en la placa es muy sencilla, no necesitamos la ayuda de programadores externos como sí ocurre con otras familias como por ejemplos las placas [ST](https://www.st.com/content/st_com/en.html). El sistema que utilizan para programarse es mediante un archivo UF2, el cual debemos copiar a la placa una vez conectada al ordenador y ¡listo!, tendremos nuestra Pico programada.

En una futura publicación de este blog veremos cómo desplegar un entorno de programación para esta placa, además del proceso de programación dependiendo del lenguaje que queramos utilizar.

## CONCLUSIONES

Desde mi punto de vista, considero que estamos ante una placa con mucho potencial, tanto por su relación potencia/tamaño como por su precio. Es una placa que cualquier persona puede permitirse y que abre un sin fin de posibilidades, al igual que ocurre con Arduino, solo que con esta podemos ir un paso más allá al contar con un procesador ARM.

He comenzado algunos proyectos con ella, ya que la verdad es que me ha encantado desde la primera vez que la vi. Es cierto que es algo compleja de programar, sobre todo al principio si nunca has utilizado compiladores manualmente, pero una vez que sabes exprimir sus capacidades, puedes hacer cualquier cosa que te propongas.

## DOCUMENTACIÓN

**Raspberry Pi Pico DataSheet:** https://datasheets.raspberrypi.com/pico/pico-datasheet.pdf<br>
**Raspberry Pi Pico product Brief:** https://datasheets.raspberrypi.com/pico/pico-product-brief.pdf<br><br>
**Raspberry Pi Pico W DataSheet:** https://datasheets.raspberrypi.com/picow/pico-w-datasheet.pdf<br>
**Raspberry Pi Pico W product Brief:** https://datasheets.raspberrypi.com/picow/pico-w-product-brief.pdf<br><br>
**Raspberry Pi Pico C/C++ SDK:** https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-c-sdk.pdf<br>
**Raspberry Pi Pico Python SDK:** https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-python-sdk.pdf