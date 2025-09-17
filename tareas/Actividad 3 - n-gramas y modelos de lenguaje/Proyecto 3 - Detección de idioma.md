### Proyecto 3: Detección de Idiomas con N-gramas de Caracteres

**Objetivo**: Crear un detector de idiomas usando n-gramas de caracteres y comparar diferentes enfoques.

**Corpus**:
100 artículos de wikipedia de cada uno de 3 idiomas de su elección (hacer webscrapping)

**Instrucciones**:
1. Extraer n-gramas de caracteres (n=2,3,4), pueden usar el mismo CountVectorizer
2. Crear perfiles de idioma basados en frecuencias de n-gramas. Por ejemplo, en cada idioma mostrar los K n-gramas de carácteres más frecuentes (considera normalizar por la "longitud" de texto)
3. Implementar clasificación por:
   - Similitud coseno con los perfiles del punto anterior (¿con cuál de los 3 perfiles del punto anterior tiene más similitud?) 
   - Modelos de Machine Learning (Logistic Regression, Multinomial Naive Bayes y algún otro de tu elección) con features de n-gramas de carácteres
5. Evaluar con texto de longitud variable (desde palabras sueltas hasta párrafos)

**Métricas**:
- Accuracy por idioma
- Evaluación humana: probar con algunos textos externos, incluye algunos errores ortográficos

**Puntos interesantes**:
- ¿Cómo es la efectividad en textos muy cortos?
- ¿Qué idiomas que se confunden más?


En la presentación incluir limitaciones del modelo, además, averiguar posibles estrategias para abordar estas limitaciones y estrategias más avanzadas que se podrán usar. También incluir cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.