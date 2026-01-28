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

Primero se visualizó el conjunto de datos graficando la luminosidad en función de la masa estelar para analizar la forma de la relación. Luego se implementó el modelo de regresión lineal junto con la función de pérdida MSE. A continuación, se derivaron y calcularon los gradientes y se aplicó el algoritmo de gradiente descendente, evaluando su convergencia y estabilidad. Posteriormente, se realizaron experimentos utilizando distintos valores de learning rate y se compararon los parámetros y pérdidas finales. Finalmente, se representó el ajuste del modelo sobre los datos y se analizaron los errores sistemáticos y las limitaciones del modelo lineal.

### NoteBook2

Primero se visualizó el conjunto de datos mostrando la relación entre masa, luminosidad y temperatura. Luego se construyó la matriz de características usando NumPy y se implementaron la función de pérdida MSE y sus gradientes de forma vectorizada. Después, se entrenaron los modelos mediante gradiente descendente y se analizó la convergencia. A continuación, se compararon los modelos M1, M2 y M3 evaluando su pérdida y predicciones. Finalmente, se analizó el efecto del término de interacción y se realizó una predicción para una nueva estrella, verificando que el resultado fuera razonable.

## Resultados y Analisis

### NoteBook1

El gráfico final muestra que el modelo presenta errores sistemáticos. En particular, tiende a sobreestimar la luminosidad en estrellas de baja masa y a subestimarla en estrellas de mayor masa. Este patrón indica que el error no es aleatorio, sino que sigue una tendencia clara a lo largo del rango de masas.

Este comportamiento sugiere que el modelo lineal tiene una capacidad limitada para describir correctamente la relación entre masa y luminosidad. Al asumir una relación recta entre ambas variables, el modelo no logra capturar el aumento cada vez más rápido de la luminosidad a medida que la masa crece. Por esta razón, el modelo lineal resulta insuficiente y se hace necesario considerar modelos más flexibles que puedan representar mejor esta relación.

### NoteBook2

En este notebook, la incorporación de términos polinomiales y de interacción permitió mejorar el ajuste del modelo respecto a versiones más simples. Al comparar M1, M2 y M3, se observó una reducción de la pérdida y una mejor coincidencia entre valores reales y predichos. El análisis del término de interacción confirmó su relevancia, y la predicción para una nueva estrella resultó coherente con la tendencia de los datos.

## Evidencia de Ejecucion en AWS SageMaker

#### Descripcion

Los notebooks se subieron a el sage maker descargando los archivos guardados en el repositorio de github o desde el editor de codigo que se este usando, en este caso VSC. Una vez descargado los notebooks se abre el sageMaker y tendra la interfaz de VSC, se abren los archivos descargados desde el sageMaker y se inicia la ejecucion.

### NoteBook1

#### Capturas

<img width="1743" height="965" alt="Captura de pantalla 2026-01-27 201700" src="https://github.com/user-attachments/assets/1b4f8d9a-c19c-447b-a103-99607dc446cd" />

<img width="1751" height="938" alt="image" src="https://github.com/user-attachments/assets/81016ddb-faf8-42ef-ba97-6ccb538247f3" />

<img width="1712" height="961" alt="image" src="https://github.com/user-attachments/assets/217e450a-2c7e-4f5e-919b-c758290a925f" />



### NoteBook2

<img width="1796" height="932" alt="image" src="https://github.com/user-attachments/assets/0e42b0a9-81c8-439d-846a-e822ee3d2d94" />

<img width="1755" height="953" alt="image" src="https://github.com/user-attachments/assets/612b2de6-775e-41f1-99ac-75ec3e0febae" />

<img width="1709" height="968" alt="image" src="https://github.com/user-attachments/assets/8d20cedc-fa8b-4797-bb7f-128df334b6b8" />

<img width="1785" height="953" alt="image" src="https://github.com/user-attachments/assets/7dc618c1-6c8d-4bc3-8c2f-b9ea85475b3a" />


### Comparacion

En mi opinion, no hubo diferencia alguna entre la ejecucuin del trabajo localmente y la de SageMaker. La experiencia fue exactamente la misma, lo unico que cambiaba es que una se hacia de manera remota y otra localmente.

## Creado con

Python
NumPy
Jupyter Notebook
AWS SageMaker

## Autor

Daniel Esteban Rodriguez Suarez

## Agradecimientos

Al profesor de la materia TDSE por la guia academica
