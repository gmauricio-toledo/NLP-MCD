# Análisis de Sentimientos

* Dataset: !gdown 1gIPIdr-L4vDERiLxp1NALclpFOAn3XGs
* Estrategias:
    1. LLM finetuning con la API Trainer de Transformers
    2. LLM prompting: zero-shot o few-shot
* Métrica de evaluación: F1-Score
* Fecha de Presentaciones: Martes 25 de Noviembre

Puntos importantes a considerar:
* Desbalance de clases
* Tamaño del dataset
* Al final habrá una evaluación con un dataset de prueba, compararemos los modelos. Guardar el mejor modelo de finetuning para hacer predicción y comparar.
* Para esta tarea de fine-tuning con AutoModelForSequenceClassification (o alguna variante si se indica en la documentación). Escoger un modelo con tamaño entre 1B y 10B idealmente. Pueden escoger de más tamaño.

Entregar: 
1. La notebook ejecutada
2. Comparación de resultados con la actividad 5, hacer una tabla ordenada por F1-score
3. Predicciones del conjunto de prueba sin etiquetas en un archivo csv