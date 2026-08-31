# Proyecto 1: Análisis Exploratorio de Datos — Online Retail

## Problema / Pregunta de negocio
Una tienda online del Reino Unido necesita entender su desempeño de ventas: ¿qué productos y países generan más ingresos, cómo varían las ventas en el tiempo, y qué perfil tienen sus clientes más valiosos?

## Datos
- **Fuente:** [Online Retail Dataset — UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/352/online+retail)
- **Periodo:** diciembre 2010 – diciembre 2011
- **Tamaño:** ~540,000 transacciones
- **Columnas:** número de factura, código y descripción de producto, cantidad, fecha de factura, precio unitario, ID de cliente, país

## Proceso
1. Inspección inicial: tipos de datos, valores nulos, estadísticas descriptivas
2. Limpieza: separación de devoluciones (cantidades negativas), eliminación de precios en cero, creación de columna de monto total
3. Análisis exploratorio: ventas por país, productos más vendidos, estacionalidad mensual, clientes más valiosos
4. Conclusiones

## Herramientas
Python (pandas, matplotlib, seaborn), Jupyter Notebook

## Hallazgos clave

- Hallazgo 1: **País líder en ventas:** Reino Unido concentra el 84.61% de las ventas totales, con aproximadamente £9.03 millones de los £10.67 millones en ventas positivas. Esto muestra una fuerte concentración de las ventas en el mercado británico y podría representar una oportunidad para analizar el potencial de otros mercados.
- Hallazgo 2: **Estacionalidad:** Las ventas muestran su mayor pico en noviembre de 2011, con aproximadamente £1.51 millones. También se observa un crecimiento en los meses anteriores. Este comportamiento podría estar relacionado con un aumento de las compras previo a la temporada navideña, aunqie sería necesario contar con información adicional para confirmar esta hipótesis.
- Hallazgo 3: **Devoluciones:** Las devoluciones representan el 1.96% de las líneas del dataset. Sin embargo, su impacto económico es mayor, ya que el valor de las devoluciones alcanza aproximadamente £896,812, equivalente al 8.41% del valor de las ventas positivas. La mayoría de las líneas de devolución corresponden al Reino Unido (86.52%), aunque esto también está relacionado con el peso de este país en las ventas totales.
- Hallazgo 4: **Concentración de clientes:** Las devoluciones representan el 1.96% de las líneas del dataset. Sin embargo, su impacto económico es mayor, ya que el valor de las devoluciones alcanza aproximadamente £896,812, equivalente al 8.41% del valor de las ventas positivas. La mayoría de las líneas de devolución corresponden al Reino Unido (86.52%), aunque esto también está relacionado con el peso de este país en las ventas totales.


## Cómo reproducir este análisis
1. Descarga el dataset desde el link de arriba (formato .xlsx)
2. Coloca el archivo en esta misma carpeta con el nombre `online_retail.xlsx`
3. Abre `EDA_Online_Retail.ipynb` en Jupyter Notebook o Google Colab
4. Ejecuta las celdas en orden

## Próximos pasos del proyecto
Este proyecto se conecta con el Proyecto 2 (SQL) y el Proyecto 3 (dashboard en Power BI/Tableau) usando el mismo dataset, para mostrar el ciclo completo de análisis.
