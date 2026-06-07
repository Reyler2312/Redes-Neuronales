 Seminario IA
 Aplicación de Redes Neuronales Convolucionales en el Diagnóstico de Neumonía1. 
1.Introducción
La inteligencia artificial ha transformado el campo de la salud, ofreciendo herramientas capaces de asistir en diagnósticos médicos complejos. Entre estas, las Redes Neuronales Convolucionales (CNN) destacan por su capacidad de procesar imágenes y detectar patrones visuales. Este trabajo aborda la aplicación de CNN en la clasificación de radiografías de tórax para identificar casos de neumonía, un problema de gran relevancia clínica y social.
 2.Fundamentación Teórica
Neuronas artificiales: unidades que simulan el procesamiento biológico.Capas convolucionales: extraen características visuales como bordes, texturas y opacidades.
Pooling: reduce dimensionalidad manteniendo información relevante.
Funciones de activación: ReLU introduce no linealidad, Softmax o Sigmoid generan salidas probabilísticas.
Entrenamiento supervisado: ajuste de pesos mediante retropropagación y optimizadores como Adam.

3.Metodología
3.1 Dataset
Se emplea el Chest X-Ray dataset, compuesto por radiografías de tórax clasificadas en dos categorías:
Sano
Neumonía
3.2 Preprocesamiento
.Normalización de valores de píxeles (0–255 → 0–1).
.Redimensionamiento de imágenes a 128x128 píxeles.
.Aumento de datos: rotaciones, zoom y volteo horizontal para mejorar generalización.
3.3.Arquitectura CNN
Tres capas convolucionales con filtros crecientes (32, 64, 128).
Capas de pooling para reducción de dimensionalidad.
Capa densa oculta con 128 neuronas y ReLU.
Capa de salida con Sigmoid para clasificación binaria.
Dropout (0.5) para evitar sobreajuste.
4.Resultados Esperados
Precisión diagnóstica superior al 85% en validación.
Reducción de errores humanos en la interpretación de radiografías.
Herramienta de apoyo para médicos en entornos con recursos limitados.
5.Discusión
Las CNN ofrecen ventajas significativas en la detección de neumonía, pero presentan limitaciones:
Dependencia de datasets balanceados y representativos.
Necesidad de validación clínica antes de su implementación hospitalaria.
Riesgo de sobreajuste si el modelo no se entrena con suficientes datos diversos.
6.Conclusiones
El uso de CNN en radiografías de tórax constituye una solución viable y prometedora para el diagnóstico asistido de neumonía. Aunque no reemplaza la labor médica, sí representa un apoyo valioso en la toma de decisiones clínicas, especialmente en contextos donde los recursos humanos y tecnológicos son limitados.
7.Referencias
LeCun, Y., Bengio, Y., & Hinton, G. (2015). Deep learning. Nature.
Kermany, D. S., et al. (2018). Identifying medical diagnoses and treatable diseases by image-based deep learning. Cell.
