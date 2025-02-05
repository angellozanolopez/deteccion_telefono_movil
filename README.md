**Formación en visión artificial: detección de objetos en vídeos**

**Bloque 1**

La formación consistirá en aprender cómo funciona Google Colab para el procesamiento de vídeos y la creación de proyectos de Visión Artificial (créate una cuenta allí con tu e-mail de Overstand, encontrarás información sobre cómo crear una cuenta de Google en el Welcome Pack . PDF). Una vez hayas accedido a Colab, puedes realizar lo siguiente:

- Cargar un vídeo MP4 (o similar) en el directorio de trabajo de Colab
- Separar el vídeo en frames
- Printar el número de frames por el stdout

**Bloque 2**

El objetivo en este momento es detectar si aparece algún teléfono móvil en el vídeo que encontrarás en este mismo directorio. 

Puedes usar Yolo para ello. Como verás, el sistema detecta móviles entre muchas otras cosas (personas, etc). 

Te recomendamos buscar una versión de algún modelo que ya esté preentrenado y descargar simplemente la estructura y los pesos de la red neuronal.

En este caso utilizaremos Yolo (a pesar de haber versiones más nuevas disponibles), pues nos viene preentrenada con 80 clases, aunque en nuestro caso solo nos interesa el teléfono móvil.

Para utilizar yolo (el siguiente ejemplo es con v3 aunque hay versiones más nuevas disponibles las cuales debes usar) y toda su estructura, puedes entrar en el siguiente enlace de github[ https://github.com/pjreddie/darknet ](https://github.com/pjreddie/darknet) 

Una vez hayas visto cómo funciona Yolo, desarrolla una función

que te genere los frames y que para cada frame se generen unos loops, para posteriormente realizarle la clasificación y bajo un umbral dibujar el cuadrado que correspondería al teléfono móvil. Y generando un nuevo vídeo formado por todos los frames añadiendo los cuadros de clasificación.

Te animamos a probar de resolverlo por tus propios medios. Si en algún momento te atascas o no logras resolverlo, avísame y te enviaré el código completo hasta este punto.

¡Ánimos!

**Bloque 3**

Como habrás observado al procesar otros vídeos, si el smartphone lleva funda o carcasa, hay varias ocasiones en que no es detectado por el sistema. ¿Qué alternativa aplicarías, y cómo?

**Bloque 4**

Una vez entendido el funcionamiento del bloque 3, partiremos otra vez del anterior (bloque 2) ya que es totalmente funcional. La misión será, ahora, conectar la videocámara de tu ordenador (o una externa) en streaming a Google Colab para ejecutar el modelo en directo.

¡Ánimos!

**----**

Entregables (en un único wetransfer):

1. Código fuente de la solución
1. Vídeo explicativo del código fuente (máximo 3 minutos)
1. Vídeo mostrando e interpretando los resultados (máximo 2 minutos)
