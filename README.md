# Detección de Neumonía mediante Redes Neuronales Convolucionales (CNN)

## Descripción
Este proyecto implementa una Red Neuronal Convolucional (CNN) para la clasificación de imágenes médicas (radiografías de tórax) con el objetivo de detectar casos de neumonía. Se trata de un problema de clasificación binaria entre pacientes sanos y pacientes con neumonía.

---

## Dataset
- **Fuente de datos:** MedMNIST (concretamente PneumoniaMNIST)  
- **Tipo de datos:** Imágenes médicas (radiografías de tórax) de 28x28 píxeles, en blanco y negro
- **Problema:** Clasificación binaria (Sano vs Neumonía)  

---

## Tecnologías utilizadas
- Lenguaje de programación: Python  
- Librerías empleadas: PyTorch, Scikit-learn, Matplotlib  

---

## Metodología

### 1. Preparación de los datos
- Carga del dataset  
- Normalización y transformación a tensores  
- Exploración básica de las imágenes  

### 2. Arquitectura del modelo
- Red neuronal convolucional (CNN)  
- Capas convolucionales y de pooling  
- Capas fully connected para clasificación  

### 3. Entrenamiento
- Función de pérdida: CrossEntropyLoss  
- Optimizador: Adam  
- Entrenamiento durante múltiples épocas. Selección del mejor hiperparámetro con validación cruzada one round

### 4. Evaluación
- Evaluación sobre conjunto de test  
- Métricas utilizadas:
  - Accuracy  
  - Recall/Sensibilidad (especialmente relevante en este problema)  
  - Matriz de confusión  

---

## Resultados

- **Accuracy:** 85.90%  
- **Recall (Neumonía):** 98.72%  

> El modelo muestra buena capacidad para identificar casos de neumonía, siendo especialmente importante minimizar falsos negativos en este tipo de aplicaciones médicas.

---

## Aprendizajes clave
- Implementación práctica de redes neuronales convolucionales  
- Trabajo con datasets de imágenes médicas  
- Evaluación de modelos en contextos donde la sensibilidad la métrica crítica
- Interpretación de resultados en problemas reales  

---

## Posibles mejoras
- Ajuste de arquitectura mayor
- Data augmentation  
- Uso de arquitecturas más avanzadas (ResNet, transfer learning) 

---

