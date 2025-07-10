# examen

grupo-03

## Integrantes

- Sofía Cartes / [sofiacartes](https://github.com/sofiacartes)
- Isabella Gutiérrez / [isabellagutierrezm](https://github.com/isabellagutierrezm)
- Valentina Ruz / [vxlentiinaa](https://github.com/vxlentiinaa)

## Proyecto-02

- aprendizajes

Trabajo en equipo; el hacer y rehacer un circuito para lograr que funcione, paciencia,  potenciómetro de 1m ohm para regular las luces junto al de 500k

soldar

cómo interactúa el objeto con el espacio, ya que como grupo definimos que ciertos elementos sobresalen de la pcb para que el usuario interactúe con estos para que funcione tal como esperamos

elección de luces, material y refracción, interacción de la luz con distintos objetos.

- dificultades

que el circuito funcionara como queríamos, porque había veces que **funcionaba pero su sensibilidad no era la que necesitábamos** (poca sensibilidad).

probar distintos micrófonos y sus sensibilidades.

decisión de la forma de la carcasa

## PCB

Prototipado de circuitos en protoboard

- El circuito de entrada reacciona al sonido para medir la sensibilidad del micrófono, mediante un potenciómetro.
- El circuito de salida usa luces LEDS de colores para representar, y ver el sonido que entra en el circuito.
  
A continuación se presentan imágenes de las protoboards usadas.

![grupo03-pcb-1](./imagenes/protoboard/tme-grupo03-registro02.JPG)

![grupo03-pcb-1](./imagenes/protoboard/tme-grupo03-registro03.JPG)

![grupo03-pcb-1](./imagenes/protoboard/tme-grupo03-registro01.JPG)

![grupo03-pcb-1](./imagenes/protoboard/tme-grupo03-registro05.JPG)


A continuación se presentan imágenes de la PCB final.

![grupo03-pcb-1](./imagenes/pcb/tme-grupo03-pcb-registro01.JPG)

![grupo03-pcb-1](./imagenes/pcb/tme-grupo03-pcb-registro03.JPG)

![grupo03-pcb-1](./imagenes/pcb/tme-grupo03-pcb-registro07.JPG)

![grupo03-pcb-1](./imagenes/pcb/tme-grupo03-pcb-registro08.JPG)

![grupo03-pcb-1](./imagenes/pcb/tme-grupo03-pcb-registro11.JPG)

## Bill of Materials

| Componente    | Cantidad | Comentarios     |
| ------------- | -------- | --------------- |
| Resistencia   | 8        | 1k              |
| Resistencia   | 4        | 10k             |
| Resistencia   | 1        | 220             |
| Resistencia   | 2        | 22k             |
| Micrófono     | 1        | CZN-15E         |
| Condensador   | 2        | 10uF            |
| Condensador   | 1        | 1uF             |
| Diodo         | 2        | 1n5819          |
| Diodo         | 1        | 1n4007          |
| Potenciómetro | 1        | 1M Ohm          |
| Potenciómetro | 1        | 500k            |
| LED           | 6     | 5mm             |
| Chip          | 1        | LM324N          |
| Chip          | 1        | 4017            |
| Terminal block | 1        | 2 pin           |
| Switch        | 1        | spdt            |
| Bateria        | 1        | 9v              |  
|socket         | 1         |  14 pins |
|socket         |  1        | 16 pins  |
|terminal block | 1  | |
|pernos m2      |4     | |

- Los LEDS de 5mm son de **colores variados**  (verde, blanco, amarillo, rojo, azul)

## Esquemático

En el primer esquemático, es el del **Chip LM324,** donde conectamos primero el micrófono, luego mediante los condensadores **regulamos la sensibilidad** de este para que capte mejor los sonidos e incorporamos dos LEDS para ver si el circuito funciona correctamente, dentro de este, el potenciómetro nos da la posibilidad de que **elijamos la receptividad.**
En el segundo esquemático es la **secuencia/contador** de luces mediante el **Chip 4017**, donde el pin 14 va al pin 14 del LM324, lo cual nos da la posibilidad de tener una **frecuencia diferente de los cuatro LEDS** incorporados,y que esta **dependa del sonido emitido.**

DESCRIPCIÓN:

- **LM324** nos sirvió para **amplificar la señal emitida y poder regular la sensibilidad** de la recepción de los sonidos (micrófono)

CONEXIONES UTILIZADAS:

CHIP LM324

- pin 1 y 2 para la conexión con el potenciómetro la dos para la su pin central,  mientras la uno se dirige al condensador.

- pin 3 hacia dos resistencias de 10k, una hacia VCC y otra a GND.

- pin 4 a  VVC

- pin 5 a GND

- pin 6 va con una conexión al pin 1, pasando por la resistencia de 10k y el condensador de 1uF, anteriormente mencionados. También, está conectado al diodo 1N5819 en serie a la resistencia de 22k, intersectando con el pin 7 que está conectado al diodo 1N5819, siguiendo a la resistencia de 220, al condensador de 10uF, resistencia 10k, llegando al pin 10.

- pin 9 se dirige a la resistencia de 1k, conectando con el pin 8 dirigiéndose a GND por medio una resistencia de 1k y un LED. De igual manera, la conexión anterior pasa por el pin 12.

- pin 13, está conectado al pin central de un potenciómetro de 500k y sus otros pines uno a VVC y otro a GND.

- pin 14 hacia GND, mediante una resistencia de 1k y al LED.

CHIP 4017

- Nos sirvió para hacer la **secuencia de luces** con un reset por cada beat.

- Desde el pin 14 del LM324N se dirige al pin 14 del 4017.

- pin 2 hacia un LED, con un color predeterminado, consecutivamente a una resistencia de 1k llegando a GND. Se repite esto con los pins 3, 4 y 7.

- pin 8 a GND.

- pin 13 va a una resistencia de 100k, finalizando en GND.

- pin 15 para hacer reset se conecta al pin 10.

- pin 16 a VVC.

## kicad

![grupo03-pcb](./imagenes/grupo03-pcb-kicad02.jpg)

![grupo03-pcb](./imagenes/grupo03-pcb-kicad03.jpg)

![grupo03-pcb](./imagenes/grupo03-pcb-kicad04.jpg)

![Esquematico en Kicad](./imagenes/grupo03-esquematico-kicad01.pdf)

![PCB en Kicad](./imagenes/grupo03-pcb-kicad05.pdf)


## Recursos adicionales

- El **Chip LMV324M** del SparkFun Sound Detector **lo desglosamos**, por así decirlo, para tener el chip aparte y **poder regular la sensibilidad del micrófono.**

<https://www.sparkfun.com/sparkfun-sound-detector.html>

## Soldadura

Se utilizó soldadura sin plomo y los cautines del laboratorio (ersa  i-con pico) (weller)
a 400°

- Pasos para soldar:

1. Se pone el cautín  3 seg. en el pad para calentar
2. Colocar soldadura
3. Mantener 3seg.
4. Sacar cautin.

Con mucho cuidado

**Recomendaciones:** Utilizamos cinta de papel para que los componentes no se movieran y antes de soldar, revisamos el esquemático y medimos con multímetro cada componente para verificar su valor.

Sólo ocurrieron **dos percances**, ya que el socket del 4017 lo colocamos al revés pero, esto tiene **diferencia mecánica y no eléctrica** . Por otra parte, la huella de las resistencias en kicad es más pequeña pero las acomodamos para que quepan bien sin problemas.

## Carcasa

Decidimos hacer una forma ortogonal, ya que nosotras relacionamos la electrónica con la **geometría,** debido a la **representación gráfica** que pusimos en la pcb, por eso decidimos seguir con la idea en cuanto a la forma de un **prisma** ya que, al buscar sobre los estados de la luz encontramos uno que es el **espectro visible .**

Según **Erco**, el espectro visible "Se denomina espectro a la distribución de las **ondas electromagnéticas.** Solo una pequeña parte en el rango entre 380 y 780 nanómetros (nm) es visible para el ser humano; este rango es lo que **denominamos luz."**

<https://www.erco.com/es/planificacion-de-iluminacion/conocimientos-luminotecnicos/fotometria/espectro-visible-7528/>

Dicho en otras palabras, es cuando la luz pasa a través de un prisma/cristal y emite la **reflexión de colores.**

- Decisión de materiales y colores
  
**Materiales:**

Impresión 3D PLA+ (marca esun). Realizado en Bambulab.
  
Vinilo tornasol transparentoso. Comprado en mercado libre.

Acrílico transparente de 2 mm. Comprado en Acrílicos Chile.

Colores utilizados:
Impresión 3D PLA+ rosada ya que, el vinilo tornasol que utilizamos tiene tonalidades rosadas.

Vinilo tornasol transparentoso.

Acrílico transparente.

## Montaje
