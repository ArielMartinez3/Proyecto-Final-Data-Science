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

## Conclusiones Gráficos

### Histograma del Nivel Educativo
- La mayoría de las personas tienen entre 9 y 12 años de educación, con el punto más alto en 10 años, que corresponde a la finalización de la secundaria (high school).
- En promedio, las personas en el dataset tienen poco más de 10 años de educación.
- La visualización muestra que la mayoría de los individuos han completado la secundaria, con una mayor representación de niveles educativos superiores que los de menor educación.

### Gráfico de Barras de Ingresos por Ocupación
- Las ocupaciones como "Ejecutivo" y "Profesional" tienen más personas con ingresos altos.
- Ocupaciones como "Limpiador" y "Servicios domésticos" tienen menos personas con ingresos altos.
- Algunas ocupaciones tienen una mezcla de ingresos altos y bajos, como "Ventas" y "Reparación".
- El gráfico muestra que las ocupaciones pueden influir en el nivel de ingresos, con algunos trabajos claramente asociados con mejores salarios que otros.

### Scatterplot: Años de Educación vs Capital Ganado
- No hay una tendencia clara en cómo el capital ganado cambia con más años de educación. La relación parece débil, como lo indica la baja correlación de 0.12. La mayoría de los puntos están cerca del eje horizontal, indicando que el capital ganado es bajo para muchos con distintos niveles educativos.
- Aunque el capital ganado a partir de los 9 años de educación es levemente superior al de los grupos de menor educación, lo que puede sugerir cierta influencia, la distribución de ingresos sigue siendo muy variada.
- No parece haber una relación fuerte entre los años de educación y el capital ganado en el dataset.

### Boxplot: Horas Trabajadas por Semana según el Sexo
- Los hombres tienden a trabajar más horas a la semana en comparación con las mujeres, con una media de 42.4 horas frente a 36.4 horas.
- El rango de horas trabajadas es más amplio para los hombres, con una mayor variabilidad.
- Las medianas (líneas dentro de las cajas) son iguales para ambos sexos (40 horas), pero las mujeres tienen una distribución más concentrada en torno a esta mediana.

### Pairplot de Variables Seleccionadas
Este gráfico muestra cómo se relacionan entre sí cuatro variables importantes: edad, años de educación, horas trabajadas por semana e ingresos.
- **Observaciones:**
  - **Edad y Educación:** No parece haber una relación clara entre la edad y los años de educación.
  - **Edad y Horas Trabajadas:** Los ingresos más altos tienden a estar asociados con un mayor número de horas trabajadas.
  - **Educación y Horas Trabajadas:** Las personas con más educación tienden a trabajar más horas.
  - **Ingreso:** Las personas con ingresos más altos tienden a tener más educación y trabajar más horas.

### Gráfico de Dispersión Multivariado
- Las personas con más edad tienden a trabajar menos horas por semana. Esto puede ser porque los trabajos suelen ser menos demandantes para los trabajadores mayores.
- Los puntos más grandes, que indican un mayor nivel educativo, están más relacionados con el aumento en las horas trabajadas y los ingresos más altos.
- Los puntos en colores más cálidos (indicando ingresos más altos) tienden a tener más educación y a trabajar más horas por semana.
- El gráfico muestra que los trabajadores más educados y con mayores ingresos tienden a trabajar más horas y tienen un rango de edad más variado. Además, los trabajadores mayores suelen trabajar menos horas.

### Distribución de Ocupaciones
- Las ocupaciones más frecuentes son "Prof-specialty" (profesionales especializados), "Craft-repair" (trabajos de reparación y mantenimiento), y "Exec-managerial" (gestión ejecutiva).
- Las ocupaciones menos comunes incluyen "Armed-Forces" (fuerzas armadas) y "Priv-house-serv" (servicios domésticos privados).

### Distribución de Ingresos por Género
- Hay una notable mayor proporción de hombres con ingresos superiores a 50K en comparación con las mujeres.
- La proporción de ingresos inferiores a 50K se distribuye de una manera mucho más similar en ambos géneros.

## Distribución de Ocupaciones por Género

1. **Ocupaciones con Alta Proporción de Hombres:**
   - Ocupaciones como "Exec-managerial", "Craft-repair", y "Transport-moving" tienen una representación significativamente mayor de hombres.
   - Estas ocupaciones suelen estar asociadas con mayores ingresos. Por ejemplo, "Exec-managerial" tiene una alta probabilidad de ingresos superiores a 50K, lo que coincide con la alta representación masculina.

