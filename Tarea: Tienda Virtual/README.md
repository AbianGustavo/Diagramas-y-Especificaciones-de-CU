<div align="justify">

# Tienda Virtual. 

<div align="center">
  <img src="https://www.emprenderalia.com/wp-content/uploads/Crear-una-tienda-online-en-10-pasos-3-meses-y-sin-inversion.jpg" width="300px" />
</div>

El sistema tendrá que gestionar las cuentas de los clientes que realizan pedidos de productos del negocio. Cada producto tiene un stock determinado. Generalmente un cliente tiene una o varias cuentas para pagar los pedidos y cada cuenta tiene asociada una tarjeta de crédito con una cantidad disponible de dinero. Esa cantidad puede aumentarse por parte del cliente para poder realizar más pedidos.

Los clientes que quieran realizar un pedido tendrán que tener alguna cuenta con saldo disponible.

Los pedidos pueden ser simples o compuestos. Un pedido simple solamente tendrá una cuenta de pago y como mucho tendrá 20 productos. 

Un pedido compuesto puede tener dos o más pedidos (simples o compuestos). Obviamente un pedido compuesto se tiene que pagar con la cuenta de un mismo cliente.

Solamente se pueden pedir productos que estén en stock.

Los cobros se hacen diariamente a las 23:59 horas. En ese procedimiento de cobro se comprueban todos los pedidos pendientes de cobro y se cobran de las cuentas de los clientes. Si una cuenta de cliente __NO__ tiene dinero suficiente se __RECHAZA__ el pedido (tanto si es simple como si forma parte de un pedido compuesto).

Una vez superado este proceso se genera la orden de distribución y confirma los pedidos.

Los pedidos listos de reparto se entregan y una vez entregados su estado pasa a estar confirmado.

> _Nota_. Un cliente puede o no estar registrado previamente, con lo cual la realización de pedidos __supone realizar un registro, para más tarde autenticarse__.

Realiza:
- Identifica los actores.
- Identifica los __CU__ de cada uno de los actores.
- Realiza el diagrama de CU.
- La especificación de CU.

## Diagrama de CU 

<img src="img\Tienda_Virtual.png">

## Especificación de CU:

<div align="center">
  <img src="https://www.emprenderalia.com/wp-content/uploads/Crear-una-tienda-online-en-10-pasos-3-meses-y-sin-inversion.jpg" width="300px" />
</div>

## Índice
  - [Introducción](#introducción).
  - [Descripción](#descripción).
  - [Especificación de actores](#especificación-de-actores).
  - [Especificación de casos de uso](#especificación-de-casos-de-uso).

### Introducción

El presente documento especifica el __diagrama de CU__ de una aplicación cuya función es la de gestionar las cuentas de los clientes que realizan pedidos de productos del negocio Este documento trata a grandes rasgos, los casos de uso identificados, así como los actores que intervienen en ellos.

### Descripción

Una empresa plantea un sistema para gestionar las cuentas de los clientes que realizan pedidos de productos del negocio.. Para ello, se han especificado una serie de requisitos descritos en el presente documento.

### Especificación de Actores

En el presente documento se realiza la especificación de los diferentes actores que intervienen en la solución propuesta.

#### Cliente

  | Actor | Cliente |
  |---|---|
  | Descripción  | Persona que va a realizar pedidos en el sistema |
  | Características  | |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | **Asociar una tarjeta**, **Establecer un limite**, **Hacer Pedidos**, **Autenticarse**, **Mostrar productos**, **Disponer de Saldo**, **Registrarse**, **Verificar Stock**. |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _25/01/2023_ |

#### Repartidor

  | Actor | Repartidor |
  |---|---|
  | Descripción  | Persona que entrega pedidos |
  | Características  | |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | **Entrega Pedido** |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _25/01/2023_ |

#### Sistema de Cobro

| Actor | Sistema de Cobro |
  |---|---|
  | Descripción  | Sistema encargado de comprobar pedidos |
  | Características  | |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | **Comprobar pedido**, **Confirmar Pedido** |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _25/01/2023_ |

### Especificación de Casos de uso
  
En el presente documento se realiza la especificación de los casos de uso que forman parte de la en la solución propuesta.

#### Asociar una tarjeta

| Caso de Uso	CU.1 | Asociar una tarjeta |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | El cliente puede asociar una tarjeta a su cuenta |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Establecer un límite

| Caso de Uso	CU.2 | Establecer un límite |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | El cliente puede aumentar o disminuir la cantidad de dinero de la tarjeta que ha asociado a su cuenta |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos | Disponer de una tarjeta de credito asociada a la cuenta |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Hacer pedidos

| Caso de Uso	CU.3 | Hacer pedidos |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | El cliente puede realizar pedidos acerca de los productos que vende la tienda |
| Flujo básico |  |
| Pre-condiciones | El cliente debe autenticarse y también debe disponer de saldo |  
| Post-condiciones  | Al hacer el pedido se le debe mostrar al cliente los productos y por ende si hay de estos en stock |  
|  Requerimientos | Sistema de autenticación y disponibilidad de saldo |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Autentificarse

| Caso de Uso	CU.4 | Autentificarse |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | A la hora de realizar un pedido el cliente debe autenticarse |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Mostrar productos

| Caso de Uso	CU.5 | Mostrar productos |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | Cuando un cliente va a realizar un pedido se deben mostrar los productos que puede pedir |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | Se deben mostrar aquellos productos que estén en stock |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Verificar Stock

| Caso de Uso	CU.6 | Verificar Stock |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | Se muestran aquellos productos que están en stock |
| Flujo básico |  |
| Pre-condiciones | Se debe hacer un pedido y también se deben mostrar los productos que el cliente deba pedir |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Disponer Saldo

| Caso de Uso	CU.7 | Disponer Saldo |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | Los clientes que quieran realizar un pedido tendrán que tener alguna cuenta con saldo disponible |
| Flujo básico |  |
| Pre-condiciones | Hacer un pedido y autenticarse |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Registrarse

| Caso de Uso	CU.8 | Registrarse |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Cliente |
| Descripción | Un cliente puede o no estar registrado previamente pero a la hora de realizar un pedido si debe autenticarse |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Comprueba pedidos

| Caso de Uso	CU.9 | Comprueba pedidos |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Sistema de Cobro |
| Descripción | El sistema de cobro comprueba todos los pedidos pendientes de cobro |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | Se debe confirmar el pedido y más tarde verificar la disponibilidad de saldo |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Confirmación de pedido

| Caso de Uso	CU.10 | Confirmación de pedido |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Sistema de Cobro |
| Descripción | El sistema de cobro confirma un pedido pendiente de un cliente con el saldo necesario |
| Flujo básico | El sistema de cobro al comprobar un pedido pendiente, cobra de la cuenta de un cliente el saldo y una vez superado dicho proceso se confirma el pedido |
| Pre-condiciones | Comprobar un pedido pendiente |  
| Post-condiciones  | Disponibilidad de saldo |  
|  Requerimientos | Disponer de saldo |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |

#### Entrega Pedido

| Caso de Uso	CU.11 | Entrega Pedido |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  | Repartidor |
| Descripción | El repartidor se encarga de distribuir pedidos |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |
