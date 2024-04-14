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
La medicina perioperatoria es campo crítico que abarca el cuidad preoperatorio, intraoperatorio y postoperatorio de pacientes sometidos a cirugía. Las complicaciones que surgen en el proceso postoperatorio constityen un reto para el personal de salud y son impredecibles; se pueden dar de forma súbita y pueden conllevar con rápidez hacia la muerte. Muchos de los pacientes requiern ser sometidos a UCI para ser monitoreados constantemente.[1]
Para garantizar una asistencia segura y reducir los daños a los pacientes, es necesario eliminar o reducir los factores de riesgo de un determinado evento. Por ello, se hace indispensable un reconocimiento previo de las necesidades presentadas por el paciente y así evitar tales episodios. [2]
Cada año alrededor de 200 millores de personas son sometidas a una cirugía mayor y de ellos fallecen cerca de un millón a nivel mundial. El cuidado postquirúrgico está determinado por la gravedad del paciente y elconocimiento de los factores involucrados con la mortalidad postoperatoria para tomar una mejor decisión clínica en cuanto a la administración de soluciones, monitoreo de signos vitales y suministro de medicamentos prescritos [3]. En el caso de Perú, tambien se cuenta con esta problemática y las cirugias que cuenta con mayor riesgo postoperatorio son las cirugias abdominales con una tasa de mortalidad a corto plazo que oscila entre el 15% y el 20%, siendo solo superada por la cirugía aórtica de emergencia.[4]
Actualmente la Inteligencia Artificial (IA), se ha aplicado de diversas doramas en el ámbito médico para ayudar en el diaagnóstico y prevención de enfermedades [5]. Por ello, la IA tambien puede ser utilizada para la predicción de complicaciones postoperatorias y así disminuir los casos de enfermedad, la mortalidad y los costos de atención médica en hospitales y el lapso de internación hospitalaria, mejorando los resultados de los paciente sometidos a cirugía. [6][7]
Para poder generar un modelo de IA, es necesario contar con una grande base de datos que este verificada y sea de confianza. De esta manera, se podrá obtener modelos predictivos basados en el aprendizaje automático. Actualmente, se cuenta con una base de datos de investigación colaborativa llamado INSPIRE, el cual será de gran ayuda desarrollar los modelos propuestos. [10]



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

 - Edad
  
 - Índice de comorbilidad de Charlson
  
 - Antecedentes quirúrgicos abdominales
  
 - Diagnóstico quirúrgico etiológico
  
 - Cirugía realizada 
  
 - Pruebas de laboratorio en el primer día postoperatorio 

 - Fecha de alta hospitalaria
  
 - SOFA (Sistema de evaluación de la aparición y evolución del Fallo Multiorgánico ) al ingreso a UCI 
  
 - APACHE II -UCI
  
 - Estancia en unidad de cuidados intensivos
  
 - Condición de egreso

  3- Implementar sistemas de vigilancia y alerta temprana para detectar y prevenir complicaciones postoperatorias, como infecciones o trombosis venosa profunda.
  
 - Edad
   
 - Índice de comorbilidad de Charlson
   
 - Antecedentes quirúrgicos abdominales
   
 - Diagnóstico quirúrgico etiológico
   
 - Diagnóstico de ingreso a unidad de cuidados intensivos
   
 - Cirugía realizada 
   
 - SOFA (Sistema de evaluación de la aparición y evolución del Fallo Multiorgánico ) al ingreso a UCI :  
   
 - APACHE II -UCI
   
 - Pruebas de laboratorio en el primer día postoperatorio 
   
 - Fecha de alta hospitalaria
   
 - Estancia hospitalaria
   
 - Estancia en unidad de cuidados intensivos
   
 - Condición de egreso

   

