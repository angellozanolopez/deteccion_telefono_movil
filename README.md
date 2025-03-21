# Formación en visión artificial: detección de objetos en vídeos

## **Bloque 1**

La formación consistirá en aprender cómo funciona Google Colab para el procesamiento de vídeos y la creación de proyectos de Visión Artificial (créate una cuenta allí con tu e-mail de Overstand, encontrarás información sobre cómo crear una cuenta de Google en el Welcome Pack . PDF). Una vez hayas accedido a Colab, puedes realizar lo siguiente:

- Cargar un vídeo MP4 (o similar) en el directorio de trabajo de Colab
- Separar el vídeo en frames
- Printar el número de frames por el stdout

## SOLUCION BLOQUE 1
### 📹 Video y Demostración  
🔹 [![Ver en YouTube](https://img.shields.io/badge/🎥%20Código-red?logo=youtube&logoColor=white)](https://youtu.be/evtm7VpLsDA?si=LdyZENa0Wygwlq28)<br>🔹 [![Ver en YouTube](https://img.shields.io/badge/🎥%20Demostración-red?logo=youtube&logoColor=white)](https://youtu.be/iVYqIj38cfY?si=0GtUAMkk4aZmzlW8)<br>📌 *Haz clic con el botón derecho encima del botón y selecciona "Abrir enlace en una nueva pestaña" para no salir del repositorio.*  

---

## **Bloque 2**

El objetivo en este momento es detectar si aparece algún teléfono móvil en el vídeo que encontrarás en este mismo directorio.  

Puedes usar Yolo para ello. Como verás, el sistema detecta móviles entre muchas otras cosas (personas, etc).  

Te recomendamos buscar una versión de algún modelo que ya esté preentrenado y descargar simplemente la estructura y los pesos de la red neuronal.  

En este caso utilizaremos Yolo (a pesar de haber versiones más nuevas disponibles), pues nos viene preentrenada con 80 clases, aunque en nuestro caso solo nos interesa el teléfono móvil.  

Para utilizar Yolo (el siguiente ejemplo es con v3 aunque hay versiones más nuevas disponibles las cuales debes usar) y toda su estructura, puedes entrar en el siguiente enlace de GitHub:  
[https://github.com/pjreddie/darknet](https://github.com/pjreddie/darknet)  

Una vez hayas visto cómo funciona Yolo, desarrolla una función que te genere los frames y que para cada frame se generen unos loops, para posteriormente realizarle la clasificación y bajo un umbral dibujar el cuadrado que correspondería al teléfono móvil. Luego, genera un nuevo vídeo formado por todos los frames añadiendo los cuadros de clasificación.  

Te animamos a probar de resolverlo por tus propios medios. Si en algún momento te atascas o no logras resolverlo, avísame y te enviaré el código completo hasta este punto.  

## SOLUCION BLOQUE 2
### 📹 Video y Demostración  
🔹 [![Ver en YouTube](https://img.shields.io/badge/🎥%20Código-red?logo=youtube&logoColor=white)](https://youtu.be/pBjsOB4OOFg?si=2KbGEd6wcFFUYFzQ)<br>🔹 [![Ver en YouTube](https://img.shields.io/badge/🎥%20Demostración-red?logo=youtube&logoColor=white)](https://youtu.be/p185JT0NhxM?si=MGObUz1sKBy7darg)<br>📌 *Haz clic con el botón derecho encima del botón y selecciona "Abrir enlace en una nueva pestaña" para no salir del repositorio.*  

---

## **Bloque 3**

Como habrás observado al procesar otros vídeos, si el smartphone lleva funda o carcasa, hay varias ocasiones en que no es detectado por el sistema. ¿Qué alternativa aplicarías, y cómo?  

### **Posibles mejoras en la detección:**  
1. **Aumentar datos de entrenamiento:** Recolectar imágenes de teléfonos con funda o carcasa y agregarlas al conjunto de datos de entrenamiento para crear nuestro propio modelo personalizado. Esto puede ayudar al modelo a reconocer mejor estas variaciones.  
2. **Data augmentation:** Aplicar efectos como rotación, cambio de escala, cambio de iluminación, etc., permitiendo que el modelo generalice mejor.  
3. **Refinamiento de hiperparámetros:** Ajustar los parámetros del modelo y las técnicas de entrenamiento para mejorar la precisión en la detección de objetos específicos, como modificar la variable de confianza dependiendo de si se producen más o menos detecciones falsas.  

Estas estrategias podrían implementarse de manera individual o combinada para mejorar la detección de teléfonos con fundas o carcasas según el contexto en el que nos movemos.  

---

## **Bloque 4**

Una vez entendido el funcionamiento del bloque 3, partiremos otra vez del anterior (bloque 2) ya que es totalmente funcional. La misión será, ahora, conectar la videocámara de tu ordenador (o una externa) en streaming a Google Colab para ejecutar el modelo en directo.  

## SOLUCION BLOQUE 4
### 📹 Video y Demostración  
🔹 [![Ver en YouTube](https://img.shields.io/badge/🎥%20Código-red?logo=youtube&logoColor=white)](https://youtu.be/IjFplR2bOC4?si=1BfCJbKLnECz8ZgV)<br>🔹 [![Ver en YouTube](https://img.shields.io/badge/🎥%20Demostración-red?logo=youtube&logoColor=white)](https://youtu.be/KL0BQlyu-xA?si=y_FurhYn16bm7geS)<br>📌 *Haz clic con el botón derecho encima del botón y selecciona "Abrir enlace en una nueva pestaña" para no salir del repositorio.*  
