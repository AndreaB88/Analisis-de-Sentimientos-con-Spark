# Analisis-de-Sentimientos-con-Spark

## Introducción

El objetivo de este proyecto es realizar un análisis de sentimientos sobre los comentarios de los pasajeros de una aerolínea utilizando técnicas de Procesamiento de Lenguaje Natural (NLP) en un entorno Big Data con Apache Spark y Python (PySpark). El análisis busca identificar opiniones positivas, negativas y neutrales en los comentarios y correlacionar estos sentimientos con otras variables disponibles en el dataset, como la valoración general, el tipo de viajero y la clase de servicio.

## Relevancia del Proyecto

El análisis de sentimientos es una herramienta poderosa para las aerolíneas, ya que les permite obtener una comprensión profunda de las opiniones y experiencias de sus clientes. Al correlacionar estos sentimientos con diferentes aspectos del servicio, la aerolínea puede identificar áreas de mejora y tomar decisiones informadas para mejorar la satisfacción del cliente y, en última instancia, su lealtad.

## Estructura de los Datos

El conjunto de datos, descargado de Kaggle, contiene opiniones y calificaciones de los pasajeros sobre los vuelos de Ryanair desde 2012 hasta 2024. Este dataset incluye 21 columnas y 2249 registros, representando una revisión detallada de la experiencia del pasajero.

## Objetivos del Proyecto

### Objetivo Principal

- Realizar un análisis de sentimientos de los comentarios de los pasajeros, clasificándolos en sentimientos positivos, negativos y neutros.

### Objetivos Específicos

- Correlación de sentimientos y valoración global.
- Relación con el tipo de viajero y clase de servicio.
- Identificación de patrones y tendencias.
- Desarrollo y aplicación de modelos de Machine Learning: Random Forest, Logistic Regression, y Naïve Bayes.

## Configuración del Entorno Big Data

Para este proyecto, se configuró un entorno Big Data usando un clúster de Spark dentro de un contenedor Docker, trabajando con Jupyter Notebook y PySpark. Esta configuración permite procesar grandes volúmenes de datos de manera distribuida y asegurar la portabilidad y reproducibilidad del entorno.

## Preparación de Datos

### Cargar el Dataset

El dataset fue descargado de Kaggle y cargado en una sesión de Spark para su análisis.

### Limpieza y Preprocesamiento de Datos

- Eliminación de columnas irrelevantes y manejo de valores nulos.
- Transformación de columnas a tipo numérico y normalización de texto.
- Filtrado de valores anómalos y codificación de variables categóricas.

## Análisis de Sentimientos

Se utilizó el SentimentIntensityAnalyzer de VADER para asignar puntuaciones de sentimiento a cada comentario y clasificarlos en positivos, negativos o neutrales.

## Algoritmos de Aprendizaje Automático

Se implementaron tres modelos de clasificación:
1. **Regresión Logística**
2. **Naive Bayes**
3. **Bosques Aleatorios (Random Forest)**

## Implementación de Modelos de Clasificación

Los datos se dividieron en conjuntos de entrenamiento y prueba. Se entrenaron y evaluaron los modelos utilizando métricas como precisión, precisión ponderada, recall ponderado y F1 ponderado.

## Resultados Obtenidos del Modelado

El modelo de Naive Bayes demostró ser el más eficaz, con un rendimiento consistente y adecuado para el manejo de grandes volúmenes de datos en un entorno Big Data.

## Recomendaciones

1. **Mejora del Servicio al Cliente**: Capacitación continua del personal y comunicación clara de políticas y cargos adicionales.
2. **Mejora de la Comodidad y Servicios a Bordo**: Mejorar la ergonomía y el espacio de los asientos.
3. **Optimización de la Relación Calidad-Precio**: Revisar políticas de precios y ofrecer promociones estratégicas.
4. **Monitoreo y Mejora Continua**: Implementar un sistema de retroalimentación continuo y actualizar regularmente los modelos de clasificación.

## Próximos Pasos

1. **Ampliación del Análisis**: Segmentar a los clientes por variables adicionales y evaluar variaciones en los sentimientos según la temporada o eventos específicos.
2. **Integración con Sistemas Operativos**: Automatizar la clasificación de comentarios y generar informes de satisfacción en tiempo real.
3. **Expansión de la Investigación**: Incluir datos de redes sociales y realizar análisis comparativos con otras aerolíneas.

## Conclusiones Generales

Este proyecto ha demostrado el valor del análisis de sentimientos en la comprensión de la percepción del cliente y ha proporcionado un marco práctico para la implementación de mejoras continuas. Con una implementación adecuada de las recomendaciones y una adaptación proactiva a las necesidades y expectativas de los pasajeros, la aerolínea puede mejorar significativamente la satisfacción del cliente y su competitividad en el mercado.

## Referencias

-
