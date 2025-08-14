# Actividad de Regex - Asignaciones por Equipo


## **Equipo 2: Números de Teléfono Internacionales**
**Extracción:** 
1. Crear patrones regex que capturen las variaciones mostradas
- `+52 (664) 123-4567`
- `+1-555-123-4567`
- `(01) 55 1234 5678`
- `664.123.4567`

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

El centro de atención telefónica de GlobalConnect ha procesado miles de llamadas durante el mes pasado. Nuestros registros muestran contactos de México como +52 (664) 123-4567 y +52 55 8765-4321, así como números de Estados Unidos incluyendo +1-555-123-4567 y (555) 987-6543.

Los clientes mexicanos frecuentemente proporcionan números locales como (01) 55 1234 5678, 664.123.4567, y 33-1234-5678. También recibimos llamadas internacionales de España +34 91 123 45 67, Argentina +54 11 4567-8901, y Colombia +57 1 234-5678.

El departamento de ventas maneja números corporativos como 01-800-123-4567 (línea gratuita), +52 (81) 8765-4321, y 33.1234.5678. Algunos registros muestran formatos inconsistentes: 5551234567 (sin formato), +1 555-123-4567 ext. 101, y (555)123.4567.

Los números de emergencia incluyen +52 664 911-2345, +1-911-555-0123, y 066 (México). Contactos de sucursales internacionales: +44 20 7123 4567 (Reino Unido), +81 3-1234-5678 (Japón), y +49 30 12345678 (Alemania).

Registros de call center muestran +52 (33) 3456-7890, 55-1234-5678, y +1 (212) 555-0199. Algunos números problemáticos para validar: 123-45-67 (muy corto), +52-664-123 (incompleto), y (555) 12-345 (formato irregular).

El sistema CRM almacena números como +52 (222) 456-7890, 664 123 4567, y +1.555.123.4567. Números de WhatsApp Business incluyen +52 1 664 123 4567 y +1 (555) 234-5678. Los contactos de proveedores internacionales: +39 06 1234 5678 (Italia), +33 1 42 34 56 78 (Francia), y +86 10 1234 5678 (China).

Números de fax tradicionales: +52 (55) 5555-1234, +1 (555) 555-5555, y 664-555-0123. El departamento de soporte técnico utiliza +52 800 987 6543 y +1-800-SUPPORT (aunque este último no es numérico puro).

---

**Web Scrapping:** Hacer web scrapping para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre **Grupos No-Capturantes `(?:...)`**
- Investigar y explicar su uso y funcionamiento
- Mostrar 3 ejemplos de su uso
- Cuál es la diferencia entre `()` y `(?:)`
- Mostrar cómo agrupar sin crear grupos numerados para optimizar memoria
