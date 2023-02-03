<div align="justify">

# Gestión Centro Profesores. 

<div align="center">
  <img src="https://www.magisnet.com/wp-content/uploads/2020/02/clima-escolar.jpeg" width="600px" />
</div>

Se desea desarrollar una aplicación de gestión de las calificaciones de los alumnos
para satisfacer las numerosas quejas de los profesores, por el uso del lápiz y papel.
La aplicación debe de cumplir los temas que se describen a continuación:
El profesor recibe las actas en blanco de las asignaturas de las que es responsable, en formato electrónico. El acta contiene los siguientes datos de la asignatura (titulación,campus, curso académico, denominación de la asignatura, convocatoria y grupo) y la lista de alumnos matriculados (niu, nif, nombre y apellidos). Alguna de las acciones que puede hacer el profesor son:
 - Completar un acta con las notas de los alumnos.
 - Añadir o borrar un alumno de un acta.
 - Integrar las actas de varios grupos de una misma asignatura en una sola acta.
 - Otras de las opciones que se le exige a la aplicación, para satisfacer completamente las necesidades del profesor, son las siguientes:
    - Permitir la consulta de la siguiente información de cualquier alumno seleccionado _DNI, N.° EXPEDIENTE, Lista de asignaturas en las que está matriculado el alumno (Código asignatura-Nombre asignatura)_.
    - Obtener una estadística de las calificaciones obtenidas por los alumnos en un determinado grupo de una asignatura. En esta estadística se tendrá para cada posible calificación:
    - Número de personas con esa calificación, Porcentaje sobre los presentados, Porcentaje sobre el total del grupo.
    - Consultar el porcentaje de personas sobre el total del grupo que se han presentado y el de los que no se han presentado.
 - Poder visualizar un gráfico indicativo del número de personas que han obtenido una calificación entre 0-0.99, 1-1.99, 2-2.99, 3-3.99, 4-4.99, 5-5.99, 6-6.99, 8-8.99, 9-10; indicándose la nota media obtenida por la clase.
 - Disponer de una calculadora que permita realizar las operaciones de suma, resta, multiplicación, división. Esta calculadora se activará cuando se vayan a introducir las notas a algún alumno de forma que una vez realizada la operación aritmética, pulsando un botón se vuelque el resultado en la casilla donde se están introduciendo las calificaciones, redondeándose a dos cifras decimales.
 - Permitir la importación y exportación de la lista de alumnos con sus calificaciones a un formato compatible con MS Excel.
 - Imprimir las actas y la lista provisional de calificaciones.

Finalmente, como una ampliación extra, a la cual sólo podrá acceder quien se
identifique inicialmente como administrador de la aplicación, se deben permitir:
 - __CRUD__ _(Altas/Bajas/Modificación y Consulta)_ para cada uno de los siguientes grupos:.
   - __Asignaturas__, teniendo en cuenta que una asignatura sólo se puede dar en un único curso (primero, segundo, tercero...) y que cada curso está formado ponlos datos sobre el número máximo de alumnos, número mínimo de créditos troncales y número mínimo de créditos optativos. Algunos de los datos que vamos a poder consultar de una asignatura son el nombre, número de créditos y cuatrimestre en el que se imparte.
   - __Titulaciones__, teniendo en cuenta que una titulación sólo se da en un campus determinado y los datos que podemos consultar son el nombre, el número de créditos o carga lectiva global, si es de 1.° o 2.' ciclo, ...
   - __Grupos__, en los que podemos consultar el número máximo de alumnos permitidos, si es un grupo de mañana, de tarde o de noche, y cuál es el código empleado para identificar el grupo.
   - __Alumnos__:
     - Consultar aquellos alumnos que no se pueden matricular y el motivo de ello.
     - Consultar el historial académico de un alumno.

</div>

## Diagrama de CU 

<img src="img\Gestion_Centro_Profesores.png">

## Especificación de CU:

<div align="center">
  <img src="https://www.magisnet.com/wp-content/uploads/2020/02/clima-escolar.jpeg" width="600px" />
</div>

