### Proyecto 2: Clasificación de Sentimiento con BOW/TF-IDF

**Objetivo**: Implementar un clasificador de sentimientos usando representaciones BOW/TF-IDF con diferentes n-gram ranges y comparar clasificadores de Machine Learning.

**Corpus**: 
- https://www.kaggle.com/datasets/ibrahimqasimi/imdb-50k-cleaned-movie-reviews
Uno de los retos es el tamaño del corpus, recordar las sugerencias de las presentaciones pasadas para atender esta situación.

**Instrucciones**:
1. División Train/Test (prestar atención a la distribución de clases) y Preprocesamiento
3. Crear features con CountVectorizer y TfidfVectorizer (probar ngram_range=(1,1), (1,2), (1,3)). Ajustar el hiperparámetro `max_features`.
4. Entrenar y evaluar: Logistic Regression (LR), Naive Bayes Multinomial (NB), Red MLP
5. Optimizar hiperparámetros, en la medida de lo posible en cada caso. 
6. Analizar features más importantes para cada modelo (LR y NB), presentar a qué n-gramas/tokens se refieren. 


**Métricas**:
- Accuracy, F1-score
- Matriz de confusión
- Evaluación humana: 100 muestras aleatorias, identificar patrones de error

**Puntos interesantes**:
- Interpretabilidad de modelos vs performance
- Palabras más influyentes en la decisión

En la presentación incluir limitaciones del modelo, además, averiguar posibles estrategias para abordar estas limitaciones y estrategias más avanzadas que se podrán usar. También incluir cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.