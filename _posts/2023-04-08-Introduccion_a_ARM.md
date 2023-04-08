---
title: INTRODUCCIÓN A ARM
date: 2023-04-08 12:00:00 +0100
categories: [RASPBERRY PI, PICO]
tags: [RASPBERRYPIPICO PICO RASPBERRY ARM CHAT-GPT]     # TAG names should always be lowercase
---

<style> 
    table {
    text-align: left;
    }

    td[align="left"] {
    overflow-wrap: anywhere;
    word-break: break-all;
    }

    td[align="right"] {
    white-space: nowrap;
    }
</style>

## ¿Qué es la arquitectura ARM?
La arquitectura ARM es una de las arquitecturas de procesadores más utilizadas en la actualidad. Es la base de la mayoría de los dispositivos móviles y también se utiliza en muchos otros dispositivos, desde relojes inteligentes hasta servidores.

![Dispositivos móviles con arquitectura ARM](https://www.muycomputer.com/wp-content/uploads/2016/02/ARM.jpg)

Se trata de una arquitectura de procesador RISC (Reduced Instruction Set Computing), lo que significa que utiliza un conjunto reducido de instrucciones para hacer que el procesador sea más rápido y eficiente en términos de energía.

Los procesadores que utilizamos en ordenadores de escritorio, por el contrario utilizan una arquitectura de procesador CISC (Complex Instryction Set Computing), lo que significa que las instrucciones que utiliza para funcionar son complejas.

Cada una de estas arquitecturas posee una serie de ventajas e inconvenientes, dependiendo de la aplicación que se les vaya a otorgar. En la siguiente tabla podemos ver sus características resumidas:

| RISC | CISC |
| ---- | ---- |
| Es una arquitectura de conjunto de instrucciones complejas | Es una arquitectura con conjunto de instrucciones reducido |
| Hace hincapié en el hardware para optimizar el conjunto de instrucciones | Hace hincapié en el software para optimizar el conjunto de instrucciones |
| Unidad de microprogramación en el procesador | Es una unidad de programación cableada en el procesador |
| Requiere un único conjunto de registros para almacenar la instrucción | Requiere múltiples conjuntos de registros para almacenar la instrucción |
| Tiene una compleja decodificación de las instrucciones | Tiene una sencilla decodificación de las instrucciones |
| Los usos de la canalización son difíciles | Los usos de la canalización son simples |
| Utiliza una gran cantidad de instrucciones que requieren más tiempo para ejecutar las instrucciones | Utiliza un número limitado de instrucciones que requiere menos tiempo para ejecutar las instrucciones |
| Utiliza la instrucción LOAD y STORE en la interacción de memoria a memoria de un programa | Utiliza LOAD y STORE que son instrucciones independientes en el registro para registrar la interacción de un programa |
| Tiene transistores para almacenar instrucciones complejas | Tiene más transistores en registros de memoria |
| El tiempo de ejecución es mayor | El tiempo de ejecución es muy corto |
| Se puede utilizar con aplicaciones de alta gama como telecomunicaciones, procesamiento de imágenes, procesamiento de video, etc. | Se puede utilizar con aplicaciones de gama baja como domótica, sistema de seguridad, etc. |
| Tiene instrucciones de formato variable | Tiene instrucciones de formato fijo |
| Los programas escritos para esta arquitectura tienden a ocupar menos espacio en la memoria | El programa escrito para esta arquitectura necesita ocupar más espacio en la memoria |

## ¿Por qué se utiliza la arquitectura ARM?
La arquitectura ARM se utiliza en una amplia variedad de dispositivos debido a su eficiencia energética y su capacidad para procesar grandes cantidades de datos. Esto la convierte en una opción popular para dispositivos móviles y otros dispositivos que requieren una gran cantidad de procesamiento en un paquete pequeño.

## ¿Cómo funciona la arquitectura ARM?
La arquitectura ARM consta de varios componentes, incluidos el procesador, la memoria y los buses de datos. El procesador es el componente principal de la arquitectura ARM y es responsable de realizar las operaciones de procesamiento. La memoria es donde se almacenan los datos y las instrucciones que se utilizan para el procesamiento, y los buses de datos son los medios por los que se transfieren los datos entre los diferentes componentes.

## ¿Qué aplicaciones tiene la arquitectura ARM?
La arquitectura ARM se utiliza en una amplia variedad de aplicaciones, desde dispositivos móviles y wearables hasta servidores de alta gama. Además, la arquitectura ARM es la base de muchos sistemas embebidos, como los sistemas de control de vehículos y las cámaras de seguridad.

- **Dispositivos móviles**: Los procesadores ARM son ampliamente utilizados en dispositivos móviles como teléfonos inteligentes, tabletas y dispositivos portátiles. Empresas como Apple, Samsung y Qualcomm utilizan procesadores ARM en sus dispositivos móviles.

- **IoT y dispositivos integrados**: La arquitectura ARM también se utiliza en dispositivos IoT (Internet de las cosas) y en sistemas embebidos, que incluyen productos como sistemas de seguridad, sensores, cámaras de vigilancia, entre otros.

- **Servidores**: La arquitectura ARM también se está utilizando cada vez más en servidores, especialmente en centros de datos y en la nube, debido a su eficiencia energética y su capacidad para manejar grandes cargas de trabajo.

- **Automoción**: Los procesadores ARM también se utilizan en sistemas de infoentretenimiento en el automóvil, así como en sistemas avanzados de asistencia al conductor y en otros sistemas de seguridad críticos.

- **Wearables**: La arquitectura ARM se utiliza en dispositivos portátiles como relojes inteligentes, rastreadores de actividad y otros dispositivos portátiles.

## Conclusión
La arquitectura ARM es una de las arquitecturas de procesador más importantes en la actualidad, gracias a su eficiencia energética y capacidad de procesamiento. Su capacidad para procesar grandes cantidades de datos en un paquete pequeño la hace una opción popular para dispositivos móviles y otros dispositivos que requieren un alto rendimiento en un espacio reducido.

Me gustaría reconocer el mérito del Chat-GPT ya que me ha ayudado a conseguir las imágenes y conexionarlas con el texto.