## Practica 4 

Castro Mejía Jonatan Alejandro

# UDP

![](https://github.com/jacs04x/Redes/blob/main/img/image-20220123212023861.png)

```markdown
Puerto de Origen

> Su longitud es de 16 bits
> Puerto que identifica como origen de envio de la aplicación

Puerto de Destino 
> Su longitud es de 16 bits
> Puesrto que se identifica como Destino o receptor de la aplicación

Longitud UDP 
> En el se define la longitud del datagrama. 
	Esta compuesta por:
	 > La longitud de la cabecera, la cual consta de 8 bytes,
	 > El tamaño de los datos.

Checksum
> Detecta errores o alteraciones durante la transmisión de los datos.
> Si detecta errores o alteraciones los paquetes "dañados" se descartan.

Para genera checksum son empleadas algunas partes de:
    > La cabecera UDP 
    > Los datos
    > La pseudocabecera (contiene información de la cabecera IP)
```

# TCP 

![](https://github.com/jacs04x/Redes/blob/main/img/image-20220123210145179.png)

```markdown
Puerto de origen
> Identifica el número de puerto de un programa de aplicación, siendo de origen.

Puerto de destino
> Identifica el número de puerto de un programa de aplicación, siendo destino.

Secuencia Numérica
> Especifica el número de secuencia del primer byte de datos de este segmento.

Número de reconocimiento
> Identifica la posición del byte más alto que se recibio.

DO (Desplazamiento de Datos)
> Especifica el desplazamiento de la parte de datos del segmento.

RSV (Reserva)
> Reservado para uso futuro.

Banderas
Bits de control para identificar la finalidad del segmento:
> URG
  El campo de puntero urgente es válido.
> ACK
  El campo de reconocimiento es válido.
> PSH
  El segmento solicita un PUSH.
> RTS
  Restablece la conexión.
> SYN
  Sincroniza los números de secuencia.
> FIN
  El remitente ha alcanzado el final de la corriente de bytes.
  
Ventana
> Especifica la cantidad de datos que el destino está dispuesto a aceptar.

Checksum
> Verifica la integridad de la cabecera y los datos de segmento.

Puntero urgente
> Indica datos que se deben entregar lo más rápidamente posible. Este puntero
  especifica la posición donde finalizan los datos urgentes.

Opciones
> Indica el final de la lista de opciones. Se utiliza en la opción final, no al final de cada
  opción individualmente. Sólo es necesario utilizar esta opción si el final de las
  opciones no coincidirá con el final de la cabecera TCP.
> No Operation (Sin operación) Indica cuales son los límites entre las opciones. 
	No existe ninguna garantía de que los remitentes vayan a utilizar esta opción, de modo que los destinatarios deben estar preparados para procesar opciones incluso aunque éstas no empiecen en un límite de palabra.
> Maximum Segment Size (Tamaño máximo de segmento) Indica cual es el tamaño máximo de segmento que TCP puede recibir. Esto sólo se envía en la petición de conexión inicial

```

# ICMP

![](https://github.com/jacs04x/Redes/blob/main/img/image-20220123213330135.png)

```markdown
Tipo 
```

![](https://github.com/jacs04x/Redes/blob/main/img/image-20220123213525373.png)

```markdown
Código 
> Subtipo al tipo solicitado o dado

Checksum
> Datos de comprobación de errores. 
Es Calculado a partir de la cabecera ICMP más los datos, con un valor de 0 para este campo.
```



