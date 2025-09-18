### Proyecto 5: Topic Modeling

**Objetivo**: Implementar y comparar diferentes técnicas de topic modeling aplicadas a un corpus específico.

**Corpus**:
https://drive.google.com/file/d/1b0cmrHesxIXzZhxAEqRizdL8zOFXyK9V/view?usp=sharing

**Instrucciones**:
1. Preprocesamiento
2. Implementar 3 estrategias de topic modelling: 
 * BOW/TFIDF + Clustering
 * LSA (TruncatedSVD)
 * [LDA](https://radimrehurek.com/gensim/models/ldamodel.html) 
3. Calcular métricas de coherencia y silueta (en el caso de clustering) para cada modelo. Ajustar el número de tópicos para mejorar las métricas
4. Presentar las palabrás más frecuentes en cada tópico y dar una interpretación de qué tópico se trata. 
5. Visualizar topics con pyLDAvis o técnicas similares

**Métricas**:
- Coherence scores (u_mass, c_v)
- Silhouette score (para clustering)
- Evaluación humana: calidad e interpretabilidad de topics

**Puntos interesantes**:
- Interpretabilidad vs métricas numéricas
- ¿Qué aplicaciones prácticas tiene estas técnicas?

En la presentación incluir limitaciones del modelo, además, averiguar posibles estrategias para abordar estas limitaciones y estrategias más avanzadas que se podrán usar. También incluir cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.

--- 

Para medir la coherencia de un modelo SVD se puede usar esta adaptación para usar gensim:

```python
from gensim.models import CoherenceModel
import numpy as np
from gensim.corpora import Dictionary  # Asegúrate de importar Dictionary

def coherencia_svd(svd_model, vectorizer, textos_tokenizados, n_palabras=10, use_abs=True):
    feature_names = vectorizer.get_feature_names_out()
    topics = []

    for component in svd_model.components_:
        if use_abs:
            component = np.abs(component) 

        top_words = [feature_names[i] for i in component.argsort()[:-n_palabras-1:-1]]
        topics.append(top_words)

    dictionary = Dictionary(textos_tokenizados)
    coherence_model = CoherenceModel(
        topics=topics,
        texts=textos_tokenizados,
        dictionary=dictionary,
        coherence='c_v'
    )
    return coherence_model.get_coherence()
```

En el caso de clustering, adaptar esta función
