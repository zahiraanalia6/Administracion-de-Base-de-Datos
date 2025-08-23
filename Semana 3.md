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

**Correspondencia de cardinalidades**

Los cardinales pueden ser:

* uno a uno: 1:1
* uno a varios: 1:N
* varios a uno: N:1
* varios a varios: N:M

***

Otra característica es el grado de relación:

* Grado 1: relaciones que solo relacionan una entidad consigo misma. 
* Grado 2: son relaciones que asocian dos entidades distintas.
* Grado n: se trata de relaciones que unen más de dos entidades distintas.

![19](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/19.png "19")

***
Recordar los elementos en un diagrama de entidad - relacion:

![20](https://github.com/zahiraanalia6/Administracion-de-Base-de-Datos/blob/main/img/20.png "20")

