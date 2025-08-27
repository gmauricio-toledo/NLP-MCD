# Actividad de Regex - Asignaciones por Equipo


## **Equipo 7: Horarios y Timestamps**
**Extracción:** 
1. Crear patrones regex que capturen las variaciones mostradas de horarios
- `14:30:25` (24h con segundos)
- `2:30 PM`, `10:45 AM` (12h)
- `14:30 hrs`, `09:15 h`
- Timestamps: `2023-12-25 14:30:25`, `25/12/2023 14:30`
- Duración: `2h 30min`, `1:45:30` (hrs:min:seg)

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

El sistema de monitoreo de TechOps registra eventos críticos las 24 horas del día. El servidor principal se reinició el 2023-12-25 14:30:25, seguido por la base de datos que completó su backup a las 23:45:30. Los logs muestran que el sistema de autenticación falló a las 8:15 AM del día siguiente.

Durante la madrugada, específicamente a las 02:30:45, se detectó un pico de tráfico inusual. El equipo de soporte respondió inmediatamente y el incidente se resolvió a las 3:45 AM. El reporte de incidentes documenta una duración total de 1h 15min.

Los procesos batch programados ejecutan diariamente: respaldos a las 01:00 hrs, sincronización de datos a las 04:30 h, y generación de reportes a las 06:15:20. El mantenimiento preventivo se realiza semanalmente los domingos de 2:00 AM a 4:30 AM.

El monitoreo continuo registra timestamps como 2023-12-26 09:15:30 para el inicio de operaciones, 12/26/2023 18:45 para el cierre del sistema de ventas, y 26/12/2023 22:30:15 para la última transacción del día.

Los logs de aplicación muestran sesiones de usuarios: login a las 9:30 AM, actividad hasta las 17:45:30, y logout automático a las 18:00 hrs. El sistema registra tiempos de respuesta promedio de 2.5 segundos, con picos de hasta 8.7 segundos durante las 14:30:00.

Las tareas programadas incluyen: limpieza de archivos temporales cada 2h 30min, verificación de integridad cada 4:15:45, y actualización de índices que toma aproximadamente 1h 45min. El proceso de facturación se ejecuta diariamente a las 23:59:59.

Los reportes de rendimiento muestran horarios pico: 09:00 AM - 11:30 AM (matutino), 14:00 hrs - 16:30 hrs (vespertino), y 19:15 - 21:45 (nocturno). Durante estos períodos, el sistema maneja hasta 1,500 transacciones por minuto.

El equipo de desarrollo registra commits en Git con timestamps como 2023-12-27 10:25:45, deployments a las 15:30:20, y rollbacks ejecutados a las 16:45 PM (formato mixto). Las pruebas automatizadas corren cada 6h 30min comenzando a las 00:00:00.

Los servicios de terceros sincronizan datos: API bancaria cada 1:30:15, servicios de pago cada 45min, y actualizaciones de catálogo que duran 3h 15min. El sistema de notificaciones envía alertas críticas inmediatamente, resúmenes cada 2h, y reportes semanales los viernes a las 17:00 hrs exactamente.

---

**Web Scrapping:** Hacer web scrapping para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre **Grupos Nombrados `(?P<nombre>...)` y `(?P=nombre)`**
- Investigar y explicar su uso y funcionamiento
- Mostrar 3 ejemplos de su uso
