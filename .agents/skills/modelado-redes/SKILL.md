---
name: modelado-redes
description: Utiliza esta habilidad para generar grafos Erdos-Renyi y calcular métricas topológicas complejas.
---
# Instrucciones
Cuando se te pida analizar o generar redes, sigue este protocolo:
1. Usa `networkx` para la generación de grafos.
2. Para el Problema 1, itera p 100 veces entre 0 y 1 para n=100.
3. Asegúrate de extraer siempre:
   - Número de componentes conexas y tamaño de la mayor.
   - Camino mínimo promedio.
   - Densidad y coeficiente de clustering promedio.
4. Para redes reales, debes calcular rigurosamente: grado medio, camino mínimo medio, desviación estándar del grado y densidad.