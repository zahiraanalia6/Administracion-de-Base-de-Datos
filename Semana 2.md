# Semana 2

*Niveles de abstraccion*

* El nivel externo es el nivel de vista del usuario. Cada vista de usuario se conoce como esquema externo, con el que descubrimos alguna parte de la base de datos.

* El nivel conceptual describe la estructura lógica de toda la base de datos. El esquema conceptual se concentra en describir entidades, tipos de datos, relaciones, operaciones y restricciones.

* El nivel interno representa el esquema interno o físico. Describe cómo se almacena en disco los datos y los caminos de acceso a la base de datos.

***

 El nivel lógico o conceptual describe qué datos son almacenados realmente en la base de datos y las relaciones que existen entre los mismos. En otras palabras, describe la base de datos completa en términos de su estructura de diseño. Este nivel de abstracción lo usan los/as administradores de bases de datos, quienes deben decidir qué información se va a guardar en la base de datos. 

* Definición de los datos

    Se describen el tipo de datos. Longitud de campo todos los elementos direccionables en la base.

* Relaciones entre datos.

    Se definen las relaciones entre datos para enlazar tipos de registros relacionados para el procesamiento de archivos múltiples.

***
**Uso de los modelos**

Los modelos consisten en sistemas de diagramas o imágenes que permiten que más personas puedan participar en el diseño del sistema. Si mostramos a un usuario final un centenar de líneas de código, esto será muy difícil para su compresión; pero si mostramos a ese usuario final un diagrama de actividades, esa misma persona podrá intervenir en el proceso de trabajo.

*Ventajas:*

* Reduce los errores en el desarrollo de software de bases de datos. 

* Facilita la rapidez y eficacia en el diseño y creación de bases de datos.

* Facilita la comunicación entre los ingenieros de datos y los departamentos de inteligencia empresarial.


**Ejemplo de un modelo conceptual de datos**

![15](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/15.png "15")


***

*Modelo de datos fisicos*

Un modelo de base de datos física muestra todas las estructuras de tabla, incluidos el nombre de columna, el tipo de datos de columna, las restricciones de columna, la clave principal, la clave externa y las relaciones entre las tablas. 

*Caracteristicas:*

* Especificación de todas las tablas y columnas.

* Las claves externas se usan para identificar relaciones entre tablas. 

* La desnormalización puede ocurrir según los requisitos del usuario.

Las consideraciones físicas pueden hacer que el modelo de datos físicos sea bastante diferente del modelo de datos lógicos. Además, el modelo de datos físicos será diferente para distintos Sistemas de Gestión de Base de datos. Por ejemplo, el tipo de datos para una columna puede ser diferente entre MySQL y SQL Server.

**Pasos para diseñar un modelo de datos físicos**

* Convertir entidades en tablas. 

* Convertir relaciones en claves externas. 

* Convertir atributos en columnas. 

* Modificar el modelo de datos físicos en función de las restricciones/requisitos físicos.


![16](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/16.png "16")

***

*Modelo de datos lógicos*

Un modelo de datos lógicos describe los datos con el mayor detalle posible, independientemente de cómo se implementarán físicamente en la base de datos.

*Caracteristicas:*

* Se representan las entidades y sus relaciones.

* Se especifican los atributos para cada entidad.

* Se sitpua la clave principal para cada entidad y las claves externas (claves que identifican la relación entre diferentes entidades)

* La normalización ocurre en este nivel.


**Pasos para diseñar un modelo de datos lógicos**

* Especificar claves primarias para todas las entidades. 

* Encontrar las relaciones entre diferentes entidades. 

* Describir todos los atributos para cada entidad. 

* Resolver las relaciones de muchos a muchos. 

* Normalización.

![17](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/17.png "17")

***

*Ventajas y desventajas de los modelos de datos*

**Ventajas:**

* Permite asegurar que los objetos de datos se representen con precisión. 

* Es lo suficientemente detallado para ser utilizado para construir la base de datos física. 

* La información en el modelo de datos se puede utilizar para definir la relación entre tablas, claves primarias y externas y procedimientos almacenados. 

* Ayuda a las empresas a comunicarse dentro y entre las organizaciones. 

* Permite documentar las asignaciones de datos en el proceso ETL Ayuda a reconocer las fuentes de datos correctas para poblar el modelo.

**Desventajas:**

* Para desarrollar el modelo de datos se deben conocer las características físicas de los datos almacenados. 

* Incluso los cambios más pequeños realizados en la estructura requieren modificaciones en toda la aplicación. 

* No hay un lenguaje de manipulación de modelos establecido en DBMS.

