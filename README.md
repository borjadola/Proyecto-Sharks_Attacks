
<a name="readme-top"></a>

#                                                 PROYECTO SHARKS ATTACKS

<img width="478" alt="Principal" src="https://github.com/borjadola/Proyecto-Sharks_Attacks/assets/132678800/054e9326-b4fd-4b4b-8815-f3a252e49448">



##  PROYECTO 

El objetivo de este proyecto es la aplicación de métodos de limpieza de bases de datos con la biblioteca de pandas y realizar un análisis superficial de los datos. Para ello se han tenido en cuenta una serie de condiciones automarcadas; no borrar columnas, no borra más filas que las duplicadas, en una franja de tiempo de 3 días completos.


## OBJETIVOS 

Ver la relación que presentan las principales especies de tiburones y sus ataques durante un intervalo de tiempo, así como la mortalidad de estos ataques.


## PROCESO

Para el planteamiento del proceso de limpieza de la base de datos se ha optado por ejecutar el siguiente orden de acción por cada columna:

- Realizamos una tranformación inicial de cada columna quitando espacios en cada estremo del valor de cada celda y una conversión del dato a minúscula para evitar errores.

- Dependiendo del tipo de información contenida en cada columna realizamos primeramente un patrón específico de búsqueda para símbolos o letras que no tenían relación con la información de esta. Estos patrones se han llevado a cabo mediante funciones y el método REGEX.

- Una vez hecho este primer filtro, se ha procedido a un filtrado más específico de la información de cada conlumna con los métodos replace(), contains(), y funciones lambdas más epecíficas.

- Posteriormente, y cuando ya teníamos una imagen más fiel de los datos de la columna, realizamos un tercer filtrado por los valores únicos de las strings y reducirlos al máximo posible, para finalmente hacer una agrupación de valores en conceptos generales y en las columnas que lo permitían.

- Para finalizar la limpieza, se han fusionado columnas con otras que reflejaban el mismo tipo de valor, para aumentar así la cantidad de datos útiles por columna. Las filas con todos los valores nulos se han descartado y los restantes se han transformado en una string con el dato "no definido".

- Para la realización del análisis gráfico se han despreciado las columnas con información no relevante para el objetivo.
  
  En este objetivo se han realizado histogramas para visulizar el ataque de las especies y la franja horaria, así como un análisis de la mortalidad por especies y su ratio. A continuación se ve representado por imágenes.

![Histo_ataques-tiempo](https://github.com/borjadola/Proyecto-Sharks_Attacks/assets/132678800/abd19541-3dcc-4dab-b56c-673c3fb7191e)

REPRESENTACIÓN DE LOS DATOS DE ATAQUES DE TIBURÓN POR INTERVALO DE TIEMPO EN UNA DÍA.

Observamos que durante la mañana es el intervalo de tiempo donde más ataques se producen. También hay que tener en cuenta que probablemente sea el intervalo de tiempo dónde más personas realizan actividades en el mar.

![Histo_ataques-especies](https://github.com/borjadola/Proyecto-Sharks_Attacks/assets/132678800/dfd21018-a2e7-48d5-82cd-134c8ef8cea5)

![Histo_ataques-especies](https://github.com/borjadola/Proyecto-Sharks_Attacks/assets/132678800/2ce6ac1f-9b95-4fe9-8e30-168c9656cbd3)

REPRESENTACIÓN DE LOS ATAQUES POR EL TOP 5 DE ESPECIES Y EL INTERVALO DE TIEMPO EN EL QUE ATACAN.

Teniendo en cuenta las especies más representativas en la base de datos. Observamos como el Tiburón Blanco es el animal con mayor número de ataques, y en general, los ataques se producen durante la mañana, independientemente de la especie.

![Histo_ratio](https://github.com/borjadola/Proyecto-Sharks_Attacks/assets/132678800/706be1a5-f2cc-4906-98e1-ad842228d80d)

RATIO DE MORTALIDAD.

En este ratio podemos observar como, aunque el Tiburón Blanco es la especie con mayor número de ataques, la relación entre la mortalidad de sus ataques y la especie, arrojan que el Tiburón Tigre es la especie con mayor mortalidad de todas.

  



## 💻 FUENTE DE DATOS 

- [GLOBAL SHARK](https://www.kaggle.com/datasets/teajay/global-shark-attacks).
- [NUMPY](https://numpy.org/doc/1.18/).
- [PANDAS](https://pandas.pydata.org/).
- [PYTHON](https://docs.python.org/3/library/functions.html).
- [PLOTLY](https://plotly.com/python/).
- [MATPLOTLIB](https://matplotlib.org/). 
- [SEABORN](https://seaborn.pydata.org/).





<p align="center">👆<a href="#readme-top">SUBIR</a>👆</p>


