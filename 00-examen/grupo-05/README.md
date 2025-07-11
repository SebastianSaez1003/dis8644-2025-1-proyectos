# examen

grupo-05

## integrantes
  - Antonia Cristi [@antocristi](https://github.com/antocristi)
  - Natalia Pilar [@sz-mada](https://github.com/sz-mada)
  - Paulina Vargas [@paulinavargasf](https://github.com/paulinavargasf)

## proyecto-02.

### aprendizajes

El mayor aprendizaje que obtuvimos durante el proyecto fue la importancia de pedir ayuda a personas externas al equipo. Al principio intentamos resolver todo solos, pero nos dimos cuenta que consultando con los docentes o gente de otros grupos, podíamos tener nuevas soluciones que nunca habríamos pensado. Si bien no logramos solucionar el principal problema que tuvimos durante todo el proyecto, el pedir ayuda nos permitió entender mejor la raíz de este error.

También aprendimos a organizarnos mejor dividiendo la carga en estaciones de trabajo, lo cual fue muy útil para optimizar el tiempo, ya que cada uno podía concentrarse en algo específico, y así como equipo avanzábamos en paralelo en vez de esperar a que alguien terminara de hacer lo suyo para que el resto siguiera trabajando.

### dificultades

Una de las principales dificultades fue que el circuito de la ruleta no funcionaba como habíamos planeado. Cuando montamos todos los componentes en la placa, al probarlo notamos que no respondía como debía. Revisamos varias veces los componentes para asegurarnos de no haber echo nada mal, pero no logramos encontrar el problema.

Otro problema constante fueron los cables de los componentes colgantes, que se cortaban con facilidad justo en la unión con la placa. Esto nos generó muchos retrasos ya que tuvimos que volver a soldar varias veces y reforzar las conexiones, lo cual también aumentaba el riesgo de dañar otros componentes en la placa.

Además, tuvimos un descuido **muy** importante: se nos olvidó retirar un chip antes de soldar cerca, así que se quemó. Por suerte, pudimos descubrir el error a tiempo.

Tuvimos un problema con el LDR, ya que el circuito no estaba recibiendo su señal como se esperaba. Aún después de revisar el componente y las conexiones, el sensor seguía sin responder correctamente, lo cual fue una de las dificultades que no logramos solucionar completamente.

Con ayuda de [FranUDP](https://github.com/FranUDP) y Aarón pudimos descubrir el error principal que estaba afectando el circuito. Nos hicieron notar que no teníamos el chip LM324 conectado a la alimentación, lo que explica por qué el circuito no funcionaba desde el inicio. Aarón nos sugirió una posible solución, conectar externamente los pines 4 y 11 del chip a la fuente de alimentación de la placa. Tristemente, aún después de probar esto, el circuito siguió sin funcionar correctamente. No sabemos si este problema era la única causa o si habían otros errores adicionales en la placa, pero sin dudarlo, podemos decir que fue el problema principal que nos retuvo durante la gran parte del proyecto.

![chip LM324 con pin 4 levantado](./imagenes/procesos/proceso_01.jpg)

![LM324 con pines 4 y 11 levantados](./imagenes/procesos/proceso_02.jpg)

![Conexión a tierra del pin 4](./imagenes/procesos/proceso_03.jpg)

![Conexión a alimentación de los pines 4 y 11](./imagenes/procesos/proceso_04.jpg)

## bill of materials

|QTY|NAME|VALUE|OBS
|:-:|-|-|-
|3|Socket 8-pin|-|-
|1|Socket 14-pin|-|-
|1|Socket 18-pin|-|-
|7|Resistencia|10k|-
|3|Resistencia|1k|-
|1|Resistencia|100k|-
|1|Diodo|1n4007|-
|1|LDR|LDR|-
|3|Condensador cerámico|474n|-
|1|Transistor|PN2222A|-
|1|Micrófono electret|MIC|-
|3|Condensador electrolítico|1u|-
|1|Condensador electrolítico|100u|-
|11|LED 5mm|LED|Distintos colores
|1|Potenciómetro|500k|-
|3|DIP-8|NE555|-
|1|DIP-14|LM324|-
|1|DIP-16|CD4017|-
|1|Terminal Block|2-pin|-
|1|Switch spdt|-|-
|26|Cables dupont|-|-

## PCB

El proyecto consiste en dos circuitos paralelos con sus respectivas PCBs; el primer circuito consiste en un detector de sombra que, por medio de un LDR, activa una secuencia de 10 pasos de LEDs, y el segundo es un micrófono electret que enciende una luz LED por medio del input de sonido. Estos circuitos **no** están relacionados en funcionalidad; el circuito del micrófono solo es un truco para el usuario.

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

Luego, en las otras placas, soldamos cables hacia los LEDs y el LDR para poder montarlos en la carcasa, pero tuvimos problemas ya que estos cables tendían a cortarse muy fácilmente.

Finalmente, luego de terminar de soldar y arreglar los cables cortados, montamos las placas correspondientes a la carcasa.

![soldadura de PCBs](./imagenes/soldadura/soldadura_01.jpg)

![soldadura de PCB ruleta](./imagenes/soldadura/soldadura_02.jpg)

![soldadura de PCB micrófono](./imagenes/soldadura/soldadura_03.jpg)

## carcasa

La carcasa se construyó en dos partes: una tapa hecha con madera terciada de 3mm en corte láser, y el contendor en impresión 3D.

Las luces LED de la ruleta se colocaron en la parte superior de la tapa en forma de arco, y el LDR fue situado en el centro para ser accesible al usuario.

Antes de cortar la tapa, decidimos agregar un diseño inspirado por una de las cartas del tarot, la rueda de la fortuna, con el centro de esta rueda alineándose con el posicionamiento del LDR.

![carta del tarot](./imagenes/procesos/carta_tarot.jpg)

Imágenes de la carcasa

![carcasa recién impresa](./imagenes/carcasa/tme-grupo05-carcasa-registro00.jpg)

![carcasa vista axial 01](./imagenes/carcasa/tme-grupo05-carcasa-registro01.jpg)

![carcasa vista axial 02](./imagenes/carcasa/tme-grupo05-carcasa-registro03.jpg)

![carcasa vista superior](./imagenes/carcasa/tme-grupo05-carcasa-registro04.jpg)

![carcasa detalle](./imagenes/carcasa/tme-grupo05-carcasa-registro06.jpg)

## montaje

Para el montaje, decidimos que la mejor manera de exponer nuestro proyecto sería comenzando con el "producto" final a la izquierda (el proyecto montado con la carcasa), llevando al prototipo inicial en la derecha (las protoboards).

El orden de las placas PCBs desde abajo hacia arriba es: placa vacía &rarr; placa con componentes soldados directamente en esta &rarr; placa con componentes soldados en cables para montaje en la carcasa &rarr; placas de intentos fallidos

![montaje 1](./imagenes/montaje/montaje_01.jpg)


![montaje 2](./imagenes/montaje/montaje_02.jpg)


![montaje placas](./imagenes/montaje/montaje_03.jpg)
