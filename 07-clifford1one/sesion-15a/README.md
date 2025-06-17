# sesion-15a


## Progreso

Conexión del circuito, en este paso, reemplazamos el puente H por un ci L293D. También redujimos la cantidad de circuitos PWM utilizados, de 2 a 1.

![Imagen circuito fps555 v2](./archivos/fps555-sch-v2.png)

También subí el archivo kicad a la carptea [archivos](https://github.com/clifford1one/dis8644-2025-1-proyectos/tree/main/07-clifford1one/sesion-15a/archivos/).


## feedback

Cree un [issue]((https://github.com/disenoUDP/dis8644-2025-1-proyectos/issues/479)) donde mostraba el avance de nuestro esquemático anterior, y gracias al feedback de franUDP y misa, apliqué ciertos cambios.

### cambios

- reemplazar botones por un switch
- quitar el transistor, ya que la función que este cumplía era llevada a cabo por el L293D
- conectar la salida del PWM al pin 1 del L293D(ENABLE). 

![Imagen del esquemático con los cambios realizados.](./archivos/fps555-sch-v4.png)