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

## Especificación de CU:

<div align="center">
  <img src="https://www.emprenderalia.com/wp-content/uploads/Crear-una-tienda-online-en-10-pasos-3-meses-y-sin-inversion.jpg" width="300px" />
</div>

## Índice
  - [Introducción](#introducción).
  - [Descripción](#descripción).
  - [Especificación de actores](#especificación-de-actores).
  - [Especificación de casos de uso](#especificación-de-casos-de-uso-1).

### Introducción

El presente documento especifica el __diagrama de CU__ de una aplicación cuya función es la de gestionar las cuentas de los clientes que realizan pedidos de productos del negocio Este documento trata a grandes rasgos, los casos de uso identificados, así como los actores que intervienen en ellos.

### Descripción

Una empresa plantea un sistema para gestionar las cuentas de los clientes que realizan pedidos de productos del negocio.. Para ello, se han especificado una serie de requisitos descritos en el presente documento.

### Especificación de Actores

En el presente documento se realiza la especificación de los diferentes actores que intervienen en la solución propuesta.

#### Cliente

  | Actor | Cliente |
  |---|---|
  | Descripción  |  |
  | Características  | |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _25/01/2023_ |

#### Repartidor

  | Actor | Repartidor |
  |---|---|
  | Descripción  |  |
  | Características  | |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _25/01/2023_ |

#### Sistema

| Actor | Sistema |
  |---|---|
  | Descripción  |  |
  | Características  | |
  | Relaciones | _No tiene relaciones con otros actores_ |
  | Referencias | |   
  |  Notas |   |
  | Autor  | _Abián Castañeda Méndez_ |
  |Fecha | _25/01/2023_ |

### Especificación de Casos de uso
  
En el presente documento se realiza la especificación de los casos de uso que forman parte de la en la solución propuesta.

#### ?¿

|  Caso de Uso	CU.1 |  |
|---|---|
| Fuentes  | El caso de uso se sustenta en [este documento](https://github.com/jpexposito/ets/tree/main/diagramas-comportamiento/diagramas-cu/tareas/tarea6).|
| Actor  |   |
| Descripción |  |
| Flujo básico |  |
| Pre-condiciones |  |  
| Post-condiciones  | |  
|  Requerimientos |  |
|  Notas |  |
| Autor  | _Abián Castañeda Méndez_ |
|Fecha | _25/01/2023_ |
