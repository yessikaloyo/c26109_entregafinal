# Impacto de las campañas de RRSS en las ventas

Trabajo Técnico TT26109 — análisis de datos de clientes, ventas y marketing para medir el impacto de las campañas en redes sociales (RRSS) sobre las ventas por producto.

**Estudiante:** Yessika Loyo

## 🔗 Presentación interactiva

**[https://yessikaloyo.github.io/c26109_entregafinal/](https://yessikaloyo.github.io/c26109_entregafinal/)**

Página con los hallazgos e insights del análisis, incluyendo 4 gráficos interactivos de Plotly (KPIs generales, evolución mensual, ventas por producto dentro/fuera de campaña, y ventas vs. costos de marketing).

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `index.html` | Presentación interactiva completa, publicada en GitHub Pages |
| `presentacion_insights.html` | Copia idéntica de `index.html` (misma presentación) |
| `Entrega_Yessika_Loyo_TT26109 (1).ipynb` | Notebook con el análisis completo: EDA, limpieza, agregaciones, ROI/ROAS y visualizaciones |
| `html_fig_kpis.html` | Gráfico Plotly exportado: KPIs generales de la campaña RRSS |
| `html_lineplot.html` | Gráfico Plotly exportado: evolución mensual de venta promedio |
| `html_barplot1.html` | Gráfico Plotly exportado: venta promedio por producto (en campaña vs. fuera de campaña) |
| `html_barplot2.html` | Gráfico Plotly exportado: venta promedio y costo de marketing por producto |

Los 4 archivos `html_*.html` son el material fuente usado para construir la presentación; `index.html` ya los tiene incrustados y no depende de ellos en tiempo de ejecución.

## Resumen de hallazgos

- **Eficiencia de la inversión:** ROAS de 93.52x y ROI de 9,251.85% — la campaña de RRSS retorna muy por encima de su costo (~$150 total).
- **RRSS impulsa volumen, no ticket promedio:** la venta promedio por transacción es similar dentro y fuera de campaña (~$475 vs. ~$490); el retorno viene de mover más unidades.
- **Respuesta desigual por producto:** Microondas, Elementos de cerámica y Heladera se disparan en campaña (+52%, +47%, +28%); Freidora eléctrica, Laptop y Plancha de vapor caen (hasta −60%).
- **Estacionalidad:** pico en marzo, caída sostenida entre junio y septiembre — posible fatiga publicitaria en ese tramo.

Detalle completo de metodología, limpieza de datos e insights ampliados en el notebook y en la presentación interactiva.

## Fuentes de datos

- `clientes`: 567 registros, 5 variables
- `ventas`: 3,035 registros (tras limpieza), 6 variables — precio, cantidad, producto, categoría, fecha de venta
- `marketing`: 90 registros, 6 variables — campañas por canal (TV, RRSS, Email), costo, fechas de inicio/fin
