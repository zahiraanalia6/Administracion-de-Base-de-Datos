# Semana 3

**Modelo entidad - relacion**

Es una herramienta para el modelo de datos, la cual facilita la representación de entidades de una base de datos.

* Se elabora el diagrama (o diagramas) entidad-relación.
* Se completa el modelo con listas de atributos y una descripción de otras restricciones que no se pueden reflejar en el diagrama.

***

*Base teorica y conceptual*

El modelo de datos entidad-relación está basado en una percepción del mundo real que consta de una colección de objetos básicos, llamados entidades, y de relaciones entre esos objetos amorfos.

*Entidad*
Representa una “cosa”, "objeto", o "concepto" del mundo real con existencia independiente, es decir, se diferencia únicamente de otro objeto o cosa, incluso siendo del mismo tipo, o una misma entidad.

Ejemplos: una persona, un automovil, una casa.

Las entidades fuertes son las que no dependen de otras entidades para existir. 

Las entidades débiles siempre dependen de otra entidad, no tienen sentido por ellas mismas.


![18](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/18.png "18")

*Atributos*

Los atributos son las características que definen o identifican a una entidad. Éstas pueden ser muchas, y el diseñador sólo utiliza o implementa las que considere más relevantes.

En un conjunto de entidades del mismo tipo, cada entidad tiene valores específicos asignados para cada uno de sus atributos, de esta forma, es posible su identificación unívoca.

Ejemplos: 

A la colección de entidades «alumnos», con el siguiente conjunto de atributos en común, (id, nombre, edad, semestre), pertenecen las entidades:

* (1, Sophia, 15 años, 2)
* (2, Josefa, 19 años, 1)
* (3, Carlos, 20 años, 2)


***

Otra característica es el grado de relación:

* Grado 1: relaciones que solo relacionan una entidad consigo misma. 
* Grado 2: son relaciones que asocian dos entidades distintas.
* Grado n: se trata de relaciones que unen más de dos entidades distintas.

![19](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/19.png "19")

***
Recordar los elementos en un diagrama de entidad - relacion:

![20](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/20.png "20")

***

La relación se representa mediante una tabla

Esta tabla representa a lo que en el modelo entidad-relación llamábamos entidad y contiene los atributos (columnas) y las tuplas (filas). 


* Atributo: se trata de cada una de las columnas de la tabla. Vienen definidas por un nombre y pueden contener un conjunto de valores.

* Tupla: se trata de cada una de las filas de la tabla. Es importante señalar que no se pueden tener tuplas duplicadas en una tabla. Las relaciones se representan gráficamente con rombos, dentro de ellas se coloca el nombre de la relación.

***
Propiedades de la relacion:
* grado
* conectividad
* condicionalidad

**Grado**

* Unario: en donde una sola entidad forma parte de la relación.
* Binario: dos entidades forman parte de la relación.
* Ternario: tres entidades forman parte de la relación.

**Conectividad**

* uno a uno: 1:1
* uno a varios: 1:N
* varios a uno: N:1
* varios a varios: N:M

**Condicionalidad**

* Con la propiedad condicionalidad estamos indicando si la relación entre las entidades es obligatoria u opcional, lo que significa determinar si existen o no instancias de ambas entidades que forman parte de la relación.

* Supongamos el siguiente ejemplo: Las entidades son profesor y materia la relación es directa, en la cual una materia puede no tener asignado ningún profesor y un profesor puede dictar varias materias. 

***

Que es la normalizacion?

Lo importante en el uso y manejo de una base de datos es evitar la redundancia de datos y garantizar el fácil acceso a los mismos.

La normalización es un mecanismo que permite que un conjunto de tablas cumpla una serie de propiedades que eviten:

* Redundancia de datos

* Anomalías de actualización

* Pérdidas de Integridad de datos

El objetivo de la normalización es construir una BD que minimice la redundancia de información; para ello es necesario reagrupar los atributos de cada tabla del modelo.

***

*Primera forma normal* 

Para decir que una relación está en 1°FN se deben cumplir las siguientes condiciones:

*Debe existir una clave principal (primaria).

* Todos los dominios simples contienen valores atómicos.


*Segunda forma normal* 

Para decir que una relación está en 2°FN se deben cumplir las siguientes condiciones:

* Debe estar en 1°FN.

* Todos los atributos no clave dependen funcionalmente de la clave primaria.

*Tercera forma normal*

Una tabla está en tercera forma normal (3FN) si, y solo si, está en 2FN y, además, cada atributo que no forma parte de la clave primaria no depende transitivamente de la clave.

