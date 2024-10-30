# Trabajo-Academico-IA
Trabajo academico del curso Inteligencia Artifical (1INF24)

# Predicción de Aterrizajes Seguros para Cohetes SpaceX con Modelos de Machine Learning

La reutilización de cohetes es crucial para reducir costos en la industria aeroespacial. SpaceX ha avanzado significativamente en este campo, recientemente logrando la captura del propulsor Super Heavy mediante los brazos de la torre Mechazilla. Sin embargo, mejorar la precisión y seguridad en los aterrizajes sigue siendo un desafío, que requiere el desarrollo de modelos predictivos capaces de anticipar el éxito de cada recuperación. Estos modelos permiten optimizar el uso de recursos y reducir los riesgos asociados a cada misión.

Este proyecto aborda este reto mediante el desarrollo de un modelo de machine learning que predice el éxito en el aterrizaje de la primera etapa de los cohetes Falcon 9 de SpaceX, utilizando datos históricos de lanzamientos.

![](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-DS0701EN-SkillsNetwork/api/Images/landing_1.gif)

## Descripción del Proyecto

El problema se plantea como una **tarea de clasificación binaria**: dado un conjunto de variables técnicas y ambientales de cada lanzamiento, el modelo debe predecir si el aterrizaje será exitoso (`1`) o fallido (`0`). Este enfoque permite analizar los factores críticos que contribuyen al éxito de los aterrizajes y optimizar las operaciones de recuperación de cohetes.

### Características Principales del Proyecto

1. **Recolección y Preprocesamiento de Datos**:
   - Los datos incluyen información detallada de cada lanzamiento de SpaceX, como el número de vuelo, la masa de la carga útil y la configuración específica del cohete.
   - Las características numéricas fueron estandarizadas para asegurar una escala uniforme entre todas las variables.

2. **Evaluación de Múltiples Algoritmos de Machine Learning**:
   - Se probaron cuatro algoritmos principales de clasificación: **Logistic Regression**, **Support Vector Machine (SVM)**, **Decision Tree Classifier**, y **K-Nearest Neighbors (KNN)**.
   - Para cada uno de estos algoritmos, se utilizó `GridSearchCV` para realizar una búsqueda exhaustiva de los mejores hiperparámetros. Este proceso permitió optimizar el rendimiento de cada modelo, ajustando parámetros específicos como la regularización en Logistic Regression, el kernel en SVM, la profundidad máxima en árboles de decisión y el número de vecinos en KNN.

3. **Comparación y Selección del Mejor Modelo**:
   - Después de optimizar cada modelo, se evaluaron y compararon en términos de precisión y rendimiento general en el conjunto de prueba.
   - El modelo con mejor desempeño final fue seleccionado para la implementación, asegurando así el equilibrio óptimo entre precisión y generalización en la predicción del éxito de los aterrizajes.

### Resultados

El proyecto logró desarrollar un modelo de machine learning confiable y preciso en la predicción del éxito de los aterrizajes de los cohetes Falcon 9. La comparación exhaustiva entre modelos permitió seleccionar el más adecuado para este propósito, basado en su rendimiento en el conjunto de prueba.

## Requisitos

- **Python 3.7+**
- **Librerías necesarias**:
  - `pandas`
  - `scikit-learn`
  - `matplotlib`

## Autores

- **Durán Castañeda, Rómulo Guillermo**
- **Rosales Ventocilla, Christian Leonardo**
- **Carrillo Arbusto, Christian Edgardo**
- **Alamo Calderon, Renzo Marcelo**
- **Chávez Sánchez, Ángel Aarón**
