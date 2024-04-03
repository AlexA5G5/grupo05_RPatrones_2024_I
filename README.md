# grupo05_RPatrones_2024_I
## Grupo 05 - Reconocimiento de Patrones

El curso introduce conocimientos sobre la implementación de sistemas de computadora para el análisis de información y toma de decisiones. Se abordan conceptos sobre características en señales e imágenes, el espacio de características y reglas de decisión. Se analizan métodos de decisión estadísticos y de inteligencia artificial: Decisiones bayesianas, análisis de discriminación lineal, análisis de componentes principales, redes neuronales, máquinas de vectores de soporte, entre otros.

## Presentación del equipo

### Integrante 1: Alexander Marlon Paredes Arellano
Correo: alexander.paredes@upch.pe

<img src="Fotos/Foto Alex.jpeg" height="250" width="200">

Soy estudiante de la carrera de Ingeniería Biomédica del 9no ciclo. Mis áreas de interés son la Ingeniería de tejidos y la Ingeniería Clínica. Me interesa aprender sobre el uso de la IA para poder automatizar procesos en el caso de descelularización y cultivo de células. Considero que el uso de IA será un apoyo para los futuros proyectos en los que participe.


### Integrante 2: Angel Eduardo Dianderas Jorge
Correo: angel.dianderas@upch.pe

<img src="Fotos/Foto Angel.jpeg" height="250" width="200">

Soy un estudiante de Ingeniería Biomédica. Me gusta mucho los temas relacionados con machine learning y biomecánica para el rapido tratamiento de lesiones en pacientes y mejorar su calidad de vida.

### Integrante 3: Eduardo André Cuti Riveros
Correo: eduardo.cuti@upch.pe

<img src="Fotos/foto Cuti.png" height="250" width="200">

Soy un estudiante de ingeniería biomédica. Quisiera  especializarme en la carrera de robótica y rehabilitación ; sin embargo, considero que la programación(machine learning,deep learning,etc ) es muy importante para  desarrollar todo proyecto de esta especialidad; por ende, tengo interes en aprender de este curso llamado  reconocimiento de patrones.
## Proyecto de curso
- Descripción del proyecto
- Problemática:

La cirugía abdominal de emergencia se ha convertido en un problema crítico de salud pública, ya que es una de las principales causas de muerte en personas menores de 45 años. De hecho, la pérdida de años de vida debido a esta cirugía supera la de muchas enfermedades infecciosas, como el VIH [1]. 
Las cirugías abdominales de emergencia se deben principalmente a enfermedades del tracto gastrointestinal. Las causas más comunes incluyen la apendicitis aguda, problemas relacionados con la vesícula biliar (como la colecistitis aguda y la colangitis aguda), y la obstrucción intestinal provocada por hernias complicadas, bridas o adherencias. [2]
A pesar de que la cirugía abdominal de emergencia es común en muchos países, incluido el nuestro, a menudo la atención que se brinda no cumple con las expectativas del paciente, lo que puede tener un impacto negativo en su pronóstico. Por ejemplo, en un estudio realizado en un hospital en Lima, Perú, se encontró que alrededor del 50% de los pacientes no estaban satisfechos con la atención recibida durante su hospitalización por apendicitis aguda, colecistitis aguda y hernias inguinales complicadas. Además, esta insatisfacción se relacionaba con una estancia más prolongada en el hospital. [3]
Los pacientes sometidos a cirugías abdominales de emergencia suelen ser adultos mayores con comorbilidades y un estado físico debilitado, lo que los hace más propensos a complicaciones cardiopulmonares e infecciosas. Estas complicaciones, especialmente los cuadros sépticos, son las principales causas de muerte en el período postoperatorio. Debido a estos riesgos, esta cirugía se considera de alto riesgo, con una tasa de mortalidad a corto plazo que oscila entre el 15% y el 20%, siendo solo superada por la cirugía aórtica de emergencia. Entonces resulta importante mapear y evaluar todos los factores que conllevan a esta alta mortalidad. [4]

- Objetivos
  - Desarrollar modelos de aprendizaje automático que puedan identificar patrones de síntomas que predicen la necesidad de una cirugía abdominal de emergencia.
  - Desarrollar un modelo que permita analizar registros médicos y registros de salud electrónicos para identificar factores de riesgo preoperatorios asociados con la mortalidad y las complicaciones postoperatorias.
  - Desarrollar modelos que puedan predecir la duración de la cirugía con base en las características del paciente y la complejidad del procedimiento. Esto puede ayudar a optimizar la programación de quirófanos y la asignación de recursos.
  - Desarrollar herramientas de apoyo a la decisión que ayuden a los cirujanos a seleccionar la técnica quirúrgica más adecuada para cada paciente, considerando sus características y riesgos individuales.
  - Desarrollar modelos que puedan predecir la probabilidad de que un paciente requiera cuidados intensivos después de la cirugía.
  - Implementar sistemas de vigilancia y alerta temprana para detectar y prevenir complicaciones postoperatorias, como infecciones o trombosis venosa profunda.

- Operacionalización de la variable (target)
Se tomo 3 posibles objetivos en los cuales nos  podríamos enfocariamos . Listamos las variables(targets) requeridos para cada objetivo.

1- Desarrollar modelos que puedan predecir la probabilidad de que un paciente requiera cuidados intensivos después de la cirugía
  Edad
  
 - Índice de comorbilidad de Charlson
  
 - Antecedentes quirúrgicos abdominales
  
 - Diagnóstico quirúrgico etiológico
  
 - Cirugía realizada 
  
 - SOFA (Sistema de evaluación de la aparición y evolución del Fallo Multiorgánico ) al ingreso a UCI 
  
 - APACHE II -UCI
  
  2-Desarrollar un modelo que permita analizar registros médicos y registros de salud electrónicos para identificar factores de riesgo preoperatorios asociados con la mortalidad y las complicaciones postoperatorias.

 -Edad
  
 -Índice de comorbilidad de Charlson
  
 -Antecedentes quirúrgicos abdominales
  
 -Diagnóstico quirúrgico etiológico
  
 -Cirugía realizada 
  
 -Pruebas de laboratorio en el primer día postoperatorio 

 -Fecha de alta hospitalaria
  
 -SOFA (Sistema de evaluación de la aparición y evolución del Fallo Multiorgánico ) al ingreso a UCI 
  
 -APACHE II -UCI
  
 -Estancia en unidad de cuidados intensivos
  
 -Condición de egreso

  3- Implementar sistemas de vigilancia y alerta temprana para detectar y prevenir complicaciones postoperatorias, como infecciones o trombosis venosa profunda.
  
 -Edad
   
 -Índice de comorbilidad de Charlson
   
 -Antecedentes quirúrgicos abdominales
   
 -Diagnóstico quirúrgico etiológico
   
 -Diagnóstico de ingreso a unidad de cuidados intensivos
   
 -Cirugía realizada 
   
 -SOFA (Sistema de evaluación de la aparición y evolución del Fallo Multiorgánico ) al ingreso a UCI :  
   
 -APACHE II -UCI
   
 -Pruebas de laboratorio en el primer día postoperatorio 
   
 -Fecha de alta hospitalaria
   
 -Estancia hospitalaria
   
 -Estancia en unidad de cuidados intensivos
   
 -Condición de egreso

   