2. **Ocupaciones con Alta Proporción de Mujeres:**
   - Ocupaciones como "Other-service" y "Priv-house-serv" tienen una mayor cantidad de mujeres.
   - Estas ocupaciones tienden a tener una menor proporción de ingresos superiores a 50K. La ocupación "Other-service", en particular, tiene una alta representación femenina y una baja proporción de ingresos altos.

3. **Ocupaciones con Baja Representación Femenina:**
   - "Craft-repair" y "Protective-serv" tienen muy pocas mujeres en comparación con los hombres.
   - Estas ocupaciones también están asociadas con una variedad de niveles de ingresos, pero "Craft-repair" en particular tiende a tener una mayor proporción de ingresos altos.

## Distribución de Ingresos según Años de Educación

- A más años de educación, mayor porcentaje de personas con ingresos >50K. Por ejemplo, el 74% de quienes tienen 16 años de educación ganan más de 50K, frente al 0% con solo 1 año.
- Los porcentajes de ingresos altos aumentan notablemente a partir de 9 años de educación, alcanzando niveles críticos en educación universitaria.
- Los niveles educativos avanzados (13 años o más) muestran los mayores porcentajes de ingresos >50K, destacando la educación universitaria como clave para mayores ingresos.
- Para niveles educativos bajos (hasta 7 años), la mayoría tiene ingresos menores a 50K, indicando que una educación mínima limita las oportunidades de altos ingresos.

## Resultados obtenidos 

### Diferencias en Ingresos entre Géneros
- Los hombres tienen una mayor probabilidad de tener ingresos superiores a 50K en comparación con las mujeres.
- Los hombres trabajan en promedio 42.43 horas por semana, mientras que las mujeres trabajan 36.41 horas por semana.
- El análisis muestra que hay una correlación entre la representación de género en diferentes ocupaciones y la diferencia salarial. Las ocupaciones dominadas por hombres tienden a ofrecer mayores ingresos, mientras que las ocupaciones dominadas por mujeres suelen ofrecer salarios más bajos. 
- Esta diferencia en la distribución de género en ocupaciones específicas contribuye a la brecha salarial observada entre hombres y mujeres en el dataset.

**Conclusión:** La diferencia en las horas trabajadas puede contribuir a las diferencias de ingresos observadas entre géneros, y también hay una correlación con la representación de ambos géneros en ciertas ocupaciones.

### Relación entre ocupación e ingreso
- Algunas ocupaciones, como "Exec-managerial" y "Prof-specialty", pueden mostrar una alta proporción de personas con ingresos mayores a 50K. Estas ocupaciones suelen estar asociadas con altos niveles de responsabilidad y especialización, lo que puede justificar los altos ingresos.
- Ocupaciones como "Adm-clerical" y "Other-service" pueden tener una baja proporción de personas con ingresos superiores a 50K. Estas ocupaciones a menudo están asociadas con roles de apoyo o servicios, que típicamente tienen menores salarios comparados con roles de gestión o profesionales especializados.
- La distribución de ingresos según ocupación puede resaltar disparidades salariales entre diferentes tipos de trabajos. Por los resultados obtenidos anteriormente, es probable que las ocupaciones que requieren más educación y experiencia estén mejor remuneradas en comparación con trabajos que no requieren tales calificaciones.
- El análisis y visualización ayudan a identificar patrones en cómo diferentes ocupaciones están relacionadas con el nivel de ingresos, proporcionando una visión clara sobre la disparidad salarial en el dataset.

### Relación entre Nivel Educativo e Ingresos
- Hay una estrecha relación entre el nivel educativo y la probabilidad de obtener ingresos superiores a 50K. A medida que aumentan los años de educación, también aumenta la probabilidad de tener ingresos más altos.
- Los niveles educativos avanzados (13 años o más) muestran los mayores porcentajes de ingresos >50K, destacando la educación universitaria como clave para mayores ingresos.
- Porcentaje de personas con ingresos mayores a 50K y más de 12 años de educación: 52.58%
- Porcentaje de personas con ingresos mayores a 50K que tienen más de 12 años de educación: 76.15%
- Porcentaje con Ingresos mayores a 50K: 24% de la población.






