# Retail Analytics Pipeline
**Evaluación Módulo 9 — Fundamentos de Big Data | Alkemy**

Pipeline integral de Big Data y Machine Learning sobre datos de e-commerce, implementado con Apache Spark / PySpark en Google Colab.

---

## Tecnologías
- Apache Spark 3.5 · PySpark · Spark SQL · Spark MLlib · Python 3.10
- Entorno: Google Colab

## Dataset
[Online Retail II — UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail+II)  
~1,067,371 transacciones de un e-commerce del Reino Unido (2009–2011).

---

## Contenido del notebook

| Lección | Contenido |
|---|---|
| L1 | Fundamentos de Big Data — 5V y arquitectura RetailMax |
| L2 | Configuración SparkSession — carga inicial en RDDs |
| L3 | RDDs, transformaciones (map, filter, flatMap) y acciones — linaje y DAG |
| L4 | DataFrames, Spark SQL, métricas RFM, guardado en Parquet |
| L5 | Pipeline MLlib: Regresión Logística + K-Means (k=4) |

---

## Cómo ejecutar

1. Abrir `retail_analytics_pipeline.ipynb` en Google Colab
2. Ejecutar todas las celdas en orden (Runtime → Run all)
3. El notebook descarga el dataset automáticamente desde UCI
4. Los archivos de salida se generan en la carpeta `output/`

> Para guardar los outputs en Google Drive, montar Drive antes de ejecutar:
> ```python
> from google.colab import drive
> drive.mount('/content/drive')
> ```

---

## Resultados principales

- **Clientes analizados:** 5,875
- **Segmentos K-Means:** 4 grupos (Base activa, Leales, En riesgo, Champions)
- **Modelo supervisado:** Regresión Logística para clasificación cliente VIP
- **Archivos Parquet generados:** 3

---

## Visualizaciones

![Métricas de Negocio](output/visualizaciones_l4.png)
![Segmentación K-Means](output/segmentacion_kmeans.png)
