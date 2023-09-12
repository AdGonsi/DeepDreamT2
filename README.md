# DeepDreamT2
Este repositorio contiene el desarrollo del equipo DeepDream Team del taller 2 del curso INF398.

Para ejecutar los códigos incluidos en este repositorio se deben guardar los datos en una carpeta llamada **Data**

## Overview
Este desafío consiste en lograr mediante el uso de distintas técnicas de preprocesamiento, la creación de un dataset capaz de ilustrar correctamente el problema de predicción de riesgo crediticio. Facilitando así el entrenamiento y obtención de buenos resultados en modelos de aprendizaje automático.

## Descripción
### Problema
En este desafío exploraremos el problema de predecir si una solicitud de crédito a un banco será pagada o no, una versión binaria de lo que se denomina análisis de riesgo, que es su vez una de las aplicaciones más comunes del aprendizaje automático en la industria financiera. Esta intersección tecnología + industria financiera (Fintech) es una de las áreas laborales de mayor crecimiento reciente.

Las clases serán:

* 1: El préstamo solicitado no será pagado o el cliente experimentará problemas/retardos en el pago.
* 0: El préstamo será pagado en los términos establecidos en la solicitud.

### Materiales
Para predecir la clase, se dispondrá de varios atributos de la solicitud, de la clase correcta para los casos de entrenamiento, y de atributos de contexto que describen el comportamiento previo del cliente. Esto último (el contexto o historia del cliente) hace que este desafío permita el uso de varios dataframes, familiarizadlos con una situación típica en datos reales.

## Evaluación
### Test/Train
Como es usual dispondrá de un conjunto de pruebas y de un conjunto de entrenamiento. Para el conjunto de entrenamiento ustedes conocerán los atributos de la solicitud y la clase correcta. Para el conjunto de pruebas ustedes conocerán los atributos de la solicitud, desconocerán la clase correcta y deben predecirla.

### Submission Format
Sus predicciones deben ser enviadas a la plataforma en un archivo CSV simple de dos columnas: la primera contiene el identificador del caso de pruebas (SK_ID_CURR) y la segunda corresponde a su predicción.

> ID,TARGET
    1,1
    2,0
    3,1
    etc.

**A veces se generan problemas cuando se deja un espacio blanco luego de la coma. Evitar.**

### Métrica
Las predicciones enviadas serán comparadas con la clase correcta usando AUC (área bajo la curva ROC).