# Actividad de Regex - Asignaciones por Equipo


## **Equipo 5: Códigos y Identificadores**
**Extracción:** 
1. Crear patrones regex robustos que capturen las variaciones mostradas
- RFC mexicanos: `ABCD850101ABC`
- Códigos postales: `22000`, `22000-1234`
- Placas de auto: `ABC-12-34`, `1234-XYZ`

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

El sistema de gestión empresarial ManageCore procesa diariamente múltiples tipos de identificadores y códigos. Los empleados registrados incluyen RFC mexicanos como GOMJ850315ABC, PEAM920528XYZ, y ROSA881203DEF. El sistema también maneja códigos postales diversos: 22000, 64000, 01000, y códigos extendidos como 22000-1234 y 64000-5678.

Las placas vehiculares del parque automotriz corporativo incluyen formatos como ABC-12-34, XYZ-99-88, 1234-DEF, y 5678-GHI. Los vehículos más antiguos mantienen placas como 123-ABC-456 y 789-XYZ-012. Algunos códigos de identificación de activos utilizan formato mixto: A1B2C3, X9Y8Z7, y 123-DEF-456.

El departamento de TI maneja códigos de equipos como COMP-2023-001, SRV-PROD-125, y NET-SW-047. Los códigos de proyectos siguen el formato PROJ-DATA-2023, PROJ-WEB-2024, y PROJ-MOBILE-089. Las licencias de software se identifican como LIC-OFFICE-2023-A1B2, LIC-ADOBE-2024-X9Y8, y LIC-ANTIVIRUS-Z7W6.

Códigos postales de sucursales incluyen: 44100 (Guadalajara), 64000 (Monterrey), 01000 (Ciudad de México), y códigos extendidos 44100-2345, 64000-6789, 01000-1111. Algunos códigos internacionales aparecen: 90210, 10001, y M5V 3A8.

Los NIPs de acceso al sistema siguen patrones como 123456, A1B2C3, XYZ123, pero también códigos más complejos: ABC-123-DEF, 999-XYZ-111, y A9B8C7. Códigos de barras de inventario: 1234567890123, 9876543210987, y 5555666677778.

Los identificadores de cliente incluyen CLI-2023-001234, USR-PREMIUM-567890, y CORP-ENTERPRISE-999888. Códigos de facturación: FAC-2023-A001, REC-2023-B999, y NOT-CRED-C555. El sistema de monitoreo genera códigos como MON-ALERT-001, LOG-ERROR-555, y SYS-WARNING-123.

Códigos de seguridad para acceso: SEC-A1B2C3, AUTH-XYZ789, y PASS-123ABC. Identificadores de transacciones bancarias: TXN-2023-1234567, PAY-CARD-9876543, y TRANS-WIRE-5555666.

---

**Web Scrapping:** Hacer web scrapping para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre **Modificadores/Flags `re.IGNORECASE, re.MULTILINE, re.DOTALL`**
- Investigar y explicar los diferentes flags y cuándo usarlos
- Mostrar 3 ejemplos de su uso
- ¿Cómo se podría usar en este ejemplo?
- Mostrar ejemplos prácticos con `re.compile(pattern, flags)`
