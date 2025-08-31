# Semana 4

**Álgebra Relacional**

Las operaciones del álgebra relacional sirven para hacer consultas a una base de datos. Es preciso conocer estas operaciones porque nos permiten saber qué servicios de consulta debe proporcionar un lenguaje relacional. Otro aporte de esta rama del álgebra es que facilita la comprensión de algunas de las construcciones del  lenguaje SQL. Además, constituye la base para el estudio del tratamiento de las consultas que efectúan los SGBD internamente (especialmente en lo que respecta a la optimización de consultas).

Sobre la clasificación de las operaciones empleadas en el álgebra relacional, pondremos atención en la clasificación según las relaciones que tiene como operandos; por lo que podemos agruparlas en:

* Operaciones binarias: son las que tienen dos relaciones como operandos. Son binarias todas las operaciones, excepto la selección y la proyección.

* Operaciones unarias: son las que tienen una sola relación como operando. La selección y la proyección son unarias.

* Operaciones conjuntistas: son las que se parecen a las de teoría de conjuntos. Se trata de la unión, la intersección, la diferencia y el producto cartesiano.

***

*Selección:*

operación que sirve para elegir algunas tuplas de una relación y eliminar el resto (Más concretamente, la selección es una operación que, a partir de una relación, obtiene una nueva relación formada por todas las tuplas de la relación de partida que cumplen una condición de selección especificada).

ejemplo grafico:

![24](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/24.jpg "24")

***

*Proyección:*

Podemos considerar la proyección como una operación que sirve para elegir algunos atributos de una relación y eliminar el resto (Más concretamente, la proyección es una operación que, a partir de una relación, obtiene una nueva relación formada por todas las tuplas de la relación de partida que resultan de eliminar unos atributos especificados. El resultado no tiene tuplas duplicadas).

![25](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/25.jpg "25")

***

*Unión:*

La unión es una operación que, a partir de dos relaciones, obtiene una nueva relación formada por todas las tuplas que están en alguna de las relaciones de partida. La unión de dos relaciones T y S se indica T  ∪ S. Elimina las tuplas repetidas.

***

*Interección:*

La intersección es una operación que, a partir de dos relaciones, obtiene una nueva relación formada por las tuplas que pertenecen a las dos relaciones de partida. La intersección de dos relaciones T y S se indica T ∩ S.

***

*Diferencia:*

La diferencia  es una operación que, a partir de dos relaciones (Tabla1 - Tabla2), obtiene una nueva relación formada por todas las tuplas que están en la primera relación y, en cambio, no están en la segunda.

La diferencia entre las relaciones T y S se indica como T – S.

***

*Producto cartesiano:*

El producto cartesiano es una operación que, a partir de dos relaciones (Tabla1 X Tabla2), obtiene una nueva relación formada por todas las tuplas que resultan de concatenar tuplas de la primera relación con tuplas de la segunda.

![26](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/26.jpg "26")

***

*Producto cartesiano natural:*

El producto cartesiano natural es una operación que, a partir de dos relaciones, obtiene una nueva relación formada por todas las tuplas que resultan de concatenar tuplas de la primera relación con tuplas de la segunda siempre y cuando tengan el mismo valor del atributo en común.

![27](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/27.jpg "27")

***

