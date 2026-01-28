# RodriguezDaniel-Regression_and_cloud_ready_AI_infrastructure
stellar-luminosity-regression

## Descripcion

Este trabajo se enmarca dentro de un bootcamp de Machine Learning de cuatro semanas, que forma parte de un curso sobre Transformación Digital y Arquitectura Empresarial. En este enfoque, el aprendizaje automático se considera una capacidad fundamental en el diseño de los sistemas empresariales actuales.

En la actualidad, la inteligencia es vista como un atributo de calidad esencial, al mismo nivel que la escalabilidad, la disponibilidad, la seguridad y el rendimiento. Los sistemas inteligentes ya no se limitan al análisis de datos fuera de línea, sino que están integrados directamente en plataformas, servicios de soporte a la toma de decisiones y componentes con distintos grados de autonomía.

Desde la perspectiva de la arquitectura empresarial, no es suficiente conocer el funcionamiento de los modelos. Es necesario entender cómo se construyen a partir de principios básicos, cómo se ejecutan y validan en entornos controlados, y cómo se despliegan y operan en infraestructuras en la nube.

## Prerrequisitos

 Python 3.11.14
 Jupyter Notebook
 Algunas librerias como: Numpy

## Instalacion

1. Se crea el repositorio en GitHub
2. Se utiliza alguna aplicacion como VSC para poder clonar el repositorio.
3. Se crean los archivos solicitados por el repositorio (Notebooks 1 y 2)
4. En los notebooks se resuelven los ejercicios de manera organizada para que al ejecutar las celdas no genere error.

## Ejecucion

### NoteBook1

Se implementa un modelo de regresion lineal con el fin de poder hacer un analisis de la relacion entre la masa y la luminosidad.

Se define la funcion de costo MSE para implementar

## Resultados y Analisis

### NoteBook1

El gráfico final muestra que el modelo presenta errores sistemáticos. En particular, tiende a sobreestimar la luminosidad en estrellas de baja masa y a subestimarla en estrellas de mayor masa. Este patrón indica que el error no es aleatorio, sino que sigue una tendencia clara a lo largo del rango de masas.

Este comportamiento sugiere que el modelo lineal tiene una capacidad limitada para describir correctamente la relación entre masa y luminosidad. Al asumir una relación recta entre ambas variables, el modelo no logra capturar el aumento cada vez más rápido de la luminosidad a medida que la masa crece. Por esta razón, el modelo lineal resulta insuficiente y se hace necesario considerar modelos más flexibles que puedan representar mejor esta relación.

## Evidencia de Ejecucion en AWS SageMaker

### NoteBook1

#### Descripcion

Los notebooks se subieron a el sage maker descargando los archivos guardados en el repositorio de github o desde el editor de codigo que se este usando, en este caso VSC. Una vez descargado los notebooks se abre el sageMaker y tendra la interfaz de VSC, se abren los archivos descargados desde el sageMaker y se inicia la ejecucion.

#### Capturas



### NoteBook2

## Creado con

Python
NumPy
Jupyter Notebook
AWS SageMaker

## Autor

Daniel Esteban Rodriguez Suarez

## Agradecimientos

Al profesor de la materia TDSE por la guia academica
