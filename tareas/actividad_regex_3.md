# Actividad de Regex - Asignaciones por Equipo


## **Equipo 3: Fechas en Múltiples Formatos**
**Extracción:** 
1. Crear patrones regex robustos que capturen las variaciones mostradas
- `25 de diciembre de 2023`
- `Dec 25, 2023`
- `2023-12-25`
- `25/12/23`
- `25.dic.2023`

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

El informe anual de la empresa DataAnalytics correspondiente al período 2023 muestra eventos importantes en diferentes fechas. El proyecto inició el 15 de enero de 2023, con la primera reunión programada para Jan 20, 2023. La fase de desarrollo comenzó oficialmente el 2023-02-01 y el primer entregable se completó el 28/02/23.

Durante marzo, específicamente el 15.mar.2023, se llevó a cabo la presentación a inversionistas. El siguiente hito se alcanzó el 5 de abril de 2023, seguido por una revisión programada para Apr 18, 2023. La implementación del sistema se realizó entre el 2023-05-01 y 15/05/23.

Los reportes mensuales se generan los días 25 de mayo de 2023, Jun 25, 2023, 2023-07-25, y 25/08/23. El equipo de QA completó las pruebas el 10.sep.2023, mientras que la certificación se obtuvo el 20 de septiembre de 2023.

El lanzamiento beta ocurrió el Oct 15, 2023, con feedback recopilado hasta el 2023-11-30. La versión final se liberó el 15/12/23, culminando con la celebración del 25.dic.2023.

Algunas fechas problemáticas aparecen en los logs: 32/01/2023 (día inválido), 15 de febrero de 24 (año abreviado ambiguo), y 2023-13-01 (mes inválido). Sin embargo, fechas válidas adicionales incluyen 1 de marzo de 2023, Mar 1, 2023, 2023-03-01, 01/03/23, y 1.mar.2023.

El cronograma de mantenimiento incluye fechas como 2023-04-15, 30 de abril de 2023, Apr 30, 2023, 30/04/23, y 30.abr.2023. Los eventos de capacitación están programados para 2023-06-10, 25 de junio de 2023, Jun 25, 2023, 25/06/23, y 25.jun.2023.

Los reportes trimestrales se publican el 31 de marzo de 2023, Jun 30, 2023, 2023-09-30, 31/12/23, y fechas similares cada trimestre.

---

**Web Scrapping:** Hacer web scrapping para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre **Backreferences `\1, \2, \3`**
- Investigar y explicar su uso y funcionamiento
- Mostrar 3 ejemplos de su uso
- ¿Cómo podrías usarlos en este problema en particular?
