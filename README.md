# TP4

## Uso de Display. 

Utilizando un Arduino Nano (`atmega328p`), `1 display 7 seg` y `2 Pulsadores` se pide:

1. Realizar un contador de `0` a `9` en decimal que se incremente al presionar un **pulsador**. Mostrar
el resultado de la cuenta en un **display**.

2.  Agregar al problema anterior un **pulsador** que decremente el número.

> Nota: Todos los pulsadores `deben` tener habilitada la resistencia de `pull-up`.

> el incremento o decremento debe de producirse en una unidad por pulsación. Utilice `debouncing` 

> Conecte una resistencia a cada segmento del display.

---

## Para poder realizar el trabajo

Tener en cuenta que los displays pueden ser anodo o catodo común, esto deberá tenerse en cuenta
para conectar el común de los displays o bien a GND o bien a +Vcc para lograr el encendido.
Opcionalmente, se puede utilizar un `decodificador BCD a 7 segmentos`, **CD4511(CMOS)** o
**SN7447(TTL)**, esto simplifica la codificación pero aumenta la complejidad de el circuito.
## ¡USAR LOS PINES INDICADOS NO CAMBIARLOS!

``` C
PC0 -> BOTON 1 
PC1 -> BOTON 2 
PC2 -> BOTON 3 
PC3 -> BOTON 4

PD2 -> SEGMENTO A   
PD3 -> SEGMENTO B 
PD4 -> SEGMENTO C
PD5 -> SEGMENTO D 
PD6 -> SEGMENTO E 
PD7 -> SEGMENTO F
PB0 -> SEGMENTO G
PB1 -> SEGMENTO DP

```
## Pinout

![PINOUT](Arduino-Nano-Pinout.png "pinout")

## Circuito

![Circuito](circuito.png "circuito")