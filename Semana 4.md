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

**SQL**

Dada su fuerte conexión con la teoría del modelo relacional, SQL es un lenguaje de alto nivel orientado a conjuntos de registros. Esto implica que un solo comando SQL  puede equivaler a decenas o cientos de líneas de código que se tendrían que utilizar en un lenguaje de más bajo nivel orientado a registros.

Para el almacenamiento y operaciones de manipulación de los datos, el modelo relacional establece el uso de relación y variable de relación; mientras tanto SQL hace uso de las tablas como elemento fundamental.

<img width="568" height="455" alt="image" src="https://github.com/user-attachments/assets/5b1f5acb-030f-4165-a710-d329621b7405" />

*Sintaxis en SQL - DDL* 

DDL -> lenguaje de definicion de datos

Administrar un modelo físico de datos SQL presenta tres cláusulas básicas: CREATE, DROP y ALTER. Los mismos se corresponden con crear, borrar o modificar el esquema existente.

***

* Para generar una BD la sentencia SQL es:

$${\color{blue}create \space \color{white}database \space nombreBD:}$$

* Para eliminar un BD:

$${\color{blue}drop \space \color{white}database \space nombreBD:}$$

* Para generar una tabla en una BD:

$${\color{blue}create \space table \space \color{white}Socio \color{blue}(}$$

$${\color{white}CodSocio \space \color{pink}int \color{blue},}$$

$${\color{white}DNI \space \color{pink}varchar \space \color{blue}( \color{yellow}10 \color{blue}) \color{blue},}$$

$${\color{white}Nombre \space \color{pink}varchar \space \color{blue}( \color{yellow}60 \color{blue}) \color{blue},}$$

$${\color{white}Apellido \space \color{pink}varchar \space \color{blue}( \color{yellow}60 \color{blue}) \color{blue},}$$

$${\color{white}Direccion \space \color{pink}varchar \space \color{blue}( \color{yellow}30 \color{blue}) \color{blue},}$$

$${\color{white}Tel \space \color{pink}varchar \space \color{blue}( \color{yellow}15 \color{blue}) \color{blue},}$$

$${\color{blue}Constraint \space \color{white}pk-persona \space \color{blue}primary \space kay \space ( \color{white}CodSocio \color{blue})  \color{blue}) \space \color{white}engine \color{blue}= \color{white}innobd \color{blue};}$$


En este caso algunos de los atributos son:

* CodSocio con dominio entero, no puede ser nulo porque está declarado como PK.

* Nombre con dominio varchar (caracteres) y con longitud máxima 60.

***

*InnoBD*

Es un mecanismo de almacenamiento de datos de código abierto para la base de datos MySQL, incluido como formato de tabla estándar en todas las distribuciones de MySQL a partir de las versiones 4.0. Su característica principal es que soporta transacciones de tipo ACID y bloqueo de registros e integridad referencial. InnoDB ofrece una fiabilidad y consistencia muy superior a MyISAM, la anterior tecnología de tablas de MySQL, si bien el mejor rendimiento de uno u otro formato dependerán de la aplicación específica.

* Para eliminar una tabla de la BD:

$${\color{blue}drop \space \color{white}table \space nombre-tabla}$$

* Para modificar una tabla del modelo:

$${\color{blue}alter \space table \color{white}nombre-tabla \space ...}$$

* Si se quiere agregar una FK:

$${\color{blue}ALTER \space TABLE \space \color{white}nombre.tabla \space \color{blue}ADD \space FOREIGN \space ( \color{white}atributo \color{blue}) \space REFERENCES \space \color{white}Tabla \color{blue}( \color{white}Atributos \color{blue});}$$

* Si se quiere crear un atributo:

$${\color{blue}ALTER \space TABLE \space \color{white}nombre.tabla \space \color{blue}ADD \space column \space [ \color{white}Atributo \color{blue}] \space [ \color{white}Tipo \space de \space datos \color{blue}];}$$ 

***

La estructura básica de SQL tiene el siguiente formato:

$${\color{blue}SELECT \space \color{white}lista.de.atributos \color{blue};}$$

$${\color{blue}From \space \color{white}lista.de.tablas \color{blue};}$$

$${\color{blue}WHERE \space \color{white} predicado \color{blue};}$$

* Veamos que significan cada uno de estos ítems:

1. lista_de_Atributos indica los nombres de los atributos que serán presentados en el resultado; estos atributos deben estar contenidos en las tablas indicadas en la consulta.


2. lista_de_Tablas indica las tablas de la BD necesarios para resolver la consulta; sobre las tablas indicadas de la lista se realiza el producto cartesiano.

3. Predicado indica que condición deben cumplir las tuplas de las tablas para estar en el resultado final de la consulta.


***

*Ejemplo de álgebra relacional migrado a SQL*

En la siguiente tabla podemos observar como es trabajar con alguna de las operaciones que vimos en álgebra relacional, pero utilizando los conceptos vistos en SQL.


<img width="583" height="390" alt="image" src="https://github.com/user-attachments/assets/76ac692f-23b4-43b5-a727-fa8fd706ad72" />

