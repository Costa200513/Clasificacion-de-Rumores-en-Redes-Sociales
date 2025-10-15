# Detección de Rumores con Machine Learning

##  Descripción del Proyecto
Este proyecto implementa un modelo de **Inteligencia Artificial** basado en **Machine Learning supervisado** para predecir si una publicación en redes sociales corresponde a un rumor (`1`) o no (`0`).  
El modelo se entrenó utilizando un conjunto de datos con publicaciones reales y la variable objetivo `is_rumor`.    
Se priorizó una limpieza básica del texto para conservar la estructura original del mensaje sin perder significado.

El objetivo principal fue **construir un clasificador de texto** que, a partir del contenido del mensaje (`text`), pueda determinar la veracidad de la información.

---

##  Proceso de Desarrollo

### 1. Exploración y limpieza de datos
- Se verificó la existencia de valores nulos y duplicados.
- Se eliminaron filas donde la variable `is_rumor` no tenía valor (`dropna`).
- Se normalizó el texto convirtiéndolo a **minúsculas** y eliminando signos de puntuación para mejorar la calidad del entrenamiento.

### 2. División de datos
- Los datos se dividieron en:
  - **Entrenamiento:** 75%
  - **Validación:** 25%

### 3. Modelo utilizado
El modelo seleccionado fue **Logistic Regression**, una técnica de clasificación supervisada adecuada para problemas binarios (rumor/no rumor).  
Se entrenó con los vectores generados a partir del texto y se evaluó con el conjunto de validación.

---

## Resultados Obtenidos

El modelo alcanzó los siguientes resultados en el conjunto de validación:

- **Accuracy:** 91.04 %  
- **F1-score:** 75.98 %  

Estos resultados muestran un rendimiento sólido, con buena capacidad para identificar rumores sin sacrificar la precisión general.

<img width="560" height="218" alt="image" src="https://github.com/user-attachments/assets/86de20fc-560c-41d2-b4b1-804e16586ff3" />


