---
title: INTRODUCCIÓN A ARM
date: 2023-04-08 12:00:00 +0100
categories: [RASPBERRY PI, PICO]
tags: [RASPBERRYPIPICO PICO RASPBERRY ARM CHAT-GPT]     # TAG names should always be lowercase
---

## ¿Qué es la arquitectura ARM?
La arquitectura ARM es una de las arquitecturas de procesadores más utilizadas en la actualidad. Es la base de la mayoría de los dispositivos móviles y también se utiliza en muchos otros dispositivos, desde relojes inteligentes hasta servidores.

![Dispositivos móviles con arquitectura ARM](https://www.muycomputer.com/wp-content/uploads/2016/02/ARM.jpg)

Se trata de una arquitectura de procesador RISC (Reduced Instruction Set Computing), lo que significa que utiliza un conjunto reducido de instrucciones para hacer que el procesador sea más rápido y eficiente en términos de energía.

Los procesadores que utilizamos en ordenadores de escritorio, por el contrario utilizan una arquitectura de procesador CISC (Complex Instryction Set Computing), lo que significa que las instrucciones que utiliza para funcionar son complejas.

Cada una de estas arquitecturas posee una serie de ventajas e inconvenientes, dependiendo de la aplicación que se les vaya a otorgar. En la siguiente tabla podemos ver sus características resumidas:

<style> 
    table {
    border: 1px solid #ccc;
    width: 100%;
    margin:0;
    padding:0;
    border-collapse: collapse;
    border-spacing: 0;
  }

  table tr {
    border: 1px solid #ddd;
    padding: 5px;
  }

  table th, table td {
    padding: 10px;
    text-align: center;
  }

  table th {
    text-transform: uppercase;
    font-size: 14px;
    letter-spacing: 1px;
  }

  @media screen and (max-width: 600px) {

    table {
      border: 0;
    }

    table thead {
      display: none;
    }

    table tr {
      margin-bottom: 10px;
      display: block;
      border-bottom: 2px solid #ddd;
    }

    table td {
      display: block;
      text-align: right;
      font-size: 13px;
      border-bottom: 1px dotted #ccc;
    }

    table td:last-child {
      border-bottom: 0;
    }

    table td:before {
      content: attr(data-label);
      float: left;
      text-transform: uppercase;
      font-weight: bold;
    }
  }
</style>

<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">RISC</th>
    <th class="tg-0pky">CISC</th>
  </tr>
</thead>
<tbody>
  <tr>
<td>Es una arquitectura con conjunto de instrucciones reducido</td>
<td>Es una arquitectura de conjunto de instrucciones complejas</td>
</tr>
<tr>
<td>Hace hincapié en el software para optimizar el conjunto de instrucciones</td>
<td>Hace hincapié en el hardware para optimizar el conjunto de instrucciones</td>
</tr>
<tr>
<td>Es una unidad de programación cableada en el procesador</td>
<td>Unidad de microprogramación en el procesador</td>
</tr>
<tr>
<td>Requiere múltiples conjuntos de registros para almacenar la instrucción</td>
<td>Requiere un único conjunto de registros para almacenar la instrucción</td>
</tr>
<tr>
<td>Tiene una sencilla decodificación de las instrucciones</td>
<td>Tiene una compleja decodificación de las instrucciones</td>
</tr>
<tr>
<td>Los usos de la canalización son simples</td>
<td>Los usos de la canalización son difíciles</td>
</tr>
<tr>
<td>Utiliza un número limitado de instrucciones que requiere menos tiempo para ejecutar las instrucciones</td>
<td>Utiliza una gran cantidad de instrucciones que requieren más tiempo para ejecutar las instrucciones</td>
</tr>
<tr>
<td>Utiliza LOAD y STORE que son instrucciones independientes en el registro para registrar la interacción de un programa</td>
<td>Utiliza la instrucción LOAD y STORE en la interacción de memoria a memoria de un programa</td>
</tr>
<tr>
<td>Tiene más transistores en registros de memoria</td>
<td>Tiene transistores para almacenar instrucciones complejas</td>
</tr>
<tr>
<td>El tiempo de ejecución es muy corto</td>
<td>El tiempo de ejecución es mayor</td>
</tr>
<tr>
<td>Se puede utilizar con aplicaciones de gama baja como domótica, sistema de seguridad, etc.</td>
<td>Se puede utilizar con aplicaciones de alta gama como telecomunicaciones, procesamiento de imágenes, procesamiento de video, etc.</td>
</tr>
<tr>
<td>Tiene instrucciones de formato fijo</td>
<td>Tiene instrucciones de formato variable</td>
</tr>
<tr>
<td>El programa escrito para esta arquitectura necesita ocupar más espacio en la memoria</td>
<td>Los programas escritos para esta arquitectura tienden a ocupar menos espacio en la memoria</td>
</tr>
</tbody>
</table>

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