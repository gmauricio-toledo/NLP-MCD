# RAG

El objetivo de esta prácticaes realizar un sistema RAG para responder querys a partir **solamente** de la información presente en algunos archivos. 

## Instrucciones

Cada equipo partirá de una combinación de distintos componentes y podrán mejorar sobre esta. 

* Escoger 3-5 archivos PDF sobre la misma temática libre.
* Definir 3 querys sobre información presente en los textos, manualmente definir las respuestas ground-truth con k=3 (ser lo más precisos posibles con estos).
* Definir 2 querys con información no presente explícitamente en los PDF, una sobre la misma temática y otra sobre una temática muy diferente.

## Equipos

Pareja,Chunking,Embeddings,Vector DB,Retrieval & Reranking,Generation
Fernando-Manuel,CharacterTextSplitter,all-MiniLM-L6-v2,ChromaDB,ContextualCompressionRetriever,LLM
Sebastian-Feliciano,RecursiveCharacterTextSplitter (Alto overlap),BAAI/bge-small-en,FAISS,Solo Similitud,LLM
Jennifer y Kevin,CharacterTextSplitter,all-MiniLM-L6-v2,Milvus Lite,Similitud + Cohere Rerank (vía HF),LLM
Angel-Federico-Jesús,SemanticChunker,BAAI/bge-large-en,LanceDB,EnsembleRetriever (BM25 + Similitud),LLM
Arian-Catherine,RecursiveCharacterTextSplitter (Bajo overlap),BAAI/bge-large-en,ChromaDB,MultiQueryRetriever,LLM
Eddel-Gerardo,SemanticChunker,BAAI/bge-large-en,Milvus Lite,ContextualCompressionRetriever,LLM



## Presentación
- Mostrar capturas donde muestren la(s) línea(s) específicas donde se realiza cada paso: chunking / embeddings / vector DB / retrieve / re-ranking (si aplica) / generation
- Mostrar los resultados con evaluación:
	* Humana para evaluar en general
	* Precision@k para evaluar el retrieval
	* RAGAS para evaluar la generación
- Hablar sobre las variantes probadas, principales dificultades y retos encontrados, así como cualquier aspecto relevante que hayan encontrado o entendido durante el desarrollo del proyecto.
- Considerando este sistema como un *proof of concept* responder a detalle las siguientes preguntas:
	* ¿cómo podrían hacer el deployment? ¿Qué servicio usarían para el LLM? ¿Cómo accederían a la Vector DB? 
	* ¿qué tan escalable es? ¿Qué componente creen que es el principal cuello de botella al escalar?


## Fecha de entrega

Las presentaciones serán el jueves 27 de noviembre (fase 1) y jueves 4 de diciembre (fase 2, por definir). 