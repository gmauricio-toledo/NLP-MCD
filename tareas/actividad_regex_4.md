# Actividad de Regex - Asignaciones por Equipo


## **Equipo 4: URLs y Dominios Web**
**Extracción:** 
1. Crear patrones regex que capturen las variaciones mostradas
- `https://www.ejemplo.com/ruta/archivo.html?param=valor`
- `http://subdomain.ejemplo.mx:8080/api/datos`
- `ftp://files.empresa.com/documentos/`
- URLs sin protocolo: `www.ejemplo.com`

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

Durante la auditoría de seguridad web de la empresa CyberSecure, nuestro equipo de análisis identificó múltiples recursos web que requieren evaluación. El sitio principal https://www.cybersecure.com.mx/portal/index.html maneja el tráfico principal, mientras que el sistema de autenticación opera desde https://login.cybersecure.com.mx:8443/auth/signin.

Los microservicios están desplegados en diferentes subdominios: https://api.servicios.cybersecure.mx/v1/usuarios, http://reports.interno.cybersecure.com:3000/dashboard, y https://storage.files.cybersecure.net/documents/secure/. El CDN utiliza URLs como https://cdn.recursos.cybersecure.mx/assets/images/logo.png y https://static.cybersecure.com/css/styles.min.css.

Nuestros partners tienen enlaces a https://partners.cybersecure.com/integration/api/webhook, ftp://files.proveedores.cybersecure.mx/uploads/contracts/, y https://external.colaborators.cybersecure.org:9443/shared/projects. El sistema de respaldos utiliza ftp://backup.cybersecure.com:21/daily_backup/2023-12-25/.

Durante el análisis, encontramos referencias a sitios externos como https://google.com/search?q=cybersecurity, www.microsoft.com/security/business, y github.com/cybersecure/open-source-tools. También identificamos recursos sin protocolo especificado: www.cybersecure.com, mail.cybersecure.mx, y ftp.downloads.cybersecure.net.

Los endpoints de API incluyen https://api.cybersecure.mx/v2/security/scan?target=192.168.1.1&deep=true, http://internal.monitoring.cybersecure.com:8080/metrics/server-status, y https://webhooks.integrations.cybersecure.net/slack/notifications. El sistema de documentación está en https://docs.cybersecure.com/api/reference/authentication.html.

Recursos de desarrollo: https://dev.cybersecure.com:8000/testing/sandbox, http://localhost:3000/development/debug, y https://staging.cybersecure.mx/pre-production/features. El repositorio de código utiliza https://git.cybersecure.com/projects/main-application/repository/commits.

URLs problemáticas detectadas incluyen enlaces rotos como https://old.cybersecure.com/deprecated/service (404), http://unsecure.cybersecure.com/login (sin HTTPS), y ftp://public.cybersecure.com/ (acceso público no deseado).

---

**Web Scrapping:** Hacer web scrapping para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre positive y negative **Lookbehind `(?<=...)` y `(?<!...)`**
- Investigar y explicar su uso y funcionamiento
- Mostrar 3 ejemplos de su uso
- ¿Cómo se podría usar en este ejemplo en particular?
