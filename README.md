# TFM_UNIR

## Autores
- **Luis Ramiro Dominguez Leiton**  
- **Daniela Alejandra Tupiza Peralta**  

## Titulo
Evaluación Comparativa de Técnicas de Inteligencia Artificial para la Predicción del Número de Estudiantes y la Asignación Docente en Educación Superior.

## Resumen 
El presente trabajo busca mejorar la eficiencia y equidad en la asignación de cursos a docentes en una institución de educación superior, cuyos datos históricos institucionales incluyen información sobre el número de estudiantes, horarios, asignaturas y disponibilidad docente. A partir de estos datos, se realizó una evaluación comparativa de técnicas de inteligencia artificial aplicadas a dos subproblemas clave: Fase 1, la predicción del número de estudiantes por curso, y Fase 2, la asignación docente al inicio de cada semestre.

En la Fase 1, se abordó el problema como una tarea de regresión mediante aprendizaje supervisado, comparando modelos como Regresión Lineal, K-Nearest Neighbors (KNN), Random Forest, Gradient Boosting, Support Vector Regressor (SVR) y Red Neuronal Multicapa (MLP) para predecir el número de estudiantes por curso . El modelo Random Forest Regressor obtuvo el mejor rendimiento (MAE: 9.71), siendo la predicción más adecuada para anticipar la demanda académica y guiar la asignación docente.

En la Fase 2, se abordó el problema desde un enfoque mixto que integró técnicas de clasificación supervisada, agrupamiento no supervisado y un algoritmo genético con restricciones para realizar la asignación docente. Se evaluaron modelos de clasificación como Regresión Logística, K-Nearest Neighbors (KNN), Support Vector Classifier (SVC), Random Forest, Decision Tree y Gradient Boosting, que permitieron identificar características de los datos para clasificarlos acrorde a sus etiquetas. Asimismo, se aplicaron métodos de clustering como K-Means, DBSCAN, Agglomerative Clustering y Spectral Clustering para identificar patrones en los datos y segmentar cursos según sus características. Si bien estos enfoques ofrecieron asignaciones equitativas, se identificaron inconsistencias como solapamientos de horario y conflictos en la distribución de carga. Para superar estas deficiencias, se diseñó un algoritmo genético con restricciones, capaz de generar asignaciones factibles y equilibradas, respetando los horarios laborales y evitando conflictos operativos. Este algoritmo superó a todas las demás técnicas evaluadas, por lo que se seleccionó como la solución final para esta fase, complementando al modelo Random Forest utilizado en la predicción de la Fase 1.


## Estructura del repositorio

```
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
```

## Descripción

- **00_INICIO:** incluye los archivos originales utilizados para el análisis exploratorio y preparación del dataset general. Contiene los archivos data.csv, data_limpia.csv y el notebook data_analisis.ipynb con el código fuente utilizado para la limpieza y visualización de los datos institucionales.
- **01_ESTUDIANTES:** dedicada a la fase de predicción del número de estudiantes por curso. Contiene el conjunto de datos procesados (datos_predic_estudiantes.csv), los objetos de entrenamiento (escalador_estus.pkl, m_f_estudiantes.pkl) y el notebook predictor_estudiantes.ipynb que documenta el proceso de entrenamiento, validación y evaluación de modelos de regresión.
- **02_CURSOS:** enfocada en la fase de asignación docente. Se subdivide en tres secciones:
  - **01_CLASIFICACION:** contiene los archivos datos_cursos.csv, etiquetas_profesores.csv y el script clasificacion_docentes.ipynb, utilizado para entrenar y evaluar modelos supervisados de clasificación.
  - **02_CLUSTERING:** contiene el notebook clusterizacion.ipynb, que documenta la implementación y evaluación de algoritmos de agrupamiento para la segmentación de cursos.
  - **03_A_GENETICO:** incluye los archivos asignacion_cursos (1).csv, datos_docentes.csv, datos_facultades.csv y el notebook genetico.ipynb, donde se implementa el algoritmo genético para la asignación optimizada de cursos a docentes bajo restricciones operativas.

