# Regresan los usuarios de RappiPlus

## Descripción del proyecto

Este proyecto evalúa la retención y el comportamiento de los clientes del servicio **RappiPlus** tras su periodo de prueba. El análisis busca identificar la etapa del embudo de conversión (*funnel*) con mayor pérdida (*drop*) de usuarios, medir el impacto financiero (ingresos vs. pérdidas en ventas) y validar cuantitativamente si las mejoras implementadas influyeron en la atracción de clientes.

---

## Objetivos principales

1. **Limpieza y preparación de datos:** Procesar y homogenizar 3 datasets con Python, tratando valores faltantes por categoría y mitigando el efecto de *outliers* extremos en ventas.
2. **Análisis de embudo y cohortes:** Evaluar mediante SQL los puntos críticos de fuga de clientes y analizar el comportamiento de recompra a lo largo del tiempo.
3. **Validación estadística:** Realizar una prueba Z (*Z-test*) en un experimento A/B para determinar si el incremento de clientes tuvo significancia estadística o se debió al azar.
4. **Visualización estratégica:** Diseñar un *dashboard* interactivo en Power BI para explorar las ventas, costos y métricas de conversión a detalle.

---

## Estructura del repositorio

* `data/` : Carpeta con los conjuntos de datos originales y procesados. *(Ajusta si los nombres son distintos)*
* `scripts/` : Scripts de Python para limpieza, tratamiento de *outliers* y prueba estadística Z.
* `queries/` : Consultas SQL empleadas para el análisis del *funnel* de conversión y cohortes.
* `dashboard/` : Archivo `.pbix` de Power BI con el informe interactivo de ventas e ingresos.

---

## Tecnologías utilizadas

* **Python:** Limpieza de datos, tratamiento de *outliers* e imputación de nulos.
* **SQL:** Análisis del embudo de conversión (*funnel*) y comportamiento de cohortes.
* **Prueba Estadística (Prueba Z):** Evaluación de hipótesis en experimento A/B.
* **Power BI:** Creación de *dashboard* dinámico para visualización de ventas e ingresos.

---

## Visualizaciones clave y hallazgos

### Principales Hallazgos
* **Punto crítico de fuga:** El paso del *checkout* al pago presentó la mayor pérdida de usuarios en el embudo.
* **Productos deficitarios:** Se detectó un producto cuyas ventas generaban pérdidas netas debido a que sus costos superaban el precio de venta (*revenue*).

### Recomendaciones / Lecciones
* **Optimización de pago:** Revisar el flujo o la pasarela de pagos para identificar fricciones técnicas o errores en la plataforma que reduzcan la tasa de abandono (*drop*).
* **Control de precios:** Implementar un sistema de control al momento de fijar precios para evitar la comercialización de productos con márgenes negativos.

> *(Aquí puedes insertar imágenes o capturas de tu dashboard de Power BI o gráficos)*
> `![Dashboard Power BI](link-o-ruta-de-tu-imagen.png)`
