# examen

grupo-05

## integrantes
  - Antonia Cristi [@antocristi](https://github.com/antocristi)
  - Natalia Pilar [@sz-mada](https://github.com/sz-mada)
  - Paulina Vargas [@paulinavargasf](https://github.com/paulinavargasf)

## proyecto-02

### aprendizajes

Pedir ayuda a gente externa al equipo (específicamente los grupos 00), organizarnos en estaciones de trabajo para facilitar el avance durante el día

### dificultades

El circuito de la ruleta en las placas no funcionaba como se esperaba

Los cables para soldar los componentes colgantes se cortaban constantemente a la altura de la placa

Se nos olvidó quitar un chip al momento de soldar y lo quemamos, pero conseguimos darnos cuenta y cambiarlo

El circuito no recibía el input del LDR

[FranUDP](https://github.com/FranUDP) y Aarón nos ayudaron a darnos cuenta que el chip LM324 no lo habíamos conectado a tierra ni VCC en el esquemático, así que en la placa final tampoco estaba conectado

La solución que nos dió Aarón, fue conectar los pines 4 y 11 externamente a la alimentación de la placa

![chip LM324 con pin 4 levantado](./imagenes/procesos/proceso_01.jpg)

![LM324 con pines 4 y 11 levantados](./imagenes/procesos/proceso_02.jpg)

![Conexión a tierra del pin 4](./imagenes/procesos/proceso_03.jpg)

![Conexión a alimentación de los pines 4 y 11](./imagenes/procesos/proceso_04.jpg)

## PCB

Protoboards de prototipado

El proyecto consiste en dos circuitos paralelos; el primero consiste en un detector de sombra y una secuencia de leds de 10 pasos, y el segundo de un micrófono electret que activa una luz led. Estos circuitos no afectan entre sí, y tan solo son un truco para el usuario.

Imágenes de las protoboards

![protoboards vista lateral](./imagenes/protoboard/tme-grupo05-protoboard-registro01.JPG)

![protoboard ruleta vista lateral](./imagenes/protoboard/tme-grupo05-protoboard-registro02.JPG)

![protoboard ruleta vista superior](./imagenes/protoboard/tme-grupo05-protoboard-registro03.JPG)

![protoboard ruleta detalle 01](./imagenes/protoboard/tme-grupo05-protoboard-registro04.JPG)

![protoboard ruleta detalle 02](./imagenes/protoboard/tme-grupo05-protoboard-registro06.JPG)

Imágenes de las placas PCB

![PCB vacía](./imagenes/pcb/tme-grupo05-pcb-registro01.JPG)

![PCB vacía reverso](./imagenes/pcb/tme-grupo05-pcb-registro03.JPG)

![PCB juntas](./imagenes/pcb/tme-grupo05-pcb-registro07.JPG)

![PCB juntas](./imagenes/pcb/tme-grupo05-pcb-registro08.JPG)

![PCB ruleta](./imagenes/pcb/tme-grupo05-pcb-registro04.JPG)

![PCB micrófono](./imagenes/pcb/tme-grupo05-pcb-registro10.JPG)

![PCB detalle](./imagenes/pcb/tme-grupo05-pcb-registro12.JPG)

## soldadura

Decidimos soldar las placas a lo largo de distintos días.

Inicialmente, soldamos una de cada placa con todos los componentes directo en estas para asegurarnos que todo funcionara como debía.

Luego, las otras placas las soldamos con cables para poder montar en la carcasa, pero tuvimos problemas ya que estos cables tendían a cortarse muy fácilmente.

Finalmente, luego de terminar de soldar y arreglar los cables cortados, montamos las placas correspondientes a la carcasa.

![soldadura de PCBs](./imagenes/soldadura/soldadura_01.jpg)

![soldadura de PCB ruleta](./imagenes/soldadura/soldadura_02.jpg)

![soldadura de PCB micrófono](./imagenes/soldadura/soldadura_03.jpg)

## carcasa

La carcasa se hizo en dos partes, la tapa con terciado de 3mm, y el contendor con impresión 3D PLA+ en Bambulab.

Las luces LED de la ruleta se colocaron en la parte superior de la carcasa en forma de arco, y el LDR fue situado en el centro para ser accesible al usuario.

Para la tapa decidimos agregar un diseño inspirado por la rueda de la fortuna de las cartas de tarot, con el centro de esta ruleta alineándose con el LDR.

![carta del tarot](./imagenes/procesos/carta_tarot.jpg)

Imágenes de la carcasa

![carcasa recién impresa](./imagenes/carcasa/tme-grupo05-carcasa-registro00.jpg)

![carcasa vista axial 01](./imagenes/carcasa/tme-grupo05-carcasa-registro01.jpg)

![carcasa vista axial 02](./imagenes/carcasa/tme-grupo05-carcasa-registro03.jpg)

![carcasa vista superior](./imagenes/carcasa/tme-grupo05-carcasa-registro04.jpg)

![carcasa detalle](./imagenes/carcasa/tme-grupo05-carcasa-registro06.jpg)

## montaje

????
