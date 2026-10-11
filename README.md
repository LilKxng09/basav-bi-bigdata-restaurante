# Solución BI y Big Data para el análisis de ventas de un restaurante

Proyecto final – Base de Datos Avanzadas y Big Data (NRC 7262), periodo 2026-2.
Universidad Privada del Norte – Ingeniería de Sistemas Computacionales.

**Docente:** Hugo Alejandro Mamanchura Lima

**Equipo:** Arroyo Luna, David Orestes · Chavarry Miranda, Brenda Fiorella · Lucas Marmolejo, Erick Giordano · Taipe Figueroa, Jhon Victor

## Contenido

| Carpeta | Contenido |
|---|---|
| `sql/` | Script SQL Server: BD_PUNTOVENTA, Data Warehouse, datos de prueba, ETL y validación |
| `powerbi/` | `puntoventa.pbix`: modelo, medidas DAX y dashboard |
| `bigdata/` | `BigData_PySpark_Restaurante.ipynb`: datos sintéticos, pandas vs. Spark, Parquet |
| `docs/` | Informe, capturas del dashboard y resultados del experimento |

## Cómo reproducir

1. **Base de datos y DW:** en SQL Server, ejecutar el script de `sql/` completo (crea BD_PUNTOVENTA, carga datos de prueba, dimensiones y hechos). La última consulta muestra los conteos esperados: 5 / 5 / 3 / 3 / 2 / 3 en dimensiones, 9 ventas y 6 pagos.
2. **Dashboard:** abrir `powerbi/puntoventa.pbix` en Power BI Desktop y actualizar la conexión a la instancia local de SQL Server.
3. **Big Data:** abrir `bigdata/ProyectoFinal_BigData_PySpark.ipynb` en Google Colab y ejecutar todas las celdas. Genera datos sintéticos (semilla 42) de 10 000, 100 000 y 1 000 000 de filas, y compara pandas con Spark en modo local.

## Dependencias

SQL Server, Power BI Desktop, Google Colab (Python 3, PySpark, pandas, pyarrow).

## Datos

Los datos son de prueba y sintéticos. No incluyen credenciales ni datos personales reales.

## Versión

La versión final evaluada está marcada con la etiqueta `v1.0-final`.
