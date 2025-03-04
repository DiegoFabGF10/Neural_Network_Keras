# Red Neuronal para Clasificación de Dígitos MNIST

Este proyecto implementa una **red neuronal artificial** en **Keras** para clasificar imágenes del conjunto de datos **MNIST** (dígitos escritos a mano).

##  Características
- **Carga del dataset MNIST** usando `keras.datasets`.
- **Preprocesamiento de datos:** Normalización y conversión de etiquetas a one-hot encoding.
- **Arquitectura de la red neuronal:**
  - Entrada de 28x28 píxeles (784 características).
  - Capa oculta con 512 neuronas y activación ReLU.
  - Capa de salida con 10 neuronas (una por dígito) y activación Softmax.
- **Entrenamiento usando `categorical_crossentropy` como función de pérdida.**
- **Evaluación del modelo con datos de prueba.**

---

##  Requisitos

Asegúrate de tener **Python 3.7 o superior** y las siguientes librerías instaladas:

```bash
pip install numpy matplotlib opencv-python keras tensorflow
```

---

##  Instalación

1. Clona el repositorio:
   ```bash
   git clone https://github.com/DiegoFabGF10/Neural_Network_Keras.git
   cd tu_repositorio
   ```

2. Crea un entorno virtual (opcional pero recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Mac/Linux
   venv\Scripts\activate     # Windows
   ```

3. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```

---

##  Uso

Ejecuta el script principal:

```bash
python main.py
```

Esto cargará los datos de MNIST, entrenará el modelo y evaluará su precisión.

---

## Resultados Esperados

Durante el entrenamiento, se imprimirá la precisión y pérdida en cada época. Después de la evaluación, se espera una precisión superior al **90%** en los datos de prueba.

Ejemplo de salida:

```
Train on 60000 samples
Epoch 1/8
60000/60000 [==============================] - 8s 140us/sample - loss: 0.2304 - accuracy: 0.9311
...
10000/10000 [==============================] - 1s - loss: 0.0768 - accuracy: 0.9786
```

También puedes visualizar una imagen de entrenamiento utilizando OpenCV (`cv2`).


