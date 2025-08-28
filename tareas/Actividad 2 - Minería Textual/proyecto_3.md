# Proyecto: Descubrimiento y Perfilado de Tópicos en Documentos

## Objetivo
Desarrollar un sistema que analice una colección de documentos para descubrir sus tópicos subyacentes, crear perfiles lingüísticos detallados para cada tópico y utilizar estos perfiles para clasificar y etiquetar nuevos documentos.

### Objetivos específicos:
- Identificar y perfilar tópicos a partir de patrones lingüísticos en documentos pre-clasificados
- Crear firmas características para cada tópico basadas en:
  - Sustantivos más frecuentes (lematizados)
  - Adjetivos más frecuentes (lematizados)  
  - Patrones gramaticales verbo + Objeto Directo
  - Entidades nombradas más frecuentes (tipo y valor)
- Bautizar cada tópico según su perfil característico
- Clasificar nuevos documentos según los tópicos identificados
- Identificar los tópicos más relevantes en documentos de prueba

## Técnicas Clave a Utilizar
- Tokenización y preprocesamiento de texto
- Eliminación de stop words y limpieza textual
- Lematización con POS tagging
- Part-of-Speech Tagging (etiquetado gramatical)
- Análisis de frecuencia
- Dependency Parsing (análisis de dependencias)
- Reconocimiento de Entidades Nombradas (NER)
- Extracción de patrones gramaticales verbo-objeto
- Análisis de similitud basado en perfiles temáticos

## Entregables

1. Código: Una notebook de Python que incluya:
 - Procesamiento y perfilado de documentos de entrenamiento
 - Creación de firmas características para cada tópico
 - Sistema de clasificación para nuevos documentos
 - Visualización de resultados y perfiles temáticos

2. Presentación: Una presentación breve que explique:
 - La metodología de perfilado de tópicos
 - El funcionamiento del sistema de clasificación
 - Los perfiles generados para cada tópico y su nombrado
 - Resultados de la clasificación en documentos de prueba
 - Análisis de la efectividad del sistema con los documentos de prueba
 - Limitaciones del enfoque y posibles mejoras

Dataset: https://drive.google.com/file/d/1JJesKC1iBsqMBtQyigoBNV8boUR_tJN0/view?usp=drive_link
Para tener el texto completo de cada documento es necesario hacer web scrapping
