---
title: "Detalles de diseño: Cantidad de reorden fija"
description: "La directiva Cdad. fija reorden está relacionada con la planificación de inventario de los productos C típicos (costo de inventario bajo, poco riesgo de obsolescencia o muchos productos). Normalmente, esta directiva se usa con relación a un punto de reorden que refleja la demanda anticipada durante el plazo del producto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6249f51415f46443eb0b528161da290aac25d202
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-fixed-reorder-qty"></a>Detalles de diseño: Cantidad de reorden fija
La directiva Cdad. fija reorden está relacionada con la planificación de inventario de los productos C típicos (costo de inventario bajo, poco riesgo de obsolescencia o muchos productos). Normalmente, esta directiva se usa con relación a un punto de reorden que refleja la demanda anticipada durante el plazo del producto.  

## <a name="calculated-per-time-bucket"></a>Calculado por ciclo  
 Si el sistema de planificación detecta que se ha alcanzado o superado el punto de pedido en un ciclo determinado (ciclo reorden), por encima del punto de pedido al inicio del periodo o en ese mismo punto, o por debajo al final del periodo o en ese mismo punto, sugerirá crear un nuevo pedido de aprovisionamiento con la cantidad de reorden especificada y anticipará su programación a partir de la primera fecha después de final del ciclo.  

 El concepto de punto de reorden por ciclos reduce el número de sugerencias de suministro. Esto refleja el proceso manual de recorrer con frecuencia el almacén para comprobar el contenido real de varias ubicaciones.  

## <a name="creates-only-necessary-supply"></a>Crea solo el aprovisionamiento necesario  
 Antes de proponer nuevos pedidos de aprovisionamiento para satisfacer un punto de reorden, el sistema de planificación comprueba si el aprovisionamiento se ha pedido ya para ser recibido en el plazo de entrega del producto. Si un pedido de aprovisionamiento existente puede solucionar el problema llevando el inventario proyectado hasta el punto de reorden o por encima dentro del plazo de entrega, el sistema no sugerirá un nuevo pedido de aprovisionamiento.  

 Los pedidos de suministro que se crean específicamente para satisfacer un punto de reorden se excluyen del equilibrado de suministro normal y no cambiarán posteriormente. Por tanto, si un producto con punto de reorden debe retirarse (no reponerse), es recomendable revisar los pedidos de aprovisionamiento pendientes manualmente o cambiar la directiva de reorden a lote por lote, de modo que el sistema reduzca o cancele los aprovisionamientos superfluos.  

## <a name="combines-with-order-modifiers"></a>Combina con modificadores de pedido  
 Los modificadores de pedido, Cantidad mínima pedido, Cantidad máxima pedido y Múltiplos de pedido, no deben desempeñar un rol amplio cuando se usa la directiva cantidad de pedido fija. No obstante, el sistema de planificación aún tiene en cuenta estos modificadores y disminuye la cantidad a la cantidad de pedido máxima especificada (y crea dos o más aprovisionamientos para alcanzar la cantidad total de pedido), aumenta el pedido a la cantidad de pedido mínima especificada, o la redondea para que llegue al múltiplo del pedido especificado.  

## <a name="combines-with-calendars"></a>Combina con Calendarios  
 Antes de proponer nueva órdenes de suministro para satisfacer un punto de reorden, el sistema de planificación comprueba si el pedido está programado para un día no laborable, según los calendarios definidos en el campo **Código calendario base** en las ventanas **Información empresa** y **Ficha almacén**.  

 Si la fecha programada es un día no laborable, el sistema de planificación mueve el pedido al próximo día laborable. Esto puede dar lugar a un pedido que cumpla con el punto de reorden pero que no cumpla una demanda específica. Para este tipo de demandas sin saldar, el sistema de planificación crea un suministro extra.  

## <a name="should-not-be-used-with-forecast"></a>No debe usarse con la previsión  
 Dado que la demanda prevista aparece expresada ya en el nivel del punto de reorden, no es necesario incluir una previsión en la planificación de un producto mediante un punto de reorden. Si es necesario basar el plan en una previsión, utilice la directiva de lote por lote.  

## <a name="must-not-be-used-with-reservations"></a>No se debe usar con reservas  
 Si el usuario ha reservado una cantidad, por ejemplo una cantidad en inventario, en algunas demandas lejanas se perturbará la base de la planificación. Aunque el nivel de inventario estimado es aceptable en relación con el punto de reorden, las cantidades pueden no estar disponibles. El programa puede intentar compensarlo mediante la creación de pedidos de excepción; no obstante, se recomienda que el campo Reservar está configurado como Nunca en los productos que están planificados con un punto de reorden.  

## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Directivas de reorden](design-details-reordering-policies.md)   
 [Detalles de diseño: Cantidad máxima](design-details-maximum-qty.md)   
 [Detalles de diseño: Parámetros de la planificación](design-details-planning-parameters.md)   
 [Detalles de diseño: Gestión de directivas de reorden](design-details-handling-reordering-policies.md)   
 [Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)

