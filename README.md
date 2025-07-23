# Challenge3-Data-Science-Latam

CHALLENGE
TELECOM X2: Predicción de Cancelación (Churn)
JUAN CARLOS GÓMEZ SALAS
ONE Oracle Next Education de Alura LATAM

El desafío consistió en lo siguiente:
Tu nueva misión es desarrollar modelos predictivos capaces de prever qué clientes tienen mayor probabilidad de cancelar sus servicios.
La empresa quiere anticiparse al problema de la cancelación, y te corresponde a ti construir un pipeline robusto para esta etapa inicial de modelado.

Objetivo general del Desafío
Predecir el churn (cancelación) de clientes en base a variables relevantes.

Objetivos específicos del Desafío
•	Preparar los datos para el modelado (tratamiento, codificación, normalización).
•	Realizar análisis de correlación y selección de variables.
•	Entrenar dos o más modelos de clasificación.
•	Evaluar el rendimiento de los modelos con métricas.
•	Interpretar los resultados, incluyendo la importancia de las variables.
•	Crear una conclusión estratégica señalando los principales factores que influyen en la cancelación.


El proyecto consiste en los siguientes archivos:
•	“Telecom_X2_Notebook_JCGS.ipynb”: notebook en lenguaje Python de Google Colab.
•	“TelecomX_Data_tratado.csv”: planilla CSV con los datos tratados resultantes de la primera parte del desafío.
•	“Telecom_X2_Secciones_JCGS.docx”: documento que detalla las secciones que conforman el notebook, las bibliotecas que se deben instalar y las acciones que se realizan incluyendo los gráficos que se generan. Además se incluyen algunos gráficos relevantes.


A continuación se resumen las secciones que conforman el notebook:
•	Lectura de los datos contenidos en la planilla CSV antes mencionada.
•	Explorando los datos: variables categóricas, variables numéricas y correlaciones.
•	Transformación de los datos: variables explicativas y variable de respuesta, transformando las variables explicativas y transformando la variable de respuesta.
•	Ajustando los modelos: dividiendo los datos (entrenamiento y prueba), modelo de referencia (baseline), árboles de decisión, normalizando los datos, KNN, escogiendo y serializando el mejor modelo, prediciendo variable respuesta para nuevo dato.
•	Variables explicativas más relevantes: selección, modelo árbol con variables explicativas más relevantes, validando y evaluando el modelo, modelo KNN con variables explicativas más relevantes.
•	Validación cruzada, validación cruzada con sensibilidad, estratificando los datos.
•	Oversampling, pipeline para validación, undersampling, probando el modelo.


Interpretación de los resultados, incluyendo la importancia de las variables:
•	Score R²: En Python, el método .score() en un modelo de regresión, devuelve el coeficiente de determinación (R²). Este valor indica la proporción de la varianza en la variable dependiente que es explicada por el modelo de regresión. Un valor de R² cercano a 1 indica un buen ajuste del modelo, mientras que un valor cercano a 0 sugiere que el modelo no explica bien la variabilidad de los datos.
•	Para los tres modelos evaluados, resultó un Score R² igual a: Modelo de Referencia Baseline (0,712), Modelo de Árbol de Decisión (0,772) y Modelo KNN (0,742), por lo que se escoge y serializa el modelo de árbol.
•	Para el modelo de árbol con las cuatro variables más relevantes resulta Score R² de 0,780.


Basado en los antecedentes presentados, se reiteran las recomendaciones entregadas a Telecom X en el primer proyecto para reducir la cantidad de abandonos de contratos:
•	Respecto al perfil de los clientes, generar mayores incentivos para clientes menores de 65 años, que estén en pareja y que tengan dependientes.
•	Respecto a los servicios a contratar, generar mayores incentivos para que los clientes contraten Internet service con Online security y Tech Support.
•	Respecto a tipo de contrato, generar mayores incentivos para que los clientes contraten a uno o dos años, e incluso más o indefinido.
•	Respecto al método de pago, eliminar o desincentivar el uso del Electronic check.

Con este segundo proyecto se dispone de un modelo de regresión (árbol de decisión), que permite predecir las posibilidades que un determinado cliente pueda abandonar el contrato.
