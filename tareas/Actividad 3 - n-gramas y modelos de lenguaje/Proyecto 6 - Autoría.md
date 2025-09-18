### Proyecto 6: Detección de Autoría

**Objetivo**: Desarrollar un sistema para atribución de autoría usando features basados en BOW/TF-IDF y features estilométricos.

**Corpus**:
- Textos de 2-3 autores diferentes, pueden probar con textos escritos por ustedes

**Instrucciones**:
1. Preprocesamiento y limpieza adecuado
2. Extraer features: BOW/TF-IDF (considerar n-gramas de palabras)
3. Agregar features estilométricos, por ejemplo: longitud de oraciones, cantidad y tipo de signos de puntuación, TTR (type token ratio):
 TTR = número_tokens_únicos / número_total_tokens
4. Entrenar al menos dos clasificadores de Machine Learning para distinguir autores
5. Realizar feature importance analysis (mediante los coeficientes de la regresión logísitica, la importancia de features del random forest, ect.)
6. Evaluar con una partición de prueba

**Métricas**:
- Accuracy, F1-Score
- Matriz de confusión
- Probar con algunos textos libres al final

En la presentación incluir limitaciones del modelo, además, averiguar posibles estrategias para abordar estas limitaciones y estrategias más avanzadas que se podrán usar. También incluir cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.