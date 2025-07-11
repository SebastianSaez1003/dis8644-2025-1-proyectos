# examen

grupo-06

fps555

Proyecto realizado para el Taller de Máquinas Electrónicas de la Universidad Diego Portales (dis8644-2025).

## Integrantes:

- Santiago Ignacio Gaete Fernández / clifford1one  

- Anais Belen Marschhausen Gajardo / Anaisbmg  

- Sebastian Alejandro Ignacio Saez Olivares / SebastianSaez1003  

## Presentación de la idea inicial y contexto

Nuestra idea de un principio era un accesorio wearable, que automáticamente pudiese “bajar” unos lentes de sol por sobre los de una persona que tuviese puestos lentes ópticos.

Gracias a un circuito detector de umbral, junto a un servomotor, se podría efectuar este movimiento de los lentes sin necesidad de una acción por parte del usuario.

Para nuestro test inicial del circuito, el servomotor no funcionaba con ninguno de los circuitos que probamos, así que decidimos ir a la solución con componentes que ya habíamos usado antes, entre esos un chip 555, para que pudiéramos regular las revoluciones por segundo de un motor regular, con la intención de que los lentes no golpeasen al usuario, sino que rotaran lentamente hacia abajo y hacia arriba.

## Circuito y su funcionalidad

Con la guía de nuestro profesor Matias Serrano, investigamos sobre el funcionamiento de un circuito llamado el “puente H”, este permite que un motor gire en ambos sentidos. Como era perfecto para nuestro objetivo, lo probamos de manera mecánica, a través de botones que permitían que llegara la corriente para que el motor girara en sentido horario o antihorario.

Ya que de esta manera era plausible el funcionamiento, fuimos capaces de incorporar un circuito integrado de nombre L293DNE, que tenía por dentro el puente H de manera nativa para el funcionamiento de 2 motores, el cual solo ocupamos un motor, que puede rotar en ambas direcciones.

Ya con la conexión entre el circuito PWM (Pulse Width Modulation) y el puente H teníamos nuestro funcionamiento por completo, excepto por el tema de las revoluciones de nuestro motor, que ni siquiera con el PWM era lo suficientemente lento, así que implementamos un motoreductor que tuviese 3 RPM y de esta manera es más razonable el movimiento de la rotación de los lentes.

Con esto ya está el funcionamiento, pero la interacción del usuario aún estaba pendiente, lo que se ocupó fue un interruptor ON-OFF-ON de 6 pines, que fue usado con 2 funciones, 3 de sus pines servía para  era que el motorreductor rotará en el sentido horario, contrahorario o no rotara en absoluto, mientras que los otros 3 pines servían a modo de interruptor de alimentación hasta el circuito que llegaba al moto controlador (L293DNE), donde dejará pasar la energía en sus dos estados ON, qué son los mismos que activan el motorreductor en sus dos sentidos, mientras que el estado OFF no dejaba el paso de energía, de esta manera no se perdía batería de mayor manera, solo lo necesario para que el LED de funcionamiento esté encendido

## PCB

Para la PCB elegimos un formato de 10 cm x 5 cm, ya que elegimos serigrafía para decorar unos lentes de modelo similar al que es usado en el producto final.

El posicionamiento de los componentes fue pensado con la intención de mantener la forma de los lentes reconocible, donde uno de los holders del chip funcionase como la conexión entre los anteojos, el potenciómetro pareciera una nariz y los tblock, de donde saldrían cables de conexión, parecieran varillas.

## Soldadura

En el proceso previo a la soldadura, se realizó una selección de componentes del BOM y los fuimos posicionando respectivamente en su lugar en la PCB. Primero colocamos las resistencias y los condensadores, ya que estos son más pequeños. Luego seguimos con el LED y los sockets, ya que los chips deben posicionarse sobre un socket para evitar repercusiones en su funcionamiento. Para finalizar, agregamos los T-blocks, los pin headers y el potenciómetro, a este último decidimos hacerle una adaptación para que su posición esté más cercana al usuario.

