## Objetivos
Evaluar las diferencias del rendimiento de consultas a una base de datos con la diferencia de unsigned en enteros, y posiblemente en flotantes (dobles (?)) con los siguientes casos de uso en consideración.

- Inserción de una columna con autoincremento en int  (caso práctico, ID)
- Inserción de una columna sin autoincremento en int (posiblemente en otras también)
- Consulta de una base de datos relacional con esquemas signed y unsigned (relaciones de ID's)
- Inner Joins, Outer Joins y demás respecto a unsigned.
- Consulta de sumatorias, multiplicaciones y `GROUP BY` en general de cualquier tipo de dato

Lo ideal es conocer si tenemos alguna referencia respecto a unsigned, y signed data.

Los dos escenarios principales son:
- El performance respecto a ID's. Inserción, actualización, y muestreo de los datos. Esto afecta enormemente a datos relacionales y bases de datos con chequeo de multiples tablas.
- El performance de Sumas, multiplicaciones y tratamiento de datos en general.


## Delimitaciones

De acuerdo al artículo **10.1002/jcb.25049** las pruebas se hicieron en una computadora personal, con *100 simulations*... supongo que no tienen que ser millones de pruebas con millones de datos.

## Referencias y datos generales

Interesante estructura y organizacion de archivos Latex

https://github.com/montyluis/paper


Posibles ideas de estructuras

10.1145/1878537.1878641

10.1109/IC3.2014.6897167

10.1002/jcb.25049 *MySQL performance evaluation*

Good MySQL internals exaplanation

https://pdfs.semanticscholar.org/c2d3/ff75ede2c2dbd9303f8b13a437d94efb98f9.pdf

Posible database benchmarking tools

https://www.hammerdb.com/

https://github.com/STSSoft/DatabaseBenchmark

