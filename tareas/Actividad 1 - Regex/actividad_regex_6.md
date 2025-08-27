# Actividad de Regex - Asignaciones por Equipo


## **Equipo 6: Datos Financieros**
**Extracción:** 
1. Crear patrones regex robustos que capturen las variaciones mostradas de montos y datos monetarios
- `$1,234.56 USD`
- `€2.500,75`
- `MXN 15,000.00`
- `$-1,500.25` (negativos)
- `(500.00)` (contabilidad)
- Porcentajes: `12.5%`, `-3.2%`

2. Usar grupos `()` para extraer componentes específicos
3. Probar en regex101.com con el siguiente texto de ejemplo:

El reporte financiero trimestral de InvestmentPro muestra los siguientes movimientos económicos durante el período enero-marzo 2023. Las ventas del primer trimestre alcanzaron $2,450,500.75 USD, representando un incremento del 15.2% comparado con el trimestre anterior que registró $2,100,000.00.

Los gastos operativos incluyen nómina por $850,000.50, renta de oficinas $125,500.00 MXN, y servicios públicos €3,250.75. Los costos de marketing digital representaron $45,678.90, mientras que la consultoría externa costó €8,500.25. Las comisiones de ventas totalizaron $186,750.00, distribuidas entre el equipo comercial.

El análisis de pérdidas y ganancias muestra ingresos por $3,125,000.00 USD contra egresos de $2,875,500.50, resultando en una utilidad neta de $249,499.50. Sin embargo, algunos ajustes contables muestran movimientos negativos: $-125,000.25 por devoluciones, €-2,500.50 por cambios de divisa, y ($85,000.00) por depreciación de activos.

Las inversiones en el portafolio incluyen acciones valoradas en $1,850,000.00 USD, bonos por €750,500.25, y fondos de inversión con $425,000.75. Los rendimientos trimestrales fueron de 8.5%, 12.3%, y 6.7% respectivamente. Algunas inversiones registraron pérdidas: -3.2%, -1.8%, y -5.5%.

Los indicadores de liquidez muestran efectivo disponible de $567,890.25 USD, cuentas por cobrar $789,123.50, y inventario valorado en $234,567.89. Las cuentas por pagar suman $456,789.12, préstamos bancarios $1,250,000.00 MXN, y líneas de crédito utilizadas por €125,750.50.

El presupuesto para el siguiente trimestre contempla ingresos proyectados de $2,750,000.00, gastos estimados de $2,500,000.25, y una meta de utilidad de $250,000.00. Las reservas de contingencia se mantienen en $500,000.00 USD y €100,000.00.

Análisis de márgenes: producto A genera 25.5% de margen, producto B alcanza 18.7%, mientras que producto C registra -2.3% (pérdida). Los costos unitarios son $125.50, $89.25, y $234.75 respectivamente. El precio de venta promedio se mantiene en $456.80 por unidad.

Las proyecciones anuales estiman ventas por $10,500,000.00 USD, con un crecimiento esperado del 22.5%. Los gastos proyectados son $9,250,000.50, buscando una utilidad anual de $1,249,999.50.


---

**Web Scrapping:** Hacer web scrapping para obtener algún texto grande donde puedas aplicar las expresiones del punto anterior y extraer todas las entidades y guardarlas en un dataframe. 

---

**Conceptos adicionales:** Averiguar sobre **Cuantificadores No-Codiciosos (Lazy) `*?, +?, {n,m}?`**
- Investigar y explicar su uso y funcionamiento
- Investigar la diferencia entre `.*` y `.*?`
- Mostrar 3 ejemplos de su uso
- ¿Cómo se podría usar en este ejemplo?