Parte importante de este proceso es asegurarse de la polaridad de nuestros componentes, que en este caso son los diodos, que se colocan en guía a la huella serigrafiada, el LED que debe estar con su lado negativo conectado de la manera correcta, los sockets de nuestros chips, para que la persona que esté armando el circuito sepa correctamente en qué dirección debe ser colocado el circuito integrado y, por último, los T-Block, que deben estar con sus entradas en dirección opuesta al centro de la PCB, de esta manera no se interrumpe nada que ocurra en el ensamblaje.

## Carcasa

Debido a que nuestro dispositivo es un “wearable”, tuvimos que investigar sobre materialidad que fuese flexible, donde se llegó al filamento TPU de impresión 3D. Se realizaron probetas de pequeño tamaño para poder determinar el grosor que es el más adecuado para nuestras impresiones.

!(Foto de las probetas de TPU)

La forma elegida fueron triángulos con unas sustracciones de una circunferencia en cada uno de sus lados, con un orificio cerca de la punta de estos, para poder interconectarlos entre sí con unos “tarugos” impresos en 3D para que no se desarme.

!(foto de los triángulos)

!(foto de los tarugos)

Con esta forma se llegó a un casco que, gracias a la flexibilidad del filamento, se adapta a distintos tamaños de cabezas.

!(foto del casco)

Para poder montar el circuito en sí, se modeló en RHINO una pieza que sería impresa en 3D con un filamento más firme PET-G, para que el funcionamiento no sufriera por ninguna variación mayor, y que estuviese lo más controlada posible. En esta pieza se podía introducir la PCB, dejándola fija con los agujeros que tiene en sí misma con pernos, también tiene un espacio en el que se introduce el switch, una base donde montar el motorreductor y que no se moviese de su lugar.

## Aprendizajes

Aprendimos a repartirnos tareas según nuestras distintas habilidades para poder desarrollar nuestro proyecto de la manera más eficiente posible.

Es muy importante el poder presupuestar todos nuestros componentes para que podamos conseguirlos en la mayor relación de calidad/precio. 

Juntamos distintas áreas, desde el diseño gráfico, diseño industrial, interfaz de usuario y la electrónica, para llegar a un producto multidisciplinario.

## Dificultades

La primera idea que tuvimos no fue usada ya que la idea ya era un circuito existente, que de hecho era vendido como un componente, así que se descartó.

Nuestro circuito inicial no funcionó con un componente en un inicio, el cual era un servomotor, y esto nos dejó en pausa hasta que los profesores nos ayudaron a darle una vuelta con componentes con los cuales ya éramos familiares.


## BOM (bill of materials)
| Grupo 6  |                          |                                |                    |                                                  |                                                           
|:-------: |------------------------- |:-----------------------------: |------------------- |------------------------------------------------- |                                                       
|   Item   |           Qty            |           Referencia           |       Valor        |                   Tipo de ítem                   |                             
|    1     |            2             |             R1, R3             |         1K         |                   Resistencia                    |                             
|    2     |            2             |               R2               |        10K         |                   Resistencia                    |                              
|    3     |            2             |             R4, R7             |        100K        |                   Resistencia                    |                            
|    4     |            1             |             R5, R6             |        470K        |                   Resistencia                    |                                 
|    5     |            6             |             D2~D7              |       1n4007       |                      Diodo                       |                                
|    6     |            1             |               C1               |        100n        |              Condensador (cerámico)              |                             
|    7     |            1             |               C2               |        470nf       |              Condensador (cerámico)              |              
|    8     |            1             |               D1               |        3mm         |                       Led                        |                                 
|    9     |            1             |               U1               |        555         |                       Chip                       |                                 
|    10    |            1             |               U2               |      L293DNE       |                       Chip                       |                                   
|    11    |            1             |               U3               | 6 Pines ON-OFF-ON  |                Interruptor Switch                |                                      
|    12    |            1             |               M1               |      6V 3RPM       |                 Motorreductor DC                 |                                        
|    13    |            1             |              RV1               |        500K        |                  Potenciometro                   |                              
|    14    |            2             |                                |      2 pines       |                      Tblock                      | 
|    15    |            1             |               U1               |      8 pines       |                      Socket                      |                        
|    16    |            1             |               U2               |      16 pines      |                      Socket                      |                               
|    17    |            6             |                                |                    |                    Pin Header                    |                           
|    18    |            6             |                                |                    | Cable dupont: terminal receptora a terminal pin  |                                   
