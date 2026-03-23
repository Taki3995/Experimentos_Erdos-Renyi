---
name: extractor-datasets
description: Habilidad para automatizar la descarga y procesamiento de redes desde Network Repository.
---
# Instrucciones
1. Selecciona redes de 3 dominios distintos (ej: biológicas, sociales, económicas) excluyendo "Generated Graphs".
2. Escribe funciones en Python usando `requests` o `urllib` para descargar los archivos.
3. Procesa los archivos descargados (.edges, .mtx) limpiando los datos y cargándolos en un objeto Grafo de `networkx`.
4. **Análisis Topológico Crítico**: Por cada red real, realiza:
   - Análisis de distribución de grado (gráficos log-log) para verificar la naturaleza Libre de Escala.
   - Cálculo del exponente $\gamma$ si se ajusta a una ley de potencia.
   - Comparación del clustering y camino mínimo promedio con una red ER equivalente ($N$ y $k$ iguales) para resaltar la ineficiencia de los modelos aleatorios en redes reales.
   - Identificación de posibles hubs y análisis de su impacto en la robustez de la red.