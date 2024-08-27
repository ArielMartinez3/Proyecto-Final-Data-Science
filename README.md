# README: ProyectoDS_ParteI_Martinez

## Introducción
Este proyecto tiene como objetivo analizar la relación entre el nivel educativo, la ocupación, las horas trabajadas y los ingresos. Se buscará responder a preguntas clave sobre la distribución de ingresos y cómo se ven influenciados por diferentes factores socioeconómicos.

## Abstract
El “Adult” dataset, también conocido como “Census Income” dataset, es una colección de datos del censo que se utiliza para predecir si el ingreso de una persona supera los $50,000 dólares americanos al año. Este dataset contiene 48,842 instancias y 14 características, incluyendo edad, educación, ocupación, y horas trabajadas por semana. El objetivo de este proyecto es explorar y visualizar los datos para identificar patrones y relaciones que puedan ayudar a responder preguntas específicas sobre los factores que influyen en los ingresos de las personas. A través de visualizaciones univariadas, bivariadas y multivariadas, junto con resúmenes numéricos, se buscará proporcionar una comprensión profunda de las variables más influyentes en la determinación de los ingresos.

## Dataset
* **Nombre:** Adult
* **Fuente:** UCI Machine Learning Repository
* **Enlace:** Adult Dataset
* **Descripción:** Conjunto de datos del censo utilizado para predecir el ingreso de una persona.
* **Variables clave:** Edad, sexo, nivel educativo, estado civil, ocupación, horas trabajadas por semana, país de origen, ingreso.

## Objetivos
* Explorar la distribución de los ingresos en función de diferentes variables sociodemográficas.
* Identificar los factores más relevantes que influyen en el ingreso.
* Construir modelos de clasificación para predecir si una persona tiene un ingreso superior a $50,000.

## Preguntas de Investigación
* **Pregunta 1:** ¿Cuál es la relación entre el nivel educativo y el ingreso?
* **Pregunta 2:** ¿Cómo influye la ocupación en el ingreso?
* **Pregunta 3:** ¿Existe una diferencia significativa en los ingresos entre hombres y mujeres?

## Metodología
1. **Carga de datos:** Cargar el dataset utilizando pandas.
2. **Exploración de datos:**
   * **Análisis univariado:** Histograma de edad, recuento de valores únicos para variables categóricas.
   * **Análisis bivariado:** Gráficos de dispersión para horas trabajadas vs. ingreso, boxplots para comparar ingresos por nivel educativo.
   * **Análisis multivariado:** Pairplots para visualizar relaciones entre múltiples variables.
3. **Limpieza de datos:**
   * Manejar valores faltantes (imputación o eliminación).
   * Codificar variables categóricas.
4. **Modelado:**
   * Selección de características relevantes.
   * Construcción de modelos de clasificación (regresión logística, árboles de decisión, etc.).
   * Evaluación del rendimiento de los modelos.
5. **Visualización de datos:**
   * Realizar 3 gráficos diferentes con Matplotlib.
   * Realizar 3 gráficos diferentes con Seaborn.
   * Usar al menos un parámetro adicional (grid, hue, etc.) para enriquecer la legibilidad de los gráficos.
   * Interpretar cada gráfico para obtener insights relevantes que permitan dar respuesta a las preguntas de investigación.

## Herramientas
* **Lenguaje de programación:** Python
* **Librerías:** pandas, NumPy, matplotlib, seaborn

## Resultados Esperados
* Identificar los factores más importantes que influyen en el ingreso.
* Construir un modelo de clasificación preciso para predecir el ingreso.
* Visualizaciones claras y concisas que respalden los hallazgos.

## Resultados obtenidos 

### Diferencias en Ingresos entre Géneros
- **Ingresos:** Los hombres tienen una mayor probabilidad de tener ingresos superiores a 50K en comparación con las mujeres.
- **Variabilidad:** La variabilidad en los ingresos es mayor entre los hombres.
- **Horas Trabajadas:** Los hombres trabajan en promedio 42.43 horas por semana, mientras que las mujeres trabajan 36.41 horas por semana.
- **Conclusión:** La diferencia en las horas trabajadas puede contribuir a las diferencias de ingresos observadas entre géneros.

### Datos Demográficos Generales
- **Edad Promedio:** La edad promedio en el dataset es de casi 39 años.
- **Educación Promedio:** La educación promedio se acerca al nivel secundario completo, con 10.08 años de educación.
- **Horas Trabajadas:** La mayoría de las personas trabajan alrededor de 40 horas por semana.
- **Ingresos:** Una proporción significativa de la población tiene ingresos inferiores a 50K.

### Relación entre Nivel Educativo e Ingresos
- **Educación y Ingresos:** Hay una relación positiva entre el nivel educativo y la probabilidad de obtener ingresos superiores a 50K. A medida que aumentan los años de educación, también aumenta la probabilidad de tener ingresos más altos.
- **Nivel Educativo Promedio:** 10.08 años.
- **Porcentaje con Ingresos > 50K:** 24% de la población.

### Influencia de la Ocupación en los Ingresos
- **Ocupaciones con Altos Ingresos:** "Exec-managerial" y "Prof-specialty" están asociadas con un mayor porcentaje de personas con ingresos superiores a 50K.
- **Ocupaciones con Bajos Ingresos:** "Other-service" y "Priv-house-serv" tienen una proporción significativamente menor de personas con ingresos superiores a 50K.
- **Conclusión:** Los roles en gestión y especialización profesional muestran mayores probabilidades de ingresos altos.

### Distribución de Ocupaciones
- **Ocupación Más Común:** La mayoría de los trabajadores están empleados en ocupaciones profesionales, con "Prof-specialty" siendo la ocupación más común.
- **Ocupaciones Menos Comunes:** Las ocupaciones menos comunes incluyen trabajos en las fuerzas armadas y servicios domésticos.




