---
title: "Detalles de diseño: Gestión de pedidos antes de la fecha de inicio de planificación"
description: "En este tema se describen las reglas que la planificación aplica a los pedidos en la zona congelada."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: planning, frozen, design serial, lot
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: be20503b92b92448eceb1f388649d9f4022836ca
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-dealing-with-orders-before-the-planning-starting-date"></a>Detalles de diseño: Gestión de pedidos antes de la fecha de inicio de planificación
Para evitar que un plan de suministro muestre sugerencias imposibles y, por tanto, de poca utilidad, el sistema de planificación considera el periodo hasta la fecha inicial como una zona congelada donde no hay nada planificado. La regla siguiente se aplica a la zona congelada:  
  
Toda la demanda y aprovisionamiento antes de la fecha de inicio del periodo de planificación se tendrá como parte del inventario o enviado.  
  
Por consiguiente, el sistema de planificación, salvo algunas excepciones, no sugerirá ningún cambio en los pedidos de aprovisionamiento en la zona congelada, y no se creará ni se guardará ningún vínculo de seguimiento de pedidos para ese periodo.  
  
Las excepciones a esta regla son las siguientes:  
  
* Si las existencias disponibles proyectadas, incluida la suma de aprovisionamiento y la demanda en la zona congelada, es menor que cero.  
* Si hacen falta números de serie o lote en los pedidos con fecha anterior.  
* Si el conjunto de aprovisionamiento y demanda se vincula por una directiva de pedido a pedido.  
  
Si las existencias disponibles iniciales son menores que cero, el sistema de planificación sugiere un pedido de aprovisionamiento de emergencia el día antes del periodo de planificación para cubrir la cantidad que falta. Por tanto, el inventario proyectado y disponible será siempre al menos cero cuando empiece la planificación para el periodo futuro. La línea de planificación de este pedido de suministro mostrará un icono de advertencia de emergencia y, tras la búsqueda, se proporciona información adicional.  
  
## <a name="seriallot-numbers-and-order-to-order-links-are-exempt-from-the-frozen-zone"></a>Los números de serie y de lote y las conexiones de pedido contra pedido están exentos de la zona congelada  
Si se requieren números de serie y de lote o si hay un vínculo de pedido a pedido, el sistema de planificación no tendrá en cuenta la zona congelada e incorporará estas cantidades con fecha anterior a partir de la fecha de inicio y potencialmente propondrá acciones correctivas si la demanda y el aprovisionamiento no están sincronizados. El motivo empresarial de este principio es que dichos conjuntos de demanda-suministro específicos deben coincidir para garantizar que se cumple esta demanda específica.  
  
## <a name="see-also"></a>Consulte también  
[Detalles de diseño: Equilibrio de aprovisionamiento y demanda](design-details-balancing-demand-and-supply.md)   
[Detalles de diseño: Conceptos centrales del sistema de planificación](design-details-central-concepts-of-the-planning-system.md)   
[Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)
