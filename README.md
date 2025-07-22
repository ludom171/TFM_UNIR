# TFM_UNIR

## Autores
- **Luis Ramiro Domínguez Leiton**  
- **Daniela Alejandra Tupiza Peralta**  

## Titulo
Evaluación Comparativa de Técnicas de Inteligencia Artificial para la Predicción del Número de Estudiantes y la Asignación Docente en Educación Superior.

## Estructura del repositorio

'''
TFM_UNIR/
├── 00_INICIO/
│   ├── data.csv
│   ├── data_limpia.csv
│   └── data_analisis.ipynb        # Análisis exploratorio y limpieza de datos
├── 01_ESTUDIANTES/
│   ├── datos_predic_estudiantes.csv
│   ├── escalador_estus.pkl
│   ├── m_f_estudiantes.pkl
│   └── predictor_estudiantes.ipynb  # Entrenamiento y evaluación de modelos de regresión
└── 02_CURSOS/
    ├── 01_CLASIFICACION/
    │   ├── datos_cursos.csv
    │   ├── etiquetas_profesores.csv
    │   └── clasificacion_docentes.ipynb  # Modelos supervisados de clasificación
    ├── 02_CLUSTERING/
    │   └── clusterizacion.ipynb         # Algoritmos de agrupamiento para segmentación
    └── 03_A_GENETICO/
        ├── asignacion_cursos (1).csv
        ├── datos_docentes.csv
        ├── datos_facultades.csv
        └── genetico.ipynb               # Implementación de algoritmo genético
'''

## Descripción

- **00_INICIO: incluye los archivos originales utilizados para el análisis exploratorio y preparación del dataset general. Contiene los archivos data.csv, data_limpia.csv y el notebook data_analisis.ipynb con el código fuente utilizado para la limpieza y visualización de los datos institucionales.**
- **01_ESTUDIANTES: dedicada a la fase de predicción del número de estudiantes por curso. Contiene el conjunto de datos procesados (datos_predic_estudiantes.csv), los objetos de entrenamiento (escalador_estus.pkl, m_f_estudiantes.pkl) y el notebook predictor_estudiantes.ipynb que documenta el proceso de entrenamiento, validación y evaluación de modelos de regresión.**
- **02_CURSOS: enfocada en la fase de asignación docente. Se subdivide en tres secciones:**
  - **01_CLASIFICACION: contiene los archivos datos_cursos.csv, etiquetas_profesores.csv y el script clasificacion_docentes.ipynb, utilizado para entrenar y evaluar modelos supervisados de clasificación.**
  - **02_CLUSTERING: contiene el notebook clusterizacion.ipynb, que documenta la implementación y evaluación de algoritmos de agrupamiento para la segmentación de cursos.**
  - **03_A_GENETICO: incluye los archivos asignacion_cursos (1).csv, datos_docentes.csv, datos_facultades.csv y el notebook genetico.ipynb, donde se implementa el algoritmo genético para la asignación optimizada de cursos a docentes bajo restricciones operativas.**

