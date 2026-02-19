# Proyecto Final - Clasificación Liebre vs No-Liebre

## Descripción del Proyecto

Este proyecto tiene como objetivo desarrollar un modelo que permita identificar vehiculos en dos categorías:

- Liebre
- No-Liebre

Se implementaron modelos baseline y un enfoque basado en Autoencoder para evaluar si una representación latente mejora el desempeño del clasificador.

---

##  Objetivos

- Construir modelos de clasificación binaria.
- Comparar el rendimiento entre modelos tradicionales y uno basado en Autoencoder.
- Evaluar métricas como Accuracy, Precision, Recall y F1-score.
- Analizar la interpretabilidad del modelo utilizando SHAP.

---

## Modelos Implementados

1. Logistic Regression
2. Random Forest
3. Autoencoder + MLP

El Autoencoder fue utilizado para reducir dimensionalidad y extraer una representación latente de los datos antes de clasificarlos.

---

## Resultados

Comparación de modelos:

| Modelo                | Accuracy | F1-Score | Recall |
|-----------------------|----------|----------|--------|
| Logistic Regression   | 0.90     | 0.80     | 0.857 |
| Random Forest         | 0.90     | 0.80     | 0.857 |
| Autoencoder + MLP     | 0.83     | 0.67     | 0.714 |

Los modelos baseline mostraron mejor desempeño general que el modelo basado en Autoencoder.

---

## Interpretabilidad

Se utilizó SHAP con Random Forest para analizar la importancia de las variables y entender qué características influyen más en la clasificación.

---

## Tecnologías Utilizadas

- Python
- Scikit-learn
- TensorFlow / Keras
- SHAP
- Matplotlib
- Pandas
- NumPy

---

## Posibles Mejoras

- Aumentar el tamaño del dataset.
- Aplicar data augmentation.
- Ajuste más exhaustivo de hiperparámetros.
- Probar arquitecturas más profundas.
- Aplicar técnicas de balanceo de clases.

---

## Conclusión

El proyecto demuestra que modelos más simples pueden superar arquitecturas más complejas cuando el dataset es reducido. 
Además, resalta la importancia de evaluar no solo el rendimiento, sino también la interpretabilidad del modelo.
