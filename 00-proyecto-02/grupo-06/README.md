# proyecto-02

## Acerca del proyecto

- Grupo: 06
- Integrantes:
  - Santiago Gaete Fernández
  - Anaís Marschhausen Gajardo
  - Sebastián Saez Olivares
- Chips usados:
  - NE555
  - L293D

## Presentación textual

fps555 es un dispositivo de protección ocular con posición adaptable mecánicamente.

El proyecto consiste en una entrada que XX, para CONTROLAR/OTRO VERBO

## Dibujos de diagramas del circuito (1 punto)

Este es el diagrama a mano.

![Dibujo del diagrama a mano](./imagenes/diagrama-mano.jpg)

En este dibujo mostramos XX.

## Prototipado de circuitos en protoboard (1 punto)

En un principio queríamos que nuestro circuito funcionara gracias a un servomotor para crear un movimiento controlado al interactuar con nuestro producto, pero no funcionó ningún circuito que encontramos en internet, y los que sí funcionaban requieren Arduino para su funcionamiento.

(video que envió Santi)

Luego Matías nos explicó sobre los puentes H, donde podíamos controlar la velocidad y la dirección del movimiento de un motor como el que se encontraba en nuestro kit.

También se nos mencionó que existe un chip integrado que realizaba esta función, pero de igual manera se hizo una prueba del circuito de manera mecánica, con 4 botones, a que era lo que más se asemejaba al esquemático del puente H a primera vista.

El funcionamiento era el siguiente:

Se armaron 2 circuitos PWM donde su output eran conectados hacia botones, donde el circuito 1 quedaría posicionado con su output al positivo del motor, mientras que a través de otro botón se dejaría pasar la conexión para completar el circuito, mientras que el circuito 2 estaría de la manera opuesta, todo esto para que no ocurriese ningún cortocircuito.

(puente H con botones)

Luego pasamos a integrar el chip L293D con el que se pudo reducir su funcionamiento a simplemente 2 botones, uno para cada dirección.

(L293D con botones)

Luego se integró el switch 6 PDT para poder generar este cambio de dirección con tan solo 1 componente, como también el estado neutro “off” del motor.

(L293D on/off/on)

Pero se nos dejó claro en la clase del martes 17 de junio unas ciertas correcciones, para poder asegurarnos de que el L293D estaba correctamente conectado, como también el uso de la otra mitad de nuestro switch on/off/on, y que de esta manera no se fuese a ocupar todo el circuito de manera constante al conectarlo al pin 4 del chip 555.

(protoboard final)

Como último componente, se conectó el motor reductor de 3 rpm que compramos, para poder demostrar el funcionamiento como lo asignamos.

Como resumen:

El circuito de entrada usa la posición del switch para determinar el estado del motoreductor.

El circuito de salida usa el L293D para cambiar el sentido de la rotación del motoreductor.

### Bill of Materials (1 punto)

| Componente   | Cantidad | Comentarios     |
| ------------ | -------- | --------------- |
| Resistor     | 5        | 1/4W            |
| XX | ... | ...       |

INCLUIR DESCRIPCIÓN DE MATERIALES COMPRADOS, SI ES QUE COMPRARON COSAS ADICIONALES.

## Ayudas y comunicación con colegas (1 punto)

DOCUMENTAR TEXTUAL, CON IMÁGENES, CON ENLACES A BITÁCORAS.

La persona XX del proyecto XX nos ayudó con XX.

La persona XX del proyecto XX nos ayudó con XX.

Ayudamos a la persona XX del proyecto XX con XX.

Ayudamos a la persona XX del proyecto XX con XX.

## Esquematico en Kicad (1 punto)

![Esquemático general](./imagenes/esquematico-general.jpg)

![Esquemático detalles](./imagenes/esquematico-detalle-01.jpg)

![Esquemático detalles](./imagenes/esquematico-detalle-02.jpg)

EXPLICACIÓN TEXTUAL DEL ESQUEMÁTICO.

DESCRIBIR CHIPS USADOS, CONEXIONES USADAS.

## PCB en Kicad (1 punto)

![PCB general](./imagenes/pcb-general.jpg)

![PCB detalles](./imagenes/pcb-detalle-01.jpg)

![PCB detalles](./imagenes/pcb-detalle-02.jpg)

![PCB 3D](./imagenes/pcb-3d.jpg)

## Recursos adicionales

## Bibliografía
