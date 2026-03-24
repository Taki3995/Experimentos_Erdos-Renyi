---
name: extractor-datasets
description: Habilidad para automatizar la descarga y procesamiento de redes desde Network Repository.
---
# Instrucciones
1. Selecciona redes de 3 dominios distintos (ej: biológicas, sociales, económicas) excluyendo "Generated Graphs".
2. Escribe funciones en Python usando `requests` o `urllib` para descargar los archivos.
3. Procesa los archivos descargados (.edges, .mtx) limpiando los datos y cargándolos en un objeto Grafo de `networkx` listo para analizar distribuciones de grado.