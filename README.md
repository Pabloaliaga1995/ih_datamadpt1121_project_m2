OBJETIVOS
- Limpiar tabla mediante querys de SQL para poder trabajar con ella en Power BI o Tableau
- Realizar los gráficos pertinentes para poder conseguir un dashboard explicatorio

ENV
We have created a new environment (project2) and installed and import (import + "name of the library") therein the following library:
- Python 3.7 (conda install python == 3.7)
- Pandas (conda install pandas)
- Sqlalchemy (conda install sqlalchemy)
- Sqlite 3 (conda install sqlite)

CODE
- Importar database:
     - diamonds_m2
Después de importar la base de datos, hemos realizado inner joins para conseguir una nueva tabla, la cual hemos sacado a partir de un dataframe con Pandas, conectandonos a la base de datos.

Posteriormente hemos guardado el dataframe como CSV para poder comenzar a trabajar con el en Power BI.

En Power BI, para nuestro gráfico, los valores que hemos tomado han sido Ciudad, Precio y media de quilares por corte, por claridad y color.

He dejado a parte de este dashboard las dimensiones (Depth, table) debido a que, en las muestras de nuestra tabla, todas comprendían el rango de los que se considera ideal, en torno a un 50% y 60%.

De lo que hemos observado, el precio del diamante, depende en mayor medida del número de quilates, seguido del corte que tenga éste, siendo mejores, los cortes premium, ideal, very Good… aunque existen casos en los cuales el precio es inferior a pesar del corte, debido al menor número de muestras. Asimismo, en menor medida influyen claridad y color.

En cuanto al color, los que normalmente utilizan las grandes marcas son DEF (Sin color) Y GHIJ (Casi sin color). Estos son los que se muestran en nuestra tabla, sin tener muestras de colores amarillos que son de menor calidad, por lo que no podemos considerarlo un factor determinante en el precio. 

La claridad, los mejores son FL, de los cuales no tenemos ninguna muestra, IF, VVS1 y VVS2, seguidos de VS1, VS2, SI1… aunque existen casos que, con una claridad IF, el precio es inferior a un SI1, esto se debe a que hay un menor número de IF que de SI1, por lo que el número de quilates disminuye y con ello, el precio.

Otro factor importante, es que, normalmente, las cualidades van ligadas entre sí, un diamante premium, suele tener un mayor número de quilates, una mayor claridad y prácticamente sin color, por lo que el precio será más alto.

En resumen, la cualidad predominante para el incremento del precio de los diamantes es el quilate, aunque se dan casos, como comentabamos, en los cuales el precio puede disminuir o incrementar dependiendo de la claridad o corte.


