# sesion-14a

como grupo 06 decidimos realizar el proyecto de SebastianSaez1003, que trata sobre uno lentes que varían su inclinación gracias a un motor.

## fps555

nuestra idea inicial consiste en desarrollar unos lentes de sol inteligentes. fps555 estarían equipados con un LDR. al detectar una intensidad de luz solar que pudiera ser dañina para la vista, los lentes encenderían un LED, recomendando al usuario que se los baje para protegerse. cuando la luz ambiental no representara un riesgo significativo, el LED se apagaría, indicando que no es necesario el uso de los lentes de sol. también habíamos pensado que la fuente de alimentación fuera un panel solar.

en esta sesión decidimos utilizar un servomotor, ya que consideramos que, una rotación de un punto x a un punto y sería la adecuada. seguimos este [video](https://youtu.be/J-QO7jQGfoE?si=Z3w117Cx1wl5pYNk&t=9) para entender el movimiento de este.

también construimos un detector de luz/sombra con un LDR.

tras la retroalimentación, decidimos utilizar un interruptor en vez del LDR, con el fin de simplificar el proyecto, ya que era complejo. asimismo, decidimos utilizar un motorreductor. buscando opciones, decidimos utilizar uno de 3 rpm de 6 v, ya que este tenía las revoluciones que generaban un movimiento óptimo para nuestro proyecto.

con dos circuitos PWM, uno que mueva los lentes de la frente del usuario a sus ojos, el otro generará el movimiento contrario, activados por un switch de 6 pines o de tres estados on-off-on.

la posición del switch estará de tal forma que al subir el interruptor, los lentes se muevan en dirección a la frente, y al bajar el interruptor, el movimiento será en dirección a los ojos, ademas el centro del interruptor será su posición neutra.
