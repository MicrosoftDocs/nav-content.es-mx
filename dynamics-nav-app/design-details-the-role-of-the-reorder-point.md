---
title: "Detalles de diseño: Función del punto de reorden"
description: "En este tema se destaca la importancia de establecer el punto de reorden, de forma que sepa cuándo solicitar más inventario."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: desigh, reorder, demand, supply
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8035a670077e53981e9c366d22bdb20df06d8c1b
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-the-role-of-the-reorder-point"></a>Detalles de diseño: Función del punto de reorden
Además del equilibrio general de la oferta y la demanda, el sistema de planificación debe supervisar los niveles de inventario para que los productos afectados respeten las políticas de reorden definidas.  
  
Un punto de reorden representa la demanda durante un plazo de entrega. Cuando el inventario proyectado está por debajo del nivel de inventario definido por el punto de reorden, ha llegado el momento de pedir más cantidad. Mientras tanto, se prevé que el inventario se reduzca gradualmente y posiblemente alcance cero (o el nivel de inventario de seguridad), hasta que llegue la reposición.  
  
Por consiguiente, el sistema de planificación sugerirá un pedido de suministros de programación anticipada en el momento en el que el inventario proyectado quede por debajo del punto de reorden.  
  
El punto de reorden refleja un determinado nivel de inventario. No obstante, los niveles de inventario pueden variar significativamente durante el ciclo y, por tanto, el sistema de planificación debe supervisar constantemente las existencias disponibles proyectadas.  
  
## <a name="see-also"></a>Consulte también  
[Detalles de diseño: Directivas de reorden](design-details-reordering-policies.md)   
[Detalles de diseño: Parámetros de la planificación](design-details-planning-parameters.md)   
[Detalles de diseño: Gestión de directivas de reorden](design-details-handling-reordering-policies.md)   
[Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)
