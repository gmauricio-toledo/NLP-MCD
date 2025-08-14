# Actividad de Regex - Asignaciones por Equipo


## **Equipo 1: Direcciones de Email**
**Extracción:** 
1. Crear patrones regex robustos que capturen las variaciones mostradas
- Subdominios: `usuario@mail.empresa.com.mx`
- Caracteres especiales: `juan.perez+newsletter@gmail.com`
- Números: `support2023@mi-empresa.org`

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

En la empresa TecnoDatos S.A. de C.V., hemos recopilado información de contacto de diversos clientes y proveedores durante el último trimestre. El director general, contactable en director.general@tecnodatos.com.mx, ha solicitado una auditoría completa de nuestra base de datos de contactos.

Nuestro equipo de ventas maneja cuentas principales como maria.rodriguez+ventas@gmail.com y carlos.martinez@subdivisiones.empresa.com. También tenemos contactos internacionales incluyendo support2023@mi-empresa.org y admin@servers.internacional.net. El departamento de marketing utiliza direcciones como newsletter.manager@marketing-digital.mx y promociones@tienda-online.com.mx.

Durante la revisión, encontramos algunas direcciones problemáticas que requieren validación: usuario.test@dominio (sin extensión), @empresa.com (sin usuario), y dirección@.com (dominio incompleto). Sin embargo, las direcciones válidas incluyen jose.perez+trabajo@corporativo.gob.mx, ana.lopez@desarrollo.software.mx, y consultoria2024@negocios-internacionales.org.

El sistema de tickets maneja correos como ticket-12345@soporte.tecnodatos.mx, bug.report@qa.sistemas.com, y feature.request+urgent@desarrollo.apps.mx. Los freelancers registrados incluyen diseñador.web@creativos.mx, developer.senior@programadores.freelance.com, y consultor.bi@datos-analytics.net.

También hemos identificado direcciones de universidades como profesor.investigacion@academica.edu.mx, estudiante.maestria@posgrados.universidad.mx, y biblioteca.digital@recursos.educativos.org.mx. Las organizaciones sin fines de lucro utilizan direcciones como donaciones@fundacion-educativa.org, voluntarios@ayuda.social.mx, y info@organizacion-ambiental.net.

Algunas direcciones corporativas especiales incluyen no-reply@notificaciones.sistema.mx, automated.reports@reportes.empresa.com, y security.alerts+critical@seguridad.tecnodatos.mx. Los departamentos de recursos humanos manejan reclutamiento@talento.humano.mx y nomina.pagos@administracion.corporativa.com.

---

**Web Scrapping:** Hacer web scrapping con Python para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades usando el modulo `re` y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre **Lookahead Positivo `(?=...)`**
- Investigar y explicar su uso y funcionamiento
- Mostrar 3 ejemplos de su uso