## Índice
  - [Introducción](#introducción).
  - [Descripción](#descripción).
  - [Especificación de actores](#especificación-de-actores).
  - [Especificación de casos de uso](#especificación-de-casos-de-uso).

### Introducción

El presente documento especifica el __diagrama de CU__ de una aplicación cuya función es la de gestionar las calificaciones de los alumnos. Este documento trata a grandes rasgos, los casos de uso identificados, así como los actores que intervienen en ellos.

### Descripción

Una centro escolar plantea desarrollar una aplicación para gestionar las calificaciones de los alumnos con el fin de satisfacer las numerosas quejas de los profesores, por el uso del lápiz y papel. Para ello, se han especificado una serie de requisitos descritos en el presente documento.

### Especificación de Actores

En el presente documento se realiza la especificación de los diferentes actores que intervienen en la solución propuesta.

#### Profesor

  | Actor | Profesor |
  |---|---|
  | Descripción  | El profesor recibe las actas en blanco de las asignaturas de las que es responsable, en formato electrónico. |
  | Características  | Debe pasar por una autenticación para realizar las acciones. |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | La información relacionada con el actor se encuentra en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7). |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _03/02/2023_ |
  
#### Administrador
  
  | Actor | Administrador |
  |---|---|
  | Descripción  | El profesor tedrá que identificarse como administrador para poder realizar funciones extras a las que ya podía realizar siendo profesor. |
  | Características  | Debe pasar por una autenticación para realizar las acciones. |
  | Relaciones | Se relaciona con el Profesor dado que puede realizar las mismas acciones que el anteriormente mencionado. |
  | Referencias | La información relacionada con el actor se encuentra en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7). |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _03/02/2023_ |

### Especificación de Casos de uso
  
En el presente documento se realiza la especificación de los casos de uso que forman parte de la en la solución propuesta.

#### Autenticarse

| Caso de Uso	CU.1 | Autenticarse |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor debe autenticarse antes de realizar alguna de sus funciones |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Poner notas

| Caso de Uso	CU.2 | Poner notas |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor completar un acta con las notas de los alumnos. |
| Flujo básico | Autenticarse --> Poner las notas en el acta |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Calculadora

| Caso de Uso	CU.3 | Calculadora |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor dispone de una calculadora que le permite realizar las operaciones de suma, resta, multiplicación, división. |
| Flujo básico | Autenticarse --> Poner las notas en el acta --> Accede a la calculadora |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Obtener Estadística

| Caso de Uso	CU.4 | Obtener Estadística |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor obtiene una estadística de las calificaciones obtenidas por los alumnos en un determinado grupo de una asignatura. |
| Flujo básico | Autenticarse --> Obtener estadística |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Consultar información

| Caso de Uso	CU.5 | Consultar información |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede consultar información sobre los alumnos |
| Flujo básico | Autenticarse --> Consultar información |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Gestionar alumno

| Caso de Uso	CU.6 | Gestionar alumno |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor dispone de una variedad de herramientas con las que gestionar al alumno |
| Flujo básico | Autenticarse --> Gestionar alumno |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Borrar

| Caso de Uso	CU.7 | Borrar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor borrar al alumno de un acta |
| Flujo básico | Autenticarse --> Gestionar alumno --> Borrar |
| Pre-condiciones |  |  
| Post-condiciones  | Se borra a un alumno de un acta |  
|  Requerimientos | Haberse autenticado y Gestionar el acta de un alumno |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Añadir

| Caso de Uso	CU.8 | Añadir |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor añade a un alumno a un acta |
| Flujo básico | Autenticarse --> Gestionar alumno --> Añadir |
| Pre-condiciones |  |  
| Post-condiciones  | Se añade al alumno a un acta |  
|  Requerimientos | Haberse autenticado y Gestionar el acta de un alumno |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Imprimir

| Caso de Uso	CU.9 | Imprimir |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede imprimir una gran variedad de datos |
| Flujo básico | Autenticarse --> Imprimir |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Actas

| Caso de Uso	CU.10 | Actas |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede imprimir las actas |
| Flujo básico | Autenticarse --> Imprimir --> Imprime las actas |
| Pre-condiciones |  |  
| Post-condiciones  | Se imprimen las actas |  
|  Requerimientos | Haberse autenticado e Imprimir |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Lista provisional

| Caso de Uso	CU.11 | Lista provisional |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede imprimir la lista provisional de calificaciones. |
| Flujo básico | Autenticarse --> Imprimir --> Imprime la lista provisional |
| Pre-condiciones |  |  
| Post-condiciones  | Se imprime la lista provisional de calificaciones |  
|  Requerimientos | Haberse autenticado e Imprimir |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Integrar

| Caso de Uso	CU.12 | Integrar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede integrar las actas de varios grupos de una misma asignatura en una sola acta. |
| Flujo básico | Autenticarse --> Integrar |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Grafico Indicativo

| Caso de Uso	CU.13 | Gráfico Indicativo |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede visualizar un gráfico indicativo del número de personas que han obtenido una calificación. |
| Flujo básico | Autenticarse --> Visualizar Gráfico |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Importación

| Caso de Uso	CU.14 | Importación |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede importar la lista de alumnos con sus calificaciones. |
| Flujo básico | Autenticarse --> Importar |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Exportación

| Caso de Uso	CU.15 | Exportación |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Profesor |
| Descripción | El profesor puede exportar la lista de alumnos con sus calificaciones. |
| Flujo básico | Autenticarse --> Exportar |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Autenticarse

| Caso de Uso	CU.16 | Autenticarse |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador debe autenticarse para realizar funciones extras a las que ya accede como profesor. |
| Flujo básico | |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | |
|  Notas | Aunque parezca que es la misma función que hace el profesor, a mi parecer el administrador debería volverse a autenticar para obtener permisos superiores a los que ya tiene como profesor. |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Gestión alumnos

| Caso de Uso	CU.17 | Gestión alumnos |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede consultar información que tiene que ver con los alumnos |
| Flujo básico | Autenticarse --> Gestionar alumnos |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado. |
|  Notas | Algunas de estas funciones que se pueden extender de este caso de uso ya las puede hacer el profesor pero hay otras dos que no dado que se deben obtener permisos de administrador para ello. |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Modificar 

| Caso de Uso	CU.18 | Modificar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede modificar la información del alumno |
| Flujo básico | Autenticarse --> Gestionar alumnos --> Modificar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y Gestionar alumno |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Consultar

| Caso de Uso	CU.19 | Consultar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede consultar información relacionada con el alumno |
| Flujo básico | Autenticarse --> Gestionar alumnos --> Consultar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Gestión Grupos

| Caso de Uso	CU.20 | Gestión Grupos |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar los grupos, en los que puede consultar el número máximo de alumnos permitidos, si es un grupo de mañana, de tarde o de noche, y cuál es el código empleado para identificar el grupo. |
| Flujo básico | Autenticarse --> Gestionar Grupos |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Alta

| Caso de Uso	CU.21 | Alta |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar las altas en lo referido al campo de "Grupos". |
| Flujo básico | Autenticarse --> Gestionar Grupos --> Alta |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Grupos. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Baja

| Caso de Uso	CU.22 | Baja |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar las bajas en lo referido al campo de "Grupos". |
| Flujo básico | Autenticarse --> Gestionar Grupos --> Baja |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Grupos. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Modificar 

| Caso de Uso	CU.23 | Modificar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede modificar la información en lo referido al campo de "Grupos". |
| Flujo básico | Autenticarse --> Gestionar Grupos --> Modificar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Grupos. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Consultar

| Caso de Uso	CU.24 | Consultar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede consultar toda la información en lo referido al campo de "Grupos". |
| Flujo básico | Autenticarse --> Gestionar alumnos --> Consultar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Grupos. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |


#### Gestión Asignaturas

| Caso de Uso	CU.25 | Gestión Asignaturas |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar el campo de "Asignaturas" |
| Flujo básico | Autenticarse --> Gestionar Asignaturas |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Alta

| Caso de Uso	CU.26 | Alta |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar las altas en lo referido al campo de "Asignaturas". |
| Flujo básico | Autenticarse --> Gestionar Asignaturas --> Alta |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Asignaturas. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Baja

| Caso de Uso	CU.27 | Baja |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar las bajas en lo referido al campo de "Asignaturas". |
| Flujo básico | Autenticarse --> Gestionar Asignaturas --> Baja |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Asignaturas. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Modificar 

| Caso de Uso	CU.28 | Modificar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede modificar la información en lo referido al campo de "Asignaturas". |
| Flujo básico | Autenticarse --> Gestionar Asignaturas --> Modificar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Asignaturas. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Consultar

| Caso de Uso	CU.29 | Consultar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede consultar toda la información en lo referido al campo de "Asignaturas". |
| Flujo básico | Autenticarse --> Gestionar Asignaturas --> Consultar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Asignaturas. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Gestión Titulaciones

| Caso de Uso	CU.30 | Gestión Titulaciones |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar el campo de "Titulaciones". |
| Flujo básico | Autenticarse --> Gestionar Titulaciones |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Alta

| Caso de Uso	CU.31 | Alta |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar las altas en lo referido al campo de "Titulaciones". |
| Flujo básico | Autenticarse --> Gestionar Titulaciones --> Alta |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Titulaciones. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Baja

| Caso de Uso	CU.32 | Baja |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede gestionar las bajas en lo referido al campo de "Titulaciones". |
| Flujo básico | Autenticarse --> Gestionar Titulaciones --> Baja |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Titulaciones. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Modificar 

| Caso de Uso	CU.33 | Modificar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede modificar la información en lo referido al campo de "Titulaciones". |
| Flujo básico | Autenticarse --> Gestionar Titulaciones --> Modificar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Titulaciones. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |

#### Consultar

| Caso de Uso	CU.34 | Consultar |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea7).|
| Actor  | Administrador |
| Descripción | El administrador puede consultar toda la información en lo referido al campo de "Titulaciones". |
| Flujo básico | Autenticarse --> Gestionar Titulaciones --> Consultar |
| Pre-condiciones | |  
| Post-condiciones  | |  
|  Requerimientos | Haberse autenticado y gestionar Titulaciones. |
|  Notas | |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _03/02/2023_ |
