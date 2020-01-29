> Signed and unsigned types use the same amount of storage space and have the same performance, so use whatever’s best for your data range.
>
> - [High Performance MySQL, Capítulo 4](https://www.oreilly.com/library/view/high-performance-mysql/9781449332471/ch04.html)

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


Excelente evaluación general de MySQL por medio de lecturas lógicas y físicas
http://uvadoc.uva.es/bitstream/handle/10324/14120/TFG-G1192.pdf?sequence=1&isAllowed=y

Esteban Mínguez, S. (2015). Solución a un problema de Rendimiento en MySQL. Optimización de UVa Online Judge.


Posibles ideas de estructuras

10.1145/1878537.1878641

10.1109/IC3.2014.6897167

10.1002/jcb.25049 *MySQL performance evaluation*

Good MySQL internals exaplanation

https://pdfs.semanticscholar.org/c2d3/ff75ede2c2dbd9303f8b13a437d94efb98f9.pdf

Posible database benchmarking tools

https://www.hammerdb.com/

https://github.com/STSSoft/DatabaseBenchmark


---

> An Updated Performance Comparison of Virtual Machines and Linux Containers

10.1109/ISPASS.2015.7095802

---

> Performance Comparison for Data Storage - Db4o and MySQL Databases 

10.1109/IC3.2014.6897167

---

> MySQL Performance Analysis on a Limited Resource Server:  Fedora vs. Ubuntu Linux 

10.1145/1878537.1878641

---

> Solución a un problema de Rendimiento en MySQL

http://uvadoc.uva.es/bitstream/handle/10324/14120/TFG-G1192.pdf?sequence=1&isAllowed=y

---

> Benchmarking Database Performance for Genomic Data

10.1002/jcb.25049

---

> Pipes, Jay. "Performance tuning best practices." (2010).

http://bbs.linuxtone.org/docs/ebooks/MySQL/performance-tuning-best-practices.pdf

---
