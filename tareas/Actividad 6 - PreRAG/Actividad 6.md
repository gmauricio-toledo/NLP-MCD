# Práctica: Information Retrieval con Chunking, Vectorización y Búsqueda Semántica

---

## **Objetivo General**
Implementar un sistema básico de recuperación de información (IR) **sin frameworks complejos** como LangChain o bases de datos vectoriales. La práctica se enfoca en:
1. Dividir documentos largos en chunks (oraciones) usando **spaCy**.
2. Vectorizar los chunks con **embeddings** (ej. `sentence-transformers`) y **BOW/TF-IDF** para comparación.
3. Almacenar los vectores y metadatos en estructuras simples (listas, diccionarios).
4. Implementar una búsqueda por similitud coseno para recuperar los chunks más relevantes a una consulta.
5. Analizar y comparar los resultados entre ambos métodos de vectorización.

---

## **Instrucciones Generales**

### **1. Requisitos Previos**
- **Herramientas:**
  - Librerías: `spacy`, `sentence-transformers`, `scikit-learn`, `numpy`, `pandas`.

- **Documentos:**
  - Se proporcionan 3 documentos sobre un tema específico

---

### **2. Pasos de la Práctica**

#### **Paso 1: Cargar y Preprocesar Documentos**
- **Objetivo:** Leer los documentos y dividirlos en oraciones (chunks) usando spaCy.
- **Tareas:**
  1. Implementar una función `chunk_document(text)` que:
     - Reciba un texto como entrada.
     - Lo divida en oraciones.
     - Filtre oraciones con menos de un umbral de caracteres.
     - Devuelva una lista de oraciones.
  2. Aplicar la función a cada documento y almacenar las oraciones en una lista de listas
  3. Imprimir el número de oraciones por documento para verificación.

---

#### **Paso 2: Vectorización con Embeddings**
- **Objetivo:** Convertir cada oración en un vector denso usando algún modelo de [`sentence-transformers`](https://sbert.net/docs/sentence_transformer/pretrained_models.html#original-models).
- **Tareas:**
  1. Cargar el modelo de embeddings:
  2. Vectorizar todas las oraciones de cada documento y almacenar los vectores en una lista de arrays de numpy:
  3. Verificar la forma de los vectores (debe ser `(n_oraciones, dim)`).

---

#### **Paso 3: Vectorización con BOW/TF-IDF**
- **Objetivo:** Vectorizar las oraciones usando **Bag of Words (BOW)**/**TF-IDF**/**doc2vec** para comparar con los embeddings.
- **Tareas:**
  1. Generar los vectores de las oraciones de cada documento.

---

#### **Paso 4: Almacenar Vectores y Metadatos**
- **Objetivo:** Guardar los vectores (embeddings de sentence-transformers y TF-IDF) junto con sus metadatos en una estructuras de tu preferencia para facilitar la búsqueda.
- **Tareas:**
  1. Crear dos listas de diccionarios:
     - `embeddings_data`: Para almacenar oraciones, embeddings y metadatos.
     - `tfidf_data`: Para almacenar oraciones, vectores TF-IDF y metadatos.
  2. Cada diccionario debe tener la siguiente estructura:

---

#### **Paso 5: Implementar Búsqueda por Similitud**
- **Objetivo:** Implementar funciones para buscar las *k* oraciones más similares a una consulta usando **similitud coseno**.
- **Tareas:**
  1. **Para embeddings:**
     - Implementar `search_with_embeddings(query, k=3)`:
       - Vectorizar la consulta con el mismo modelo de embeddings.
       - Calcular la similitud coseno entre la consulta y todos los vectores almacenados.
       - Devolver los *k* resultados más similares.
  2. **Para BOW/TF-IDF/Doc2Vec:**
     - Implementar `search_with_bow(query, k=3)`:
       - Vectorizar la consulta con el vectorizador TF-IDF ajustado.
       - Calcular la similitud coseno entre la consulta y todos los vectores TF-IDF.
       - Devolver los *k* resultados más similares.

---

#### **Paso 6: Evaluar y Comparar Resultados**
- **Objetivo:** Probar consultas y analizar las diferencias entre los resultados de embeddings y TF-IDF.
- **Tareas:**
  1. Definir al menos **3 consultas** sobre el tema de los documentos:
  2. Ejecutar cada consulta con ambas funciones de búsqueda y mostrar los resultados.
  3. **Preguntas para análisis:**
     - ¿Qué método (embeddings o TF-IDF) recupera resultados más relevantes para cada consulta? ¿Por qué?
     - ¿En qué casos falla cada método?
     - ¿Cómo afecta la longitud de la consulta a los resultados?

---

### **3. Entregables**
1. **Notebook de Colab** con:
   - Todo el código implementado y ejecutado.
   - Salidas de las consultas con ambos métodos.
   - Comentarios explicando cada paso.
2. **Presentación** que incluya:
   - Comparación entre los resultados de embeddings y TF-IDF.
   - Análisis de al menos una métrica de evaluación (ej. precisión@k).
   - Retos, Limitaciones y Propuestas de mejora para el sistema.

---

### **4. Evaluación**
- **Criterios:**
  - Correctitud del chunking y vectorización.
  - Funcionalidad de las funciones de búsqueda.
  - Claridad en la comparación de resultados.
  - Profundidad del análisis en el informe.

---

### **5. Preguntas para Presentación**
1. ¿Cómo afectaría el tamaño del chunk (oración vs. párrafo) a la calidad de los resultados?
2. ¿Qué ventajas tiene usar embeddings sobre TF-IDF en este contexto? ¿Y desventajas?
3. ¿Cómo implementarías un sistema de filtrado por documento o tema antes de la búsqueda?
4. Si quisieras escalar este sistema a miles de documentos, ¿qué cambios harías?

---

**Nota:** Esta práctica está diseñada para ejecutarse **sin frameworks complejos**, con el fin de entender los fundamentos de IR antes de avanzar a RAG.
