# Proyecto 1: Modelo de Lenguaje con N-gramas



**Objetivo**: Desarrollar un modelo de lenguaje que funcione para autocompletar y generar texto usando n-gramas de palabras.

**Corpus**: 
- Usar un corpus apropiado para los objetivos del proyecto. Incluir, de ser posible, conversaciones de WhatsApp
- Sugerencias: Wikipedia en español (porciones) o noticias
Separar algunos textos para validación

**Instrucciones**:
1. Preprocesar textos: considerar el manejo de emojis 
2. Extraer n-gramas (n=2,3,4) y calcular probabilidades condicionales, usar el token <UNK> para manejar palabras desconocidas en la etapa de la generación de texto. Sugerencia: Usar los tokens <START> y <END> para inicio y final de 
3. Implementar algoritmo de autocompletado que sugiera siguientes palabras a las que se van escribiendo (dar algunas demostraciones en la presentación). Para esto usar las probabilidades estimadas.
4. Generar texto automático comenzando con una semilla  (dar algunas demostraciones en la presentación).

**Métricas**:
- K-Precisión para autocompletado en algunos textos de validación (¿cuántas veces la palabra correcta está en top-k?)
- Perplejidad del modelo en texto de validación (pueden usar el método perplexity de nltk.model.NgramModel)
- Evaluación humana: calidad de las sugerencias y texto generado (escala 1-5)

En la presentación incluir limitaciones del modelo, además, averiguar posibles estrategias para abordar estas limitaciones. También incluir cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.