### Proyecto 4: Análisis de Textos Anómalos con Ley de Zipf

**Objetivo**: Analizar textos para detectar anomalías mediante el estudio de distribuciones de frecuencia y la ley de Zipf. Para esto entrenar un clasificador y un detector de anomalías.

**Corpus**:
- 300 Textos normales: scrapping de artículos de wikipedia en inglés. 
- 300 Textos "anómalos": Generar documentos "aleatorios" usando el mismo vocabulario de los textos normales y de longitud similar. Estos documentos son solo secuencias aleatorias de tokens. 

**Instrucciones**:
1. Calcular las frecuencia de tokens para diferentes textos
2. Para cada documento obtener las frecuencias normalizadas de los K tokens más frecuentes:
 
 frecuencia_normalizada = frecuencia_j / sum(frecuencias_top_K)
 
3. Estrategia 1: Representar a cada documento por un vector de tamaño K donde la componente j es la frecuencia normalizada del j-simo token más frecuente del documento. Con estas features entrenar un clasificador binario usando la métrica coseno. 
4. Estrategia 2: Cada documento tiene asociando un conjunto de 100 datos: 

 (log(ranking),log(frecuencia))

 A este conjunto de datos hacerle regresión lineal para obtener la pendiente y el coeficiente R^2. Además, de cada documento mide el TTR (type token ratio):

 TTR = número_tokens_únicos / número_total_tokens

 Ahora cada documento está representado por 3 features: (pendiente, R^2, TTR). Entrena un clasificador binario y un detector de anomalías (por ejemplo Isolation Forest).


**Métricas**:
- Accuracy
- Matriz de confusión
- F1 score


**Puntos interesantes**:
- Presentar algunos textos que se clasifican como normales pero son anómalos
- Genera un gráfico 3d para la estrategía 2.
- Genera un documento Lorem ipsum y pásalo por tus clasificadores para ver si es lenguaje natural o no.
- Aplica tu clasificador a un documento que consista de código de programación
- Aplica tu clasificador a un documento que sea SPAM muy claro

En la presentación incluir limitaciones del modelo, además, averiguar posibles estrategias para abordar estas limitaciones y estrategias más avanzadas que se podrán usar. También incluir cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.