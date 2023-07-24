
<a name="readme-top"></a>

#                                                 PROYECTO SHARK ATTACKS

![shark_img](https://github.com/borjadola/Proyecto-Sharks_Attacks/assets/132678800/22ef5f38-36c6-4d34-8b28-389fff95026e)



##  PROYECTO 

El objetivo de este proyecto es la aplicación de métodos de limpieza de bases de datos con la biblioteca de pandas y realizar un análisis superficial de los datos. Para ello se han tenido una serie de condiciones automarcadas; no borrar columnas, no borra más filas que las duplicadas, en una franja de tiempo de 3 días completos.


## OBJETIVOS 

Ver la relación que presentan las principales especies de tiburones y sus ataques durante un intervalo de tiempo,a sí como la mortalidad de estos ataques.


## PROCESO

Para el planteamiento del proceso de limpieza de la base de datos se ha optado por ejecutar el siguiente orden de acción por cada columna:

- Realizamos una tranformación inicial de cada columna quitando espacios en cada estremo del valor de cada celda y una conversión del dato a minúscula para evitar errores.

- Dependiendo del tipo de información contenida en cada columna realizamos primeramente un patrón específico de búsqueda para símbolos o letras que no tenían relación con la información de esta. Estos patrones se han llevado a cabo mediante funciones y el método REGEX.

- Una vez hecho este primer filtro, se ha procedido a un filtrado más específico de la información de cada conlumna con los métodos replace(), contains(), y funciones lambdas más epecíficas.

- Posteriormente, y cuando ya teníamos una imagen más fiel de los datos de la columna, realizamos un tercer filtrado por los valores únicos de las strings y reducirlos al máximo posible, para finalmente hacer una agrupación de valores en conceptos generales y en las columnas que lo permitían.

- Para finalizar la limpieza, se han fusionado columnas con otras que reflejaban el mismo tipo de valor, para aumentar así la cantidad de datos útiles por columna. Las filas con valores todos los valores nulos se han descartado y los restantes se han transformado en una string con el dato "no definido".

- Para la realización del análisis gráfico se han despreciado las columnas con información no relevante para el objetivo.
  
  En este objetivo se han realizado histogramas para visulizar el ataque de las especies y la franja horaria, así como un análisis de la mortalidad por especies y su ratio. A continuación se ve representado por imágenes.

  https://raw.githubusercontent.com/borjadola/Proyecto-Sharks_Attacks/Master//Users/borja/IronHack/Proyecto-Sharks_Attacks/images

  



## 💻 FUENTE DE DATOS 

- [GLOBAL SHARK](https://www.kaggle.com/datasets/teajay/global-shark-attacks).
- [NUMPY](https://numpy.org/doc/1.18/).
- [PANDAS](https://pandas.pydata.org/).
- [PYTHON](https://docs.python.org/3/library/functions.html).
- [PLOTLY](https://plotly.com/python/).
- [MATPLOTLIB](https://matplotlib.org/). 
- [SEABORN](https://seaborn.pydata.org/).





<p align="center">👆<a href="#readme-top">SUBIR</a>👆</p>


