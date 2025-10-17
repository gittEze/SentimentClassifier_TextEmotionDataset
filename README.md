# Clasificación de Sentimientos con Regresión Logística

Este colab utiliza **Procesamiento de Lenguaje Natural (PLN)** y **Machine Learning** para predecir el **sentimiento** de publicaciones.  
El objetivo es clasificar si un texto tiene un sentimiento **negativo (0)** o **positivo (1)**, aplicando el modelo **Regresión Logística** sobre datos de texto previamente vectorizados.

---

## Preparación de los datos

Durante la etapa de preprocesamiento se realizaron las siguientes acciones:

- Carga del dataset `dataset_train.csv`, con las columnas:  
  `id`, `user`, `text`, `date`, `emotion`, `sentimento`.
- Verificación de valores faltantes.  
- División del conjunto de datos en entrenamiento (90%) y prueba (10%).  
- Transformación del texto en vectores numéricos usando **CountVectorizer**.  
- Entrenamiento del modelo con **Regresión Logística** para realizar la clasificación.  
- Generación de predicciones sobre el conjunto `dataset_test_sin_sentimento.csv`.  
- Exportación de los resultados al archivo `submission3.csv`.

---

## Variables utilizadas

### Variables de entrada (X)
- `text`.

### Variable objetivo (y)
- `sentimento`.
  (0 = Negativo, 1 = Positivo)

---

