---
layout: post
title:  "Criptografía: Una Introducción posible"
categories: [ Articulos ]
author: DrNykterstein
image: assets/images/criptografia-intro/1.png
tags: [ Criptografia, Articulos, Tecnologia]
---
### Introducción
Históricamente el ser humano siempre ha tenido la necesidad de mantener la privacidad de sus secretos y de sus comunicaciones, esto lo ha llevado a la búsqueda de diferentes mecanismos para lograrlo, en el caso de la información, si es transmitida por un canal inseguro, esta puede ser vista y modificada por manos indeseadas. Todas las técnicas y mecanismos que intentan asegurar la confidencialidad e integridad de la información que es transmitida por un canal es lo que se denomina como **criptografía**.

La palabra **criptografía** proviene del griego kryptós que significa oculto y graphé, de escritura. Por lo que su significado seria algo como “Escritura oculta”. Junto al criptoanálisis la criptografía es una rama de la **criptologia** y esta mediante métodos matemáticos tiene como objetivo proteger una información, mensaje o un archivo mediante el uso de un algoritmo de cifrado. De esta forma asegurar la autenticidad, confidencialidad e integridad del mensaje.

<p align="center">
<img src="../assets/images/criptografia-intro/2.jpg">
</p>

### ¿Qué es el Cifrado?
El **cifrado** es la principal aplicación de la **criptografía** y se podría definir como un proceso que codifica un mensaje mediante la utilización de un algoritmo y solo se podría descifrar mediante una clave especial. Evitando de esta forma que si la información cae en manos de terceros, estos puedan entenderla ( A menos que tengan la clave que fue usada para cifrar). Ya en este punto podemos hablar de **criptografía simétrica** y **criptografía asimetrica**.

<p align="center">
<img src="../assets/images/criptografia-intro/3.png">
</p>

### ¿Qué es la criptografía simétrica?
La **criptografía simétrica** es aquella en que solo utiliza una clave secreta ,tanto para cifrar como para descifrar el mensaje. Es decir que cada participante en una comunicación secreta dispone de la misma clave y es aquí donde radica su problema, en la distribución de claves. La clave se tiene que intercambiar por un canal seguro para evitar que sea interceptada, pero **¿Qué canal es seguro para compartir la clave secreta?**.

La seguridad del cifrado **no debe depender de mantener el secreto del algoritmo, debe depender es de la clave secreta usada para el cifrado**. Por lo que esta debe ser compleja y de longitud elevada para evitar los ataques de fuerza bruta y tanto el emisor como el receptor la deben de mantener en secreto. Por poner un ejemplo, el algoritmo de cifrado simétrico DES (Data Encription Standard o Estándar de Encriptación de Datos) usa una clave de 56 bits, lo que significa un número de 72.057.594.037.927.936 claves posibles , por supuesto que para una persona probar todas estas posibilidades resulta imposible, pero hoy en día existen ordenadores con la capacidad de probarlas todas en tan solo unas horas. Por esta razón este algoritmo ya esta en desuso

<p align="center">
<img src="../assets/images/criptografia-intro/4.png">
</p>

Sin lugar a dudas este tipo de **criptografía** fue de utilidad en entornos militares y políticos, inclusive la máquina enigma usaba un método simétrico pero debido a la expansión del Internet y a los problemas que esta generaba, se avanzo hacia la **criptografia asimétrica**.

# ¿Qué es la criptografía asimétrica?
La **criptografía asimétrica** también conocida como **criptografía de clave pública** es la que permite solucionar el problema de distribución de clave a través de un canal completamente público. Este sistema se usan dos claves, la pública, que se puede compartir con cualquier persona y publicar en cualquier parte y la **privada**, que nunca jamas se debe compartir y esta vinculada con la pública.

En el caso de que queramos que nos envíen un archivo cifrado, debemos enviar nuestra clave pública para que cifren el archivo y de esta manera nos lo enviaran de forma confidencial y solo se podrá descifrar con la clave privada.

<p align="center">
<img src="../assets/images/criptografia-intro/5.png">
</p>

Este sistema se compone en la **factorización de números primos**, la clave pública contiene un número compuesto de dos números primos muy grandes. A la hora de cifrar un mensaje, el algoritmo usa el número compuesto para cifrarlo y para descifrar el mensaje el algoritmo requiere saber los factores primos y uno de esos factores se encuentra en la clave privada. Podemos pensar que con los equipos actuales podemos averiguar la clave privada de alguien sabiendo su clave pública. Pero realizar algo así seria bastante complicado, porque dado un número compuesto debemos factorizarlo para conocer cada uno de los dos números, además debemos decir que una clave privada y pública pueden tener un tamaño de 2048 bits, por lo que es imposible realizar un ataque de fuerza bruta sobre ellas.

### Conclusión
La **criptografía** ha sido usada a lo largo de la historia, desde **la escítala espartana** pasando por Julio Cesar que la usaba para comunicarse con sus generales y llegando hasta la actualidad, donde ya no es solamente usada en el ámbito militar y por los gobiernos, sino que es usada a diario por la sociedad.

Esta ciencia ha venido apoyando el avance del Internet y la podemos encontrar en diversas partes, como en los certificados digitales, las firmas electrónicas y gracias a ella podemos realizar transacciones (por dar un simple ejemplo). Pero más allá de eso, **la criptografía se ha convertido hoy en día en la única arma con la que podemos defender nuestro derecho a la privacidad**.
