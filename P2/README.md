# Práctica 1 - Funciones básicas de OpenCV

El objetivo de la práctica es seguir profundizando en las operaciones fundamentales de procesamiento de imágenes de OpenCV, 
como la conversión entre diferentes espacios de color (especialmente la conversión a escala de grises), el cálculo de bordes mediante 
el algoritmo de Canny, la segmentación de imágenes mediante umbralización, el análisis de histogramas y 
la detección de cambios entre fotogramas con técnicas de sustracción de fondo. Estas herramientas permiten explorar los conceptos 
clave del procesamiento de imágenes, facilitando la detección de características visuales esenciales para tareas de visión por computador.

## Autores
[![GitHub](https://img.shields.io/badge/GitHub-Javier%20Gómez%20Falcón-red?style=flat-square&logo=github)](https://github.com/GomFal)
[![GitHub](https://img.shields.io/badge/GitHub-Cristian%20Marrero%20Vega-blue?style=flat-square&logo=github)](https://github.com/XxMARRExX)

## Tecnologías
  - [Python](https://www.python.org/)

## Librerías 
  - [OpenCV](https://opencv.org/)
  - [Matplotlib](https://matplotlib.org/)
  - [NumPy](https://numpy.org/)

## TAREA 1: Realiza la cuenta de píxeles blancos por filas (en lugar de por columnas). Determina el máximo para filas y columnas (uno para cada) y muestra el número de filas con un número de píxeles blancos mayor o igual que 0.95*máximo.

- **Paso 1. Leer imagen**: Se lee la imagen *mandril.jpg*, para convertirla a una imagen en escala de grises.
- **Paso 2. Captura de bordes**: 
    Para ello usamos la función *Canny()*. Esta  función aplica el algoritmo de detección de bordes que identifica 
    bordes en una imagen basándose en cambios abruptos en la intensidad de los píxeles.
- **Paso 3. Extracción del máximo para filas y columnas**: Usamos la función *max()* para extraer los máximos.
- **Paso 4. Normalización de los valores**: En este ejercicio no es necesario hacerlo, pero es importante de cara a usos futuros como redes neuronales.
- **Paso 5. Búsqueda de filas mayores que el 95% del máximo**: Procedemos a iterar sobre los valores de las filas para encontrar el número de filas que cumplen la condición *filas > 0.95 * máximo*

## Tarea 2: Aplica umbralizado a la imagen resultante de Sobel (valores 0 a 255 y convertida a 8 bits por ejemplo sobel8 = np.uint8(sobel)), y posteriormente realiza el conteo por filas y columnas similar al realizado en el ejemplo con la salida de Canny. Calcula los máximos por filas y columnas, y determina las filas y columnas por encima del 0.95*máximo. Remarca con alguna primitiva gráfica dichas filas y columnas sobre la imagen ¿Cómo se comparan los resultados obtenidos a partir de Sobel y Canny?

- **Paso 1. Capturar la imagen desde la cámara web:**: Se utiliza *cv2.VideoCapture(0)* para acceder a la cámara web del sistema y capturar los fotogramas.
- **Paso 2. Obtener el ancho y alto de la cámara, ajustándolos para reducir el tamaño:**
- **Paso 3. Crear un collage en negro para visualizar todas las transformaciones:**
- **Paso 4. Iniciar el bucle para capturar fotogramas:**
- **Paso 5. Procesamiento de la imagen capturada:**
- **Paso 6. Colocar las diferentes versiones de la imagen en el collage:**
- **Paso 7. Mostrar el collage resultante:**
- **Paso 8. Liberar los recursos:**


## Tarea 3: Tras ver los vídeos My little piece of privacy, Messa di voce y Virtual air guitar plantear una reinterpretación de la parte de procesamiento de la imagen tomando como punto de partida alguna de dichas instalaciones.

- **Paso 1. Capturar vídeo desde la cámara web:**
- **Paso 2. Cargar el clasificador Haar Cascade para detección de rostros:**
- **Paso 3. Convertir la imagen a escala de grises para la detección de rostros:**
- **Paso 4. Detectar rostros en el fotograma:**
- **Paso 5. Dibujar rectángulos sobre los rostros detectados:**
- **Paso 6. Añadir texto "null :(" en los rostros detectados:**
- **Paso 7. Mostrar el fotograma procesado:**
- **Paso 8. Liberar los recursos:**



