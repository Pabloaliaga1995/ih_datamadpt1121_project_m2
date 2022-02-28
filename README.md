OBJETIVOS
- Limpiar tabla mediante queries de SQL para poder trabajar con ella en Power BI o Tableau
- Realizar los gráficos pertinentes para poder conseguir un dashboard explicatorio

ENV
Hemos creado un nuevo entorno (project2), instalado e importado (import + "name of the library") en el:
- Python 3.7 (conda install python == 3.7)
- Pandas (conda install pandas)
- Sqlalchemy (conda install sqlalchemy)
- Sqlite 3 (conda install sqlite)

CODE
En primer lugar, hemos importado la base de datos:
     - diamonds_m2

Después de importar la base de datos, mediante inner joins hemos conseguido una nueva tabla, la cual hemos exportado a un dataframe mediante Pandas.

Posteriormente hemos guardado el dataframe como CSV para poder comenzar a trabajar con el en Power BI.

Con el nuevo dataframe en CSV, los valores que hemos tomado para nuestro Dashboard han sido Ciudad, Precio y media de quilares por corte, por claridad y color.

No hemos considerado en este dashboard las dimensiones (Depth, Table) debido a que, en las muestras de nuestra tabla, todas comprendían el rango de lo que se considera ideal, en torno a un 50% y 60%.

Después de observar los valores, hemos llegado a la conclusión de que el precio del diamante depende en mayor medida del número de quilates, seguido del corte que tenga éste, siendo mejores los cortes premium, ideal, very Good… aunque existen casos en los cuales el precio es inferior a pesar del corte, debido al menor número de muestras. Asimismo, influyen en menor medida claridad y color.

En cuanto al color, los que normalmente utilizan las grandes marcas son DEF (Sin color) Y GHIJ (Casi sin color). Estos son los que encontramos en nuestra tabla, ya que no dispone de  muestras de colores amarillos que son de menor calidad, por lo que no podemos considerarlo un factor determinante en el precio. 

Por otro lado, en cuanto a la claridad, los mejores son FL, de los cuales no tenemos ninguna muestra, IF, VVS1 y VVS2, seguidos de VS1, VS2, SI1… aunque existen casos que, con una claridad IF, el precio es inferior a un SI1, esto se debe a que hay un menor número de IF que de SI1, por lo que el número de quilates disminuye y con ello, el precio.

Debemos considerar también el hecho de que, normalmente, las cualidades van ligadas entre sí. Un diamante premium suele tener un mayor número de quilates, una mayor claridad y prácticamente no tener color color, por lo que el precio será más alto que uno de menos claridad, quilates...

En resumen, la cualidad predominante para el incremento del precio de los diamantes es el quilate, aunque se dan casos, como comentabamos, en los cuales el precio puede disminuir o incrementar dependiendo de la claridad o corte.


