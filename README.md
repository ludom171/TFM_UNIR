# TFM_UNIR

# Autores
Luis Ramiro Dominguez Leiton
Daniela Alejandra Tupiza Peralta

# Resumen

•	00_INICIO: incluye los archivos originales utilizados para el análisis exploratorio y preparación del dataset general. Contiene los archivos data.csv, data_limpia.csv y el notebook data_analisis.ipynb con el código fuente utilizado para la limpieza y visualización de los datos institucionales.
•	01_ESTUDIANTES: dedicada a la fase de predicción del número de estudiantes por curso. Contiene el conjunto de datos procesados (datos_predic_estudiantes.csv), los objetos de entrenamiento (escalador_estus.pkl, m_f_estudiantes.pkl) y el notebook predictor_estudiantes.ipynb que documenta el proceso de entrenamiento, validación y evaluación de modelos de regresión.
•	02_CURSOS: enfocada en la fase de asignación docente. Se subdivide en tres secciones:
o	01_CLASIFICACION: contiene los archivos datos_cursos.csv, etiquetas_profesores.csv y el script clasificacion_docentes.ipynb, utilizado para entrenar y evaluar modelos supervisados de clasificación.
o	02_CLUSTERING: contiene el notebook clusterizacion.ipynb, que documenta la implementación y evaluación de algoritmos de agrupamiento para la segmentación de cursos.
o	03_A_GENETICO: incluye los archivos asignacion_cursos (1).csv, datos_docentes.csv, datos_facultades.csv y el notebook genetico.ipynb, donde se implementa el algoritmo genético para la asignación optimizada de cursos a docentes bajo restricciones operativas.

