# Clasificación de Imágenes con Red Neuronal Convolucional (CNN)

En este proyecto se entrena una red neuronal convolucional usando TensorFlow / Keras para clasificar imágenes de gatos y perros.

Se entrena un modelo CNN, se evalúa su rendimiento y después se mejora usando data augmentation y dropout para reducir el overfitting.

---

## Objetivo

- Entrenar una CNN para clasificar imágenes
- Evaluar el rendimiento del modelo
- Reducir overfitting
- Probar data augmentation
- Probar dropout

---

## Dataset

Se usa el dataset de **cats vs dogs**.

Las imágenes están separadas en carpetas:

- train/
- validation/

Cada carpeta contiene:
- cats/
- dogs/

Las etiquetas son:

- 0 → gato
- 1 → perro

---

## Preparación de datos

Se usa `ImageDataGenerator` para cargar las imágenes.

Se normalizan los valores dividiendo por 255.

```python
ImageDataGenerator(rescale=1./255)
