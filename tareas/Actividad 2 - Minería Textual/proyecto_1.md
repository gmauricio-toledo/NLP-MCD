# Proyecto: Extracción Automática de Acuerdos de Actas

## Objetivo
Desarrollar un script en Python que procese minutas de reuniones en español (en formato PDF) para identificar párrafos que contengan **acuerdos o acciones**, y luego extraer de ellos:
- **El responsable** de la acción.
- **La acción** a realizar (lematizada).
- **La fecha límite** (si se menciona).

## Técnicas Clave a Utilizar
- Expresiones regulares
- Tokenización y Procesamiento Lingüístico con `spaCy`
- Part-of-Speech Tagging
- Dependency Parsing
- Lematización

## Entregables
1.  Código: Una notebook de Python que procese un archivo de texto.
2.  Datos: Al menos **3 actas reales** en formato PDF que servirán como corpus de prueba.
3.  Presentación: Una presentación breve donde expliquen:
    - Funcionamiento del código.
    - Dónde se encontraron las actas.
    - El rendimiento del código en cada una, enlistando éxitos y fracasos.
    - Una discusión sobre las limitaciones del método y qué patrones gramaticales fueron difíciles de capturar.
