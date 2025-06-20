# proyecto-02

## Acerca del proyecto

- Grupo: 04
- Integrantes:
  - Braulio Figueroa
  - Carlo Martínez
  - Bastian Solís
- Chips usados:
  - Chip LM324
  - Chip NE555

## Presentación textual

El proyecto consiste en un juguete para gato que funciona con un LDR que controla la activación de un motor dc

## Dibujos de diagramas del circuito (1 punto)

Este es el diagrama a mano.

![Dibujo del diagrama a mano](https://github.com/HSB25/dis8644-2025-1-proyectos/blob/main/00-proyecto-02/grupo-04/imagenes/BOCETODIAGRAMAFLUJO.jpg?raw=true)

En este dibujo mostramos nuestro proyecto el cual consiste en un juguete automático para gatos que funciona con un sensor de luz (LDR). Cuando el gato se coloca frente al sensor, su sombra reduce la luz que llega al LDR, lo que activa el motor del juguete. Si el gato se aleja, vuelve a llegar luz al sensor, lo que hace que el motor se apague. Así, el juguete se enciende solo cuando el gato está presente y se apaga automáticamente cuando se va.

# Diagrama de Flujo (SIMPLE)

![DIAGRAMA DE FLUJO](https://github.com/HSB25/dis8644-2025-1-proyectos/blob/main/00-proyecto-02/grupo-04/imagenes/DIAGRAMADEFLUJO01.png?raw=true)

- Resumen del funcionamiento del juguete para gato (según el dibujo):

1. Inicio:
El sistema comienza en modo espera.

2. ¿El gato está frente al LDR?
Se detecta si hay sombra sobre el sensor de luz (LDR). Esto indica que el gato está cerca.

3. Si el gato está frente al sensor (hay sombra):
→ Se activa el motor del juguete para que se mueva.

4. Si el gato se va (hay luz):
→ Se desactiva el motor automáticamente.

5. Fin:
El sistema vuelve al inicio y espera una nueva detección.

# Diagrama de Flujo (DETALLADO)

![DIAGRAMA DE FLUJO 2](https://github.com/HSB25/dis8644-2025-1-proyectos/blob/main/00-proyecto-02/grupo-04/imagenes/DIAGRAMADEFLUJO02.png?raw=true)

- Funcionamiento General del Sistema

1. Detección de sombra (presencia del gato):

El sistema usa un sensor LDR (resistor dependiente de la luz) que mide la cantidad de luz ambiente.
Cuando hay luz normal, el sensor detecta niveles altos de luz.
Cuando el gato se acerca al juguete y lo tapa (proyectando sombra), el sensor detecta una baja de luz.

2. Activación del motor:

Al detectar esa baja de luz, el sistema interpreta que el gato está presente.
Se activa un temporizador o lógica de control que enciende un motor DC.
Este motor puede mover una cuerda, una pluma u otro objeto que atraiga la atención del gato.

3. Desactivación automática:

Cuando el gato se aleja del juguete, vuelve a llegar luz al sensor.
El sistema detecta el aumento de luz y apaga el motor automáticamente.
El juguete vuelve a estar en modo espera, listo para activarse nuevamente.

### Resumen del Comportamiento

| Situación                       | Sensor (LDR) detecta | Acción del sistema     |
|--------------------------------|----------------------|------------------------|
| Gato frente al sensor (sombra) | Poca luz             | Motor se enciende      |
| Gato se va                     | Luz normal           | Motor se apaga         |


## Prototipado de circuitos en protoboard (1 punto)

A continuación se presentan imágenes de las protoboards usadas.

![Vista protoboard de frente](./imagenes/tme-grupo04-registro02.jpg)

![Vista protoboard de arriba](./imagenes/tme-grupo04-registro01.jpg)

A continuación se presentan textos explicativos del prototipado.

El circuito de entrada USA XX para medir XX.

El circuito de salida usa XX para cambiar XX.

## Bill of Materials (1 punto)

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

![Esquemático general](./imagenes/esquematicofinal2.JPG)

![Esquemático detalles](./imagenes/esquematico-detalle-01.JPG)

![Esquemático detalles](./imagenes/esquematico-detalle-02.JPG)

EXPLICACIÓN TEXTUAL DEL ESQUEMÁTICO.

DESCRIBIR CHIPS USADOS, CONEXIONES USADAS.

## PCB en Kicad (1 punto)

![PCB general](./imagenes/pcb-general.jpg)

![PCB detalles](./imagenes/pcb-detalle-01.JPG)

![PCB detalles](./imagenes/pcb-detalle-02.JPG)

![PCB 3D](./imagenes/pcb-3d.JPG)

![PCB 3D](./imagenes/pcb-3d-02.JPG)

## Recursos adicionales

## Bibliografía
