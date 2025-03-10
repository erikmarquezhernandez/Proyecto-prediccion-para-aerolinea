# Proyecto-prediccion-para-aerolinea

**Situación:**  
La aerolínea enfrentaba el desafío de mejorar su capacidad para pronosticar el promedio mensual de pasajeros, con el fin de optimizar la asignación de recursos, ajustar estrategias de precios y planificar campañas de marketing de manera más precisa.

**Tarea:**  
Se me encargó desarrollar un modelo predictivo que redujera significativamente el error de pronóstico (medido por el $RMSE$), proporcionando herramientas analíticas robustas para apoyar la toma de decisiones operativas y estratégicas.

**Acción:**  
- Realicé un análisis exploratorio de datos (EDA) para asegurar la calidad de la información, detectar valores atípicos y comprender la distribución de la serie.  
- Descompuse la serie temporal en sus componentes de tendencia, estacionalidad y residuo, lo que permitió identificar la naturaleza multiplicativa de la serie a través del análisis de heterocedasticidad.  
- Apliqué la transformación Box-Cox ($\lambda = 0.1480$) para estabilizar la varianza y corregir la heterocedasticidad, facilitando la modelación.  
- Implementé el modelo Prophet y, en paralelo, utilicé un modelo ARIMA optimizado, aplicando validación cruzada y GridSearch para ajustar los hiperparámetros y mejorar la precisión de los pronósticos.  
- Comparé los resultados obtenidos en la escala transformada y tras invertir la transformación, evaluando el desempeño a partir de la reducción del $RMSE$.

**Resultado:**  
La integración de la transformación Box-Cox y la aplicación de modelos avanzados condujeron a una reducción del $RMSE$ en un $66\%$ (de $35.52$ a $12.14$). Este significativo avance no solo mejoró la precisión de los pronósticos, sino que también permitió simular escenarios operativos de alta relevancia, facilitando decisiones estratégicas que optimizarían la asignación de recursos y potenciarían las estrategias de precios y marketing en la aerolínea.

# Análisis de Impacto Práctico

El análisis realizado demuestra que el modelo predictivo optimiza el proceso de pronóstico de pasajeros mensuales y tiene un impacto significativo en la toma de decisiones operativas y estratégicas para la aerolínea.

Mediante la simulación de escenarios, se observa cómo varía la demanda de pasajeros a lo largo del año. Por ejemplo, en meses de alta demanda, el modelo indica la necesidad de aumentar la frecuencia de vuelos para maximizar la ocupación de la flota, mientras que en periodos de menor demanda se pueden ajustar los vuelos para optimizar el uso de recursos y reducir costos operativos.

La mejora en la precisión del modelo es notable, con una reducción del RMSE del 66% (de 35.52 a 12.14). Esta significativa disminución del error permite una asignación más eficiente de recursos, ya que la aerolínea puede planificar de manera óptima la distribución de aeronaves y tripulaciones, evitando vuelos con baja ocupación y maximizando la rentabilidad operativa.

Además, un pronóstico más preciso abre la posibilidad de implementar estrategias de precios dinámicos. Esto permite ajustar las tarifas de forma competitiva durante periodos de baja demanda y maximizar ingresos en picos de alta ocupación. Los datos generados por el modelo pueden también servir para diseñar campañas de marketing dirigidas a segmentos específicos de clientes, mejorando la captación y fidelización de pasajeros.

Finalmente, la evaluación del impacto económico respalda la utilidad del modelo, ya que la mejora en la precisión predictiva se traduce en una mayor eficiencia operativa y un potencial ahorro en costos, justificando la inversión en la optimización y desarrollo continuo del sistema de pronósticos.

**En conclusión**, este análisis de impacto práctico evidencia que el modelo predictivo es una herramienta clave para la toma de decisiones estratégicas, abarcando desde la optimización de recursos y asignación de capacidad hasta la implementación de estrategias de precios y marketing, lo que impulsa la eficiencia operativa y económica de la aerolínea.
