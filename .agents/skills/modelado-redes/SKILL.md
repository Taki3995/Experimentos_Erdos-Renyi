---
name: modelado-redes
description: Utiliza esta habilidad para generar grafos Erdos-Renyi y calcular métricas topológicas complejas.
---
# Instrucciones
Cuando se te pida analizar o generar redes, sigue este protocolo:
1. Usa `networkx` para la generación de grafos.
2. Para el **Problema 1 (Modelado ER)**, el objetivo es graficar la transición de conectividad. Para $N=100$:
   - Selecciona valores de $p$ que capturen los 4 regímenes:
     - **Subcrítico**: $p < 1/(N-1)$ (ej. $p=0.005$).
     - **Crítico**: $p = 1/(N-1)$ (ej. $p=0.010$).
     - **Supercrítico**: $1/(N-1) < p < \ln(N)/(N-1)$ (ej. $p=0.03$).
     - **Conectado**: $p > \ln(N)/(N-1)$ (al menos $p=0.06$).
   - Itera al menos 100 veces para cada $p$ para obtener promedios robustos.
3. Métricas obligatorias por cada $p$:
   - Número de componentes conexas y **tamaño relativo de la mayor componente ($G/N$)**.
   - Camino mínimo promedio (solo en la componente gigante si la red no es conexa).
   - Densidad y Coeficiente de Clustering.
4. Para el **Modelo BA**, considera siempre el parámetro de conexión preferencial y verifica la ley de potencia $\gamma \approx 3$.