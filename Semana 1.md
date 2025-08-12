# Semana 1

Que es una base de datos?

*"una colección de datos interrelacionados, almacenados en conjunto sin
redundancias perjudiciales o innecesarias, garantizando la consistencia, la integridad y la seguridad de los mismos; cuyo fin es la de servir a una o varias aplicaciones, de la mejor manera posible. Los datos se almacenan de modo que resulten independientes de los programas que los usan”*

![1](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/1.png "1")

* las filas contienen datos/registros concretos.
* las columnas representan atributos/campos de cada dato/registro.

que es un dato?
* representacion simbolica.
* por si solo no significa nada.
* los datos son valores que representan hechos o realidades del mundo real

que es informacion?
* datos procesados e interpretables (puedan ser entendidos e interpretados por el receptor).

que es una base de datos?
* Las bases de datos se crearon a partir de la necesidad de las grandes empresas de almacenar grandes cantidades de información de forma rápida, sencilla y fiable, y que a su vez pudieran acceder a ella en cualquier momento sin necesidad de desplazarse a salas dedicadas a archivar documentació física (como se hacía hasta el momento). 

En la base de datos se guarda informacion de dos tipos:
* datos de ususario (usados por aplicaciones).
* datos de sistema (la base de datos utiliza para su gestion).

Para que una base de datos se considere organizada debe cumplir los siguientes objetivos:
* ser versatil.
* atender con rapidez adecuada a la aplicacion o empresa.
* indice de redundancia bajo.
* alta capacidad de acceso.
* alto indice de integridad
* nivel alto de seguridad y privacidad.
* estar actualizada.
* contar con independencia fisica y logica.

informacion:
El conocimiento derivado del analisis o tratamiento de los datos qeu se utiliza para tomar decisiones con vistas a un accionar concreto.

***

Que es un sistema de informacion?
Coleccion de datos debidamente recopilados y estructurados que proporcionan informacion sobre la realidad.

problemas de utilizacion de planillas:
* Redundancia. Al no existir algún tipo de control sobre el ingreso más que el del usuario, es muy normal que existan registros duplicados y repeticiones. 
* Error de ingreso. Al hacer un ingreso manual de datos, son frecuentes los errores de tipo de letras y números, errores ortográficos, entre otros. 
* Estandarización. Es el tipo de error más común y se ejemplifica en el ingreso de fechas donde, a pesar de poder regir el formato de entrada, se ingresan otros formatos que, si bien pueden ser correctos, interfieren en la organización de la base de datos. Por ejemplo: 21-12-2021 o bien 21/02/2021, o 21/2/2021.
* Seguridad. No hay control de uso y acceso por parte de los usuarios de los datos, más que el control al archivo físico en la computadora local o servidor.

***

Sistemas de gestion de base de datos
Es un sistema que permite la creación, gestión y administración de base de datos, asi como la eleccion y manejo de las estructuras necesarias para el almacenamiento y la busqueda de la informacion del modo mas eficiente posible.

Base de datos y SGBD
una BD es un conjunto de datos relacionados entre si. no se debe confundir BD con SGBD que proporciona una forma de alamacenar y recuperar la informacion de una base de datos de manera practica y eficiente.

Caracteristicas fundamentales de un BDMS
* Es un componente de software. 
* Garantiza disponibilidad y accesibilidad. 
* Permite el acceso concurrente a los datos. 
* Asegura la integridad transaccional.
* Protege los datos y los accesos. 
* Optimiza la performance y el rendimiento.

ACID 
Es el grupo de cautro propiedades que garantizan que las transacciones en las bases de datos se realicen de forma confiable.

Concepto ACID letra por letra:
* Atomicidad: todo o nada.
* Consistencia: llevará a la base de datos de un estado válido a otro válido.
* Aislamiento: Cada transacción debe ejecutarse en aislamiento total. Por ejemplo, si T1 y T2 se ejecutan concurrentemente, cada una deberá mantenerse independiente.
* Durabilidad:  La propiedad de durabilidad significa que una vez que se confirmó una transacción (commit), quedará persistida incluso ante eventos como pérdida de alimentación eléctrica, errores y caídas del sistema.
