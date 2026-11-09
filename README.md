# Simuladores · Procesamiento de Datos a Gran Escala

Luis Ernesto Bueno Solano · Pontificia Universidad Javeriana · 2026-30

Dos simuladores interactivos hechos en un solo archivo HTML cada uno (HTML, CSS y JavaScript, sin dependencias externas). Basta con abrirlos en el navegador.

## Simulador de clúster Apache Spark

Muestra cómo un clúster de Spark reparte el trabajo entre workers y executors.

- Scheduler FAIR con localidad de datos
- Caché LRU por executor y tasa de aciertos (hit rate)
- Jobs de tres stages separados por shuffles
- Tolerancia a fallos: caída y recuperación de nodos
- Benchmark con 3, 6 y 10 workers para ver por qué escalar no es lineal

## Simulador MLlib · Clasificación

Simula un `LogisticRegression` de Spark MLlib entrenado sobre el clúster.

- Datasets lineal, solapado, círculos y XOR
- Hiperparámetros: `maxIter`, `regParam`, `elasticNetParam`, umbral, `StandardScaler` y `PolynomialExpansion`
- Frontera de decisión en vivo; clic sobre la gráfica para predecir un punto nuevo
- Métricas: matriz de confusión, accuracy, precision, recall, F1 y AUC
- Carga del clúster según workers, núcleos, RAM, particiones y `df.cache()`

## Uso

```bash
git clone https://github.com/Luis-bu/procesamiento_simuladores
```

Luego abre cualquiera de los `.html` en el navegador.
