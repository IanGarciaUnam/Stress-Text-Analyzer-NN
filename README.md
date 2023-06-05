# Stress-Text-Analyzer-NN

En el desarrollo de este proyecto busqué realizar la comparación de una red Neuronal multicapas contra un recurrente para la clasificación de texto.

## Clasificación

En el archivo ```Stress.csv``` se encuentra los textos de ejemplo, descargados de un servidor de discord, con diversas etiquetas añadidas de acuerdo al tipo de trastorno al que fueron etiquetados en el mismo servidor. Cargados con 0 o 1 para diferenciar aquellos textos que no reflejan estrés de los que sí.

## Red Neruronal Multicapas
Esta primer red es bastante pequeña, pero utiliza las etiquetas de trastornos y las etiquetas de estrés para entrenarse. De igual forma la entrada requerirá de estos tres. Logro un accuracy del 62%

## Red Neuronal recurrente
Esta segunda red tiene una infraestructura adecuada para el problema, sin embargo, el entrenamiento no ha avanzado más del 55% pero tiene amplías capacidades de detección. Probando con muestras de 10 ejemplares, obtuve hasta un 70% de correctez.
Esta utiliza las mismas etiquetas de trastornos o ámbito al que se refiere, semejante a la anterior

## Conclusiones y resultados
En este proyecto pude aplicar mi aprendizaje adquirido a través de bastante esfuerzo durante el curso, bastante (Creo que notarán mi curva de aprendizaje respecto a las práctica e incluso los exámenes). Sin embargo mis resultados aún me parecen inesperados, puesto que como la red recurrente es la adecuada para este tipo de problemas, no esperaba que mantuviera un accuracy menor respecto a la otra. Pero es posible que necesite más entrenamiento o yo tenga un sesgo por el cuál los datos aún no logran mejorar.


## Aplicaciones del proyecto
Naturalmente este proyecto arraiga aplicaciones médicas por la detección de estrés en texto. Pero también lo he pensado en una forma de eficientizar la administración de recursos humanos. Sería posible cuantificar el estrés en un equipo a lo largo del proyecto, canalizar a descansos o redistribuir las cargas de trabajo para una mejora del bienestar y la eficiencia.
Asimismo tiene cabida en la vida académica, permitiendo detectar el estrés entre alumnos y académicos para así tomar decisiones que pudieran impactar y mejorar la calidad de vida y educación de ambos sectores.

## USO

Tras la carga de todos los módulos, en la parte inferior final del jupyter notebook, podremos observar la llamda a la función sample, misma que le permite ingresar texto, en inglés, para finalmente devolver la etiqueta Stress o No-Stress.

## Camino de mejora
Con una interfaz y enlazado a más sistemas de métricas y más información, como edad, género, enfermedades subyacentes, etc. Podría diagnosticar trastornos mentales o dar un acercamiento al médico sobre ello. Este proyecto puede tener crecimiento como una herramienta para el manejo, control y detección de enfermedades o malestares psicológicos. Sin llegar a substituir la mano experta del diagnóstico médico.