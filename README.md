# Tarea-DM
Tarea mediante la cual se selecciona un algoritmo de machine learning, se explica y se muestra un ejemplo
Link colab (es el mismo código que el .ipynb): https://colab.research.google.com/drive/1flwpbW7IaZtEhNomH1cqOh8DmlPWe6mY#scrollTo=qN8dW1mbRrN1


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Modelo XGBoost de clasificación

Breve explicación:

XGBoost es una herramienta de aprendizaje automático que se utiliza para clasificar datos en diferentes categorías. En lugar de predecir un número, como en otros modelos, XGBoost predice etiquetas o clases.

En este ejemplo, el modelo predice si un empleado asistirá o no al trabajo basándose en características como el día de la semana, día del mes o la tienda en la que trabaja.

Su funcionamiento se basa creando una serie de árboles de decisiones, para luego, con cada nuevo árbol se mejora el anterior, aprendiendo de sus errores para hacer mejores predicciones.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Datos implementados:

Se tienen datos históricos de las asitencias del personal de una empresa. Se busca crear un modelo de clasificación mediante el cual podamos predecir los días en que la persona tendrá inasistencia. Como parámetros tenemos el id del empleado, la fecha, el día de la semana, el día del mes, la evaluación de la asistencia (1 = asistencia, 0 = ausencia)


-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


Análisis de resultados 

Vemos que en general el modelo tiene un buen desempeño pero cuando se evaluan asistencias e inasistencias, las inasistencias muestran un menor desempeño debido.

Esto puede ser en parte por la naturaleza del negocio donde no todas las personas asisten 6 días a la semana por uno de descanso. Hay figuras que tienen contratación por 1, 2 ó 3 días a la semana lo que nos puede estar generando ruido en este análsis. Otra area de mejora sería ver si no hay gente dada de baja a la cual le esté contando muchas inasistencias y que esté generando ruido ya que en este rubro la tasa de rotación llga a ser hasta del 25% de la plantilla.

