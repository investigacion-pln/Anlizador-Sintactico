# Analizador Sintáctico

<p style='text-align: justify;'>
El análisis sintáctico parcial hoy en día ha sido utilizado en las tareas de extracción de información y minería de textos, específicamente, los analizadores sintácticos probabilísticos los cuales permiten la obtención de subestructuras y estructuras del árbol más posible de una sentencia dada.
</p>

## Website
[Analizador sintáctico](http://eiscapp.univalle.edu.co/bikel/parser/index.php)

## Objetivo

<p style='text-align: justify;'>
El análisis sintáctico parcial se caracteriza en predecir la estructura de frases en forma de árbol para una sentencia dada en lenguaje natural. Este tipo de análisis se realiza bajo el enfoque basado en corpus donde éste es el insumo anotado manualmente con estructuras sintácticas. 
</p>

## Metodología
<p style='text-align: justify;'>
Un algoritmo de aprendizaje de máquinas suministra el modelo de aprendizaje sobre el corpus y anota automáticamante la estructura sintáctica de una sentencia de entrada. Un analizador sintáctico parcial puede ser denominado como un analizador sintáctico probabilístico el cual consiste de un corpus anotado sintácticamente, un modelo probablístico para el manejo de las dependencia entre variables y un enfoque de aprendizaje supervisado para la obtención del modelo de aprendizaje. 
</p>

## Precisión
<p style='text-align: justify;'>
El rendimiento de estos analizadores depende de los corpus y de las capacidad de las modelos para cada lenguaje, por ejemplo, para el idioma inglés el rendimiento está entre el 80% y 90% mientras que para el idioma español está en el 85 %. La capacidad de los modelos a su vez depende de la variabilidad y uso de las características para reponder a los fenómenos linguísticos de cada idioma. 
</p>

## Marco Teórico
<p style='text-align: justify;'>
Se han realizado muchos trabajos que aportan a la precisión en la inferencia de estas estructuras de frase basados en técnicas probabilísticas. Michael Collins propone tres modelos probabilísticos; el primero basado en reglas de gramáticas libres de contextos probabilísticas lexicalizadas, donde la tarea es encontrar el núcleo sintáctico de la frase. 
</p><br/>
<p style='text-align: justify;'>
En el segundo modelo adiciona un componente para las distinción entre adjunción y complementación, y en el tercer modelo integra rastros de movimientos del núcleo sintáctico y adiciona la característica de diferencia en los nodos no-terminales. Mas adelante, Dan Bikel propone una metodología para la investigación de modelos probabilísticos que abordan el problema del análisis sintáctico. 
</p>

## Conclusiones
<p style='text-align: justify;'>
En este trabajo se usó la implementación de Bikel con el objetivo de estudiar los modelos de análisis sintácticos probabilísticos, se obtuvieron características linguísticas para usar técnicas de máquinas de soporte vectorial y poder lograr una clasicación de los complementos que son requeridos como argumentos de los verbos. Así como lo hace el segundo modelo de Collins, se usa esta clasicación para ser contrastada con los tipos de complementos que son requeridos por el núcleo en caso de tratarse de un verbo. 
</p><br/>
<p style='text-align: justify;'>
Los tipos de complementos requeridos como argumentos se obtienen de la información léxica suministrada por ANCORA, que provee un archivo para cada lema de los verbos existentes en el idioma español. Se realizaron pruebas de validación cruzada con 610 archivos del subconjunto de ANCORA CESS ESP, presentando F1 score para el modelo de línea base xx;xx y del xx;xx para el modelo con clasicación de argumentos, de esta manera se logra una mejora del xx;xx%. 
</p><br/>
<p style='text-align: justify;'>
Este trabajo presenta un analizador sintáctico probabilístico entrenado por el corpus del idioma español ANCORA y un modelo de ajuste del analizador de Bikel usando máquinas de soporte vectorial para clasicar el tipo de complemento de los modificadores de los verbos que son argumentos.
</p>