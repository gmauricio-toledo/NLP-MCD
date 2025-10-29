# Análisis de Sentimientos

* Dataset: !gdown 1gIPIdr-L4vDERiLxp1NALclpFOAn3XGs
* Estrategias:
    1. BOW / TFIDF
    2. Word2vec / FastText / Doc2vec
    3. BERT Finetuning
    4. Embeddings Transformers + Clasificador 
* Métrica de evaluación: F1-Score
* Fecha de Presentaciones: Jueves 30 de Octubre

Puntos importantes a considerar:
* Desbalance de clases
* Tamaño del dataset
* Al final habrá una evaluación con un dataset de prueba, compararemos los modelos. Guardar el mejor modelo de finetuning para hacer predicción en clase y comparar.
* Para esta tarea de fine-tuning con AutoModelForSequenceClassification, deben seleccionar una variante de BERT distinta a `bert-base-uncased`. Algunas opciones válidas incluyen (pero no se limitan a):

    - bert-base-multilingual-uncased (para textos en español o multilinguales),
    - bert-large-uncased (versión más grande del modelo base),
    - distilbert-base-uncased (versión distilada, más ligera),
    - roberta-base (variante optimizada de BERT),
    - xlm-roberta-base (para contextos multilinguales avanzados),
    - bert-base-spanish-wwm-uncased (específico para español).

En la presentación mencionen qué variante eligieron, incluyan una descripción breve.
