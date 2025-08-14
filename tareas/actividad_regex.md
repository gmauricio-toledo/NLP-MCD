# Actividad de Regex - Asignaciones por Equipo

## **Equipo 1: Direcciones de Email Complejas**
**Extracción:** Emails con variaciones complejas incluyendo:
- Subdominios: `usuario@mail.empresa.com.mx`
- Caracteres especiales: `juan.perez+newsletter@gmail.com`
- Números: `support2023@mi-empresa.org`

**Concepto adicional:** **Lookahead Positivo `(?=...)`**
- Investigar y explicar cómo usar lookahead para validar que un email tenga al menos un punto en el dominio
- Ejemplo: `\w+@\w+(?=\.\w+)`

---

## **Equipo 2: Números de Teléfono Internacionales**
**Extracción:** Teléfonos en múltiples formatos:
- `+52 (664) 123-4567`
- `+1-555-123-4567`
- `(01) 55 1234 5678`
- `664.123.4567`

**Concepto adicional:** **Grupos No-Capturantes `(?:...)`**
- Investigar la diferencia entre `()` y `(?:)`
- Mostrar cómo agrupar sin crear grupos numerados para optimizar memoria

---

## **Equipo 3: Fechas en Múltiples Formatos**
**Extracción:** Fechas en formatos variados:
- `25 de diciembre de 2023`
- `Dec 25, 2023`
- `2023-12-25`
- `25/12/23`
- `25.dic.2023`

**Concepto adicional:** **Backreferences `\1, \2, \3`**
- Investigar cómo usar backreferences para encontrar patrones repetidos
- Ejemplo: detectar fechas duplicadas o formatos consistentes

---

## **Equipo 4: URLs y Dominios Web**
**Extracción:** URLs completas incluyendo:
- `https://www.ejemplo.com/ruta/archivo.html?param=valor`
- `http://subdomain.ejemplo.mx:8080/api/datos`
- `ftp://files.empresa.com/documentos/`
- URLs sin protocolo: `www.ejemplo.com`

**Concepto adicional:** **Lookbehind `(?<=...)` y `(?<!...)`**
- Investigar positive y negative lookbehind
- Ejemplo: extraer dominios que NO estén precedidos por "www."

---

## **Equipo 5: Códigos y Identificadores**
**Extracción:** Diferentes tipos de códigos:
- RFC mexicanos: `ABCD850101ABC`
- Códigos postales: `22000`, `22000-1234`
- Placas de auto: `ABC-12-34`, `1234-XYZ`
- NIPs/códigos: `A1B2C3`, `123-ABC-456`

**Concepto adicional:** **Modificadores/Flags `re.IGNORECASE, re.MULTILINE, re.DOTALL`**
- Investigar los diferentes flags y cuándo usarlos
- Mostrar ejemplos prácticos con `re.compile(pattern, flags)`

---

## **Equipo 6: Datos Financieros**
**Extracción:** Montos y datos económicos:
- `$1,234.56 USD`
- `€2.500,75`
- `MXN 15,000.00`
- `$-1,500.25` (negativos)
- `(500.00)` (contabilidad)
- Porcentajes: `12.5%`, `-3.2%`

**Concepto adicional:** **Cuantificadores No-Codiciosos (Lazy) `*?, +?, {n,m}?`**
- Investigar la diferencia entre `.*` y `.*?`
- Ejemplo práctico: extraer contenido entre etiquetas

---

## **Equipo 7: Horarios y Timestamps**
**Extracción:** Horarios en diferentes formatos:
- `14:30:25` (24h con segundos)
- `2:30 PM`, `10:45 AM` (12h)
- `14:30 hrs`, `09:15 h`
- Timestamps: `2023-12-25 14:30:25`, `25/12/2023 14:30`
- Duración: `2h 30min`, `1:45:30` (hrs:min:seg)

**Concepto adicional:** **Grupos Nombrados `(?P<nombre>...)` y `(?P=nombre)`**
- Investigar cómo crear y usar grupos nombrados
- Ejemplo: `(?P<hora>\d{1,2}):(?P<minuto>\d{2})` para extraer horas y minutos por nombre

---

## **Instrucciones Generales:**

### **Para la extracción:**
1. Crear patrones regex robustos que capturen las variaciones mostradas
2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con texto de ejemplo
4. Mostrar código Python funcional con `re.findall()` o `re.search()`

