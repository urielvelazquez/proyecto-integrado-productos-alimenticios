### ¿Cómo afecta el diseño a tus decisiones? Un viaje de datos por la aplicación de una Food Startup

#### Objetivo del proyecto
Analizar el comportamiento del usuario dentro de la aplicación de una empresa emergente del sector alimenticio, con el fin de:

- Identificar cuellos de botella en el embudo de ventas y optimizar la conversión en cada etapa.

- Evaluar el impacto del rediseño tipográfico mediante un test A/A/B y detectar posibles efectos adversos.

- Ofrecer recomendaciones basadas en datos para mejorar la experiencia del usuario y aumentar las conversiones.

#### Lenguaje de programación, librerías y habilidades 
![Python](https://img.shields.io/badge/PYTHON-%232A5D9F.svg?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/PANDAS-%232A5D9F.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NUMPY-%232A5D9F.svg?style=for-the-badge&logo=numpy&logoColor=white)
![SciPy](https://img.shields.io/badge/SCIPY-%232A5D9F.svg?style=for-the-badge&logo=scipy&logoColor=white)
![re](https://img.shields.io/badge/RE-%232A5D9F.svg?style=for-the-badge&logoColor=white)
![datetime](https://img.shields.io/badge/DATETIME-%232A5D9F.svg?style=for-the-badge&logoColor=white)
![math](https://img.shields.io/badge/MATH-%232A5D9F.svg?style=for-the-badge&logoColor=white)
![Matplotlib](https://img.shields.io/badge/MATPLOTLIB-%232A5D9F.svg?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/SEABORN-%232A5D9F.svg?style=for-the-badge&logo=seaborn&logoColor=white)
![Limpieza de Datos](https://img.shields.io/badge/LIMPIEZA%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis de Datos](https://img.shields.io/badge/ANÁLISIS%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis Estadístico](https://img.shields.io/badge/ANÁLISIS%20ESTADÍSTICO-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis de Negocio](https://img.shields.io/badge/ANÁLISIS%20DE%20NEGOCIO-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Análisis de pruebas A/A/B](https://img.shields.io/badge/ANÁLISIS%20DE%20PRUEBAS%20A/A/B-%233B7DD8.svg?style=for-the-badge&logoColor=white)
![Visualización de Datos](https://img.shields.io/badge/VISUALIZACIÓN%20DE%20DATOS-%233B7DD8.svg?style=for-the-badge&logoColor=white)

#### Preguntas clave
- ¿Qué eventos del embudo de ventas tienen mayores tasas de abandono?

- ¿El cambio en el diseño de las fuentes afecta significativamente la conversión?

- ¿Hay diferencias estadísticas entre los grupos de control y el grupo de prueba?

#### Metodología
- **Preprocesamiento de datos:** Se ajustaron los nombres de columnas, se eliminaron duplicados y se filtraron registros incompletos o inconsistentes.

- **Análisis del embudo de ventas:** Se identificaron eventos clave y se calcularon las tasas de conversión entre etapas para detectar puntos críticos de abandono.

- **Evaluación del experimento A/A/B:** Se analizaron métricas de conversión y comportamiento entre los dos grupos de control y el grupo de prueba, aplicando pruebas de hipótesis estadísticas para evaluar el impacto del cambio de fuentes.

#### Conclusiones generales
- En todas las comparaciones realizadas entre el grupo con fuentes alteradas (248) y los grupos de control (246 y 247) para cada uno de los eventos, no se pudo rechazar la hipótesis nula. Esto significa que no hay diferencias estadísticamente significativas en las proporciones de usuarios que realizaron estos eventos.

- La consistencia observada sugiere que los grupos de control y el grupo con fuentes alteradas se comportan de manera similar en términos de participación en estos eventos específicos.

- La ausencia de diferencias significativas también valida el diseño experimental, lo que implica que cualquier cambio observado en futuros análisis podrá ser atribuido con mayor certeza a las intervenciones experimentales y no a la división original de los grupos.

- Dado que los resultados muestran que las proporciones de eventos son consistentes entre los grupos, se puede concluir que el experimento fue diseñado y ejecutado correctamente, proporcionando resultados fiables para futuras pruebas y análisis.

Basado en un análisis más conservador (α=0.01), los grupos no muestran diferencias significativas en todos los eventos. Esto sugiere que las fuentes alteradas no tienen un efecto significativo sobre la participación del usuario.

#### Diccionario de datos

La tabla `logs_exp` (cada entrada de registro es una acción de usuario o un evento):

- `EventName:` nombre del evento.

- `DeviceIDHash:` identificador de usuario unívoco.

- `EventTimestamp:` hora del evento.

- `ExpId:` número de experimento. 246 y 247 son los grupos de control, y 248 es el grupo de prueba.
