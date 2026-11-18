# Aprendizaje Automático Profundo

Este repositorio contiene las implementaciones, análisis y resoluciones de las actividades de la asignatura **Aprendizaje Automático Profundo**. Los proyectos abarcan desde perceptrones multicapa clásicos hasta arquitecturas convolucionales avanzadas y transferencia de aprendizaje.

## Integrantes
* **Coronel, Paula Martina** 
* **Villarroel, Valentina** 

---

## Proyectos y Actividades

### Actividad 2: Redes Neuronales con TensorFlow
Modelo de clasificación binaria para predecir la aprobación escolar basándose en el dataset *Student Performance* (`student-mat.csv`).
* **Tecnologías:** Python, TensorFlow, Keras, Pandas, Plotly.
* **Conceptos aplicados:** 
  * Diseño de Perceptrones Multicapa (MLP) con activación ReLU y Sigmoide.
  * Comparativa de métodos de Descenso de Gradiente (Batch vs. Mini-batch).
  * Evaluación de Funciones de Pérdida (*Binary Cross-Entropy* vs. *MSE*).
  * Análisis de Optimizadores (SGD, RMSprop, Adam).
  * Mitigación de Overfitting mediante regularización $L_2$, Dropout y *Early Stopping*.

### Actividad 3: Entrenando una CNN
Diseño y entrenamiento de Redes Neuronales Convolucionales (CNN) para el reconocimiento de vocales manuscritas del dataset *EMNIST Letters*.
* **Tecnologías:** TensorFlow, Keras, TensorFlow.js, Scikit-learn.
* **Conceptos aplicados:**
  * Extracción de características espaciales mediante capas convolucionales y de *MaxPooling*.
  * Estrategias de robustez: *Data Augmentation* (rotación, desplazamiento, zoom) y regularización por *Dropout*.
  * Optimización mediante *Batch Normalization*.
  * Estudio de ablación arquitectónico para maximizar la exactitud reduciendo los parámetros libres.
  * Exportación de modelos `.h5` a `tfjs` para evaluación en tiempo real sobre un lienzo de dibujo en el navegador (evaluación con escritura propia).

### Actividad 5: Fine-Tuning Supervisado
Aplicación de *Transfer Learning* utilizando la arquitectura **ResNet-18** preentrenada en ImageNet.
* **Tecnologías:** PyTorch, Torchvision.
* **Conceptos aplicados:**
  * **Clasificación base:** Reconocimiento de objetos (Hot Dogs vs. Not Hot Dogs) ajustando la capa de salida fully connected (`fc`).
  * **Problema de dominio médico:** Adaptación de la red para clasificar imágenes de lesiones cutáneas (Equimosis vs. No equimosis).
  * Variación e impacto de la tasa de aprendizaje (*learning rate*) en el congelamiento de capas previas.
  * Evaluación de desempeño en corpus pequeños mediante métricas de Precisión, Recall, F1-Score y matrices de confusión.
