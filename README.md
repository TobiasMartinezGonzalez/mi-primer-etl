
# Mi Primer ETL con Python

## Descripción
Pipeline ETL que procesa datos de e-commerce para generar métricas de ventas.

## Cómo correr
```bash
pip install pandas pyarrow
python etl.py
```

## Decisiones de limpieza
- **Nulos**: No había datos nulos importantes, rellené los nulos en notes y promotion_id con 0.
- **Duplicados**: Eliminé filas duplicadas en el dataset de ordenes
- **Tipos**: Convertí order_date a datetime

## Output
- `ventas_por_cliente.csv`: Total gastado y cantidad de órdenes por cliente
- `ventas_por_mes.csv`: Ventas totales por mes
- `orders_clean.csv`: Dataset limpio
- También se descargaron los 3 datasets en formato parquet

## Autor
Tobias Martinez Gonzalez - 29/04/2026
