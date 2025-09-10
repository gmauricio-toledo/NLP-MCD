# Proyectos de N-gramas para Curso de NLP

## **Proyecto 1: Autocompletado/Generación de Texto**

### Objetivos Específicos:
- Implementar predicción de siguiente palabra usando n-gramas
- Desarrollar un generador de texto básico con sampling probabilístico
- Crear un chatbot simple entrenado con conversaciones personales
- Comparar diferentes valores de n (bigrama vs trigrama vs 4-grama)

### Contenido Teórico:
- Probabilidades condicionales P(w_n|w_1...w_{n-1})
- Técnicas de sampling: greedy vs probabilístico vs top-k
- Manejo de contexto y memoria limitada
- Evaluación con perplejidad

### Tareas Específicas:
1. **Autocompletado básico**: Dado "el gato come", predecir siguiente palabra
2. **Generación de párrafos**: Generar 50 palabras desde semilla "hoy voy a"
3. **Chatbot personal**: Entrenar con conversaciones de WhatsApp y crear bot que responda preguntas
4. **Análisis comparativo**: Evaluar calidad de texto generado con n=2,3,4
5. **Evaluación**: Calcular perplejidad y hacer "Turing test personal"

---

## **Proyecto 2: Detección de Idiomas**

### Objetivos Específicos:
- Construir clasificador de idiomas usando n-gramas de caracteres
- Entender cómo patrones estadísticos identifican lenguas
- Manejar casos edge: code-switching, palabras prestadas, textos cortos
- Evaluar precisión con métricas de clasificación

### Contenido Teórico:
- N-gramas de caracteres vs palabras
- Distribuciones de probabilidad por idioma
- Clasificación por máxima verosimilitud
- Manejo de vocabulario no visto (smoothing)

### Tareas Específicas:
1. **Extractor de trigramas**: Implementar extracción de 3-gramas de caracteres
2. **Entrenamiento multilingüe**: Crear modelos para español, inglés, francés
3. **Clasificador**: Implementar detección por perplejidad mínima
4. **Casos complejos**: Probar con mensajes bilingües de WhatsApp
5. **Evaluación**: Matriz de confusión y análisis de errores típicos

---

## **Proyecto 3: Detección de Texto Anómalo**

### Objetivos Específicos:
- Identificar mensajes "extraños" usando perplejidad alta
- Aplicar ley de Zipf para detectar distribuciones inusuales
- Clasificar tipos de anomalías: spam, código, idiomas mezclados
- Establecer umbrales de detección apropiados

### Contenido Teórico:
- Perplejidad como medida de "sorpresa" del modelo
- Ley de Zipf y distribuciones de frecuencia esperadas
- Detección de outliers estadísticos
- Trade-off entre sensibilidad y especificidad

### Tareas Específicas:
1. **Calculadora de perplejidad**: Implementar cálculo para mensajes individuales
2. **Análisis de Zipf**: Graficar distribución de n-gramas y detectar desviaciones
3. **Detector de anomalías**: Clasificar mensajes como normales/anómalos usando umbral
4. **Categorización**: Distinguir entre tipos de anomalías (spam vs código vs idioma)
5. **Evaluación**: Precisión/recall en dataset etiquetado manualmente

---

## **Proyecto 4: Detección de Autoría**

### Objetivos Específicos:
- Identificar patrones únicos de escritura usando n-gramas
- Distinguir entre diferentes autores/personas

### Contenido Teórico:
- N-gramas como features discriminativos
- Medidas de similitud entre distribuciones
- Consideraciones éticas de identificación automática

### Tareas Específicas:
1. **Extractor de features**: Crear vectores de n-gramas característicos por persona
2. **Clasificador de autoría**: Distinguir entre 3-5 personas usando sus conversaciones
3. **Análisis temporal**: ¿Cambia el estilo de escritura con el tiempo?
4. **Experimento ciego**: Identificar autor de mensajes anónimos
5. **Análisis de privacidad**: ¿Qué tan fácil es identificar personas por su escritura?

---

## **Proyecto 5: Análisis de Sentimientos**

### Objetivos Específicos:
- Construir clasificador de emociones usando n-gramas como features
- Comparar enfoque de diccionario vs machine learning supervisado
- Analizar patrones emocionales en conversaciones personales
- Manejar casos ambiguos y context-dependent sentiment

### Contenido Teórico:
- N-gramas como indicadores emocionales
- Polaridad y intensidad de sentimientos
- CountVectorizer y representación sparse
- Comparación: rule-based vs supervised learning

### Tareas Específicas:
1. **Etiquetado manual**: Clasificar 200 mensajes propios como positivos/negativos/neutrales
2. **Diccionario de sentimientos**: Crear diccionarios de n-gramas emocionales, usar diccionarios
3. **Clasificador supervisado**: Entrenar modelo usando CountVectorizer + LogisticRegression
4. **Análisis comparativo**: Evaluar ambos enfoques y analizar discrepancias
5. **Patrones personales**: Identificar n-gramas únicos de emociones en conversaciones propias