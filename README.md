# Superstore Sales Analysis - Power BI Dashboard

Dashboard ejecutivo multi-página construido en Power BI, analizando 
el dataset público "Superstore" de Kaggle (9,994 registros de ventas 
retail en EE.UU., 2014-2017).

## Objetivo
Analizar ventas, ganancias y comportamiento de clientes para identificar 
oportunidades de mejora en rentabilidad.

## Contenido del dashboard
1. **Dashboard Ejecutivo** — KPIs generales, ventas por mes/categoría, profit por región
2. **Análisis de Productos** — Top productos por ventas/ganancia, productos no rentables
3. **Clientes** — Top clientes por compras y profit, ventas por segmento
4. **Geografía** — Mapa interactivo, ventas por ciudad/estado
5. **Tendencias** — Evolución de ventas y profit por año/trimestre/mes
6. **Descuentos** — Impacto del descuento en ventas y rentabilidad

## Insights clave
- El margen de ganancia real es ~12.5% (validado contra el dataset original)
- A mayor descuento (>20%), la ganancia cae drásticamente e incluso 
  se vuelve negativa
- [Otros hallazgos que encontraste — producto top, cliente top, etc.]

## Herramientas utilizadas
- Power BI Desktop
- DAX (SUM, DISTINCTCOUNT, DIVIDE, TOPN, MAXX)
- Power Query (limpieza de datos, corrección de tipos regionales)

## Proceso de limpieza de datos
Durante la importación del CSV, Power Query interpretó mal los 
separadores decimales debido a la configuración regional del sistema, 
inflando las métricas de Sales y Profit hasta ~6000x. Se diagnosticó 
y corrigió ajustando el tipo de dato con configuración regional 
"English (United States)" en Power Query.

## Dataset
[Superstore Dataset - Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

## Cómo ver el dashboard
Descarga el archivo `.pbix` y ábrelo con Power BI Desktop 
(gratuito, disponible para Windows).
