# Ciencia de Datos aplicada a la gestión de incidentes de soporte TI

## Presentación del proyecto

Este proyecto hace parte de mi proceso de formación en Ciencia de Datos en la Universidad EAN y nace del interés por comprender cómo podemos aprovechar la información que se genera diariamente en las mesas de servicio de tecnología para mejorar la atención de los incidentes.

Más allá de realizar cálculos estadísticos o generar gráficos, mi propósito es identificar situaciones que afectan la calidad del servicio y explorar cómo los datos pueden ayudar a tomar mejores decisiones, anticipar dificultades y establecer prioridades de atención.

## Objetivo del proyecto

Analizar el comportamiento de los incidentes de soporte TI, identificar los factores asociados a sus tiempos de resolución y evaluar la posibilidad de utilizar modelos predictivos como herramienta de apoyo a la gestión del servicio.

## Desarrollo del proyecto

El trabajo fue desarrollado de manera individual y se organizó en las siguientes etapas:

1. Exploración, limpieza y preparación de los datos.
2. Análisis estadístico y visualización de la información.
3. Construcción y evaluación de un modelo predictivo.
4. Diseño de un tablero ejecutivo y propuesta de alertas preventivas.

## Principales resultados

La base de datos original contiene 141.712 registros, correspondientes a 24.918 incidentes únicos. Después del proceso de limpieza y consolidación, se obtuvieron 23.362 incidentes válidos y 17 variables para el análisis.

| Indicador | Resultado |
| --- | ---: |
| Incidentes analizados | 23.362 |
| Tiempo promedio de resolución | 178,17 horas |
| Mediana de resolución | 22,10 horas |
| Incidentes resueltos en máximo 24 horas | 51,67 % |
| Cumplimiento del SLA registrado | 61,78 % |
| Incidentes que superan los 7 días | 22,94 % |
| Cumplimiento del SLA en incidentes críticos | 1,85 % |

Uno de los resultados que más llamó mi atención fue que los incidentes críticos presentan una mediana de resolución considerablemente superior a la de los incidentes de baja prioridad. Esta situación plantea la necesidad de revisar los mecanismos de priorización, asignación y seguimiento de los casos.

## Modelo predictivo

Se desarrolló un modelo de regresión lineal utilizando variables relacionadas con la caracterización de los incidentes y se comparó su desempeño con un modelo base basado en la mediana histórica.

Los resultados mostraron que la regresión lineal no logró mejorar el error absoluto medio del modelo base, aunque presentó una ligera reducción del RMSE. Esto evidencia las limitaciones de la información utilizada y la necesidad de explorar otras variables y métodos de predicción.

Considero que reconocer estas limitaciones también hace parte del aprendizaje, ya que un modelo predictivo no necesariamente representa una mejora por el solo hecho de ser más elaborado.

## Propuesta de aplicación práctica

Como complemento al análisis, se diseñó un tablero ejecutivo con indicadores de gestión y una simulación retrospectiva de alertas mediante un sistema de semáforos.

- Verde: seguimiento habitual del incidente.
- Amarillo: caso que requiere atención y seguimiento preventivo.
- Rojo: caso que requiere revisión prioritaria.

La propuesta busca facilitar el seguimiento de los incidentes y apoyar la toma de decisiones de los responsables de las mesas de servicio. La simulación utiliza información histórica y no constituye un sistema predictivo validado en tiempo real.

## Herramientas utilizadas

- Python.
- Google Colab.
- Pandas y NumPy.
- Matplotlib y Seaborn.
- Scikit-learn.
- GitHub.

## Cuaderno del proyecto

[Consultar el cuaderno de Ciencia de Datos](Proyecto_Ciencia_de_Datos_Soporte.ipynb)

## Reflexión final

El desarrollo de este proyecto me permitió comprender que los datos de una mesa de servicio pueden aportar mucho más que un simple registro de incidentes. Su análisis permite reconocer dificultades operativas, identificar oportunidades de mejora y orientar decisiones que contribuyan a ofrecer un mejor servicio tecnológico.

El principal aprendizaje es que la tecnología y el análisis de datos deben estar al servicio de las necesidades reales de las personas y de las organizaciones.

---



## Origen de los datos

Para el desarrollo de este proyecto utilicé el conjunto de datos Incident Management Process Enriched Event Log, publicado por Amaral, Fantinato y Peres (2018) en el repositorio de aprendizaje automático de la Universidad de California, Irvine (UCI).

La base de datos contiene información anonimizada de incidentes registrados en la plataforma ServiceNow de una empresa de tecnología.

Llegué a esta fuente con el apoyo de ChatGPT, herramienta que me orientó en la búsqueda y selección de un conjunto de datos relacionado con la gestión de servicios TI.

Los datos fueron consolidados, depurados y transformados de acuerdo con los objetivos de este proyecto.

Fuente original: https://doi.org/10.24432/C57S4H

Licencia: Creative Commons Attribution 4.0 International (CC BY 4.0).

## Fundamentación metodológica

El análisis exploratorio y la identificación de valores atípicos se relacionan con los métodos de análisis de datos planteados por Tukey (1977).

Para complementar la comprensión de la regresión lineal y la evaluación del modelo predictivo, se propone como referencia el trabajo de James et al. (2023), especialmente por su aplicación práctica mediante Python.

## Uso de inteligencia artificial

Durante el desarrollo de este proyecto utilicé ChatGPT, de OpenAI, como herramienta de apoyo académico.

Su acompañamiento me permitió identificar una fuente de datos adecuada, estructurar las etapas del proyecto, construir y revisar el código en Python, interpretar los resultados y organizar la documentación.

El trabajo fue desarrollado de manera individual, mediante un proceso de ejecución, revisión y ajuste de los resultados obtenidos en Google Colab.

Mi interés fue comprender el propósito de cada etapa y relacionar los resultados con situaciones propias de la gestión de servicios tecnológicos.

## Referencias bibliográficas

- Amaral, C., Fantinato, M., & Peres, S. (2018). *Incident management process enriched event log* [Conjunto de datos]. UCI Machine Learning Repository. https://doi.org/10.24432/C57S4H

- Tukey, J. W. (1977). *Exploratory data analysis*. Addison-Wesley.

- James, G., Witten, D., Hastie, T., Tibshirani, R., & Taylor, J. (2023). *An introduction to statistical learning: With applications in Python*. Springer. https://doi.org/10.1007/978-3-031-38747-0

- OpenAI. (2026). *ChatGPT* [Modelo de lenguaje de inteligencia artificial]. https://chatgpt.com/

Universidad EAN | Ciencia de Datos

Proyecto académico desarrollado de manera individual.
