---
title: "Detalles de diseño: Redondeo"
description: Los redondeos residuales se pueden producir cuando se valora el costo de una salida de inventario que se mide en una cantidad distinta a la de la entrada de inventario correspondiente. Cuando se ejecuta el proceso **Valorar existencias - movs. producto**, se calculan los redondeos residuales para todas las valoraciones de existencias.
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
ms.openlocfilehash: 2a5187811051ee2bd32ec44b22876f0a468225e2
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-rounding"></a>Detalles de diseño: Redondeo
Los redondeos residuales se pueden producir cuando se valora el costo de una salida de inventario que se mide en una cantidad distinta a la de la entrada de inventario correspondiente. Cuando se ejecuta el proceso **Valorar existencias - movs. producto**, se calculan los redondeos residuales para todas las valoraciones de existencias.  

 Cuando se usa la valoración de existencias media, el redondeo residual se calcula y registra de forma acumulada y movimiento a movimiento.  

 Cuando se usa una valuación de inventarios distinta de Media, el redondeo residual se calcula cuando se ha aplicado completamente la entrada de inventario, lo que sucede cuando la cantidad restante de la entrada de inventario es igual a cero. A continuación se crea una entrada independiente para la redondeo residual, y la fecha de registro en esta entrada de redondeo es la fecha de registro de la entrada del último valor facturado de la entrada de existencias.  

## <a name="example"></a>Ejemplo  
 En el ejemplo siguiente se ilustra cómo se tratan diferentes redondeos residuales para la valoración de existencias Media y de otro tipo, respectivamente. En ambos casos, se ha ejecutado el proceso **Valorar existencias - movs. producto**.  

 En la tabla siguiente se muestran los movimientos de producto en los que se basa el ejemplo.  

|Fecha registro|Cantidad|Nº mov.|  
|------------------|--------------|---------------|  
|01-01-20|3|1|  
|01-02-20|-1|2|  
|01-03-20|-1|3|  
|01-04-20|-1|4|  

 Para un producto que emplee el método de coste Promedio, dicha residual de redondeo (1/300) se calcula con la primera disminución (movimiento número 2) y se transfiere al movimiento número 3.  Por tanto, el movimiento número 3 se valua en –3,34.  

 En la tabla siguiente se muestran los movimientos de valoración resultantes.  

|Fecha registro|Cantidad|Importe costo (Real)|Nº mov. producto|Nº mov.|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01-01-20|3|10|1|1|  
|01-02-20|-1|-3,33|2|2|  
|01-03-20|-1|-3,34|3|3|  
|01-04-20|-1|-3,33|4|4|  

 Para un producto que emplee un método de costo diferente al de Promedio, la residual de redondeo (0,01) se calcula cuando la cantidad pendiente para que la entrada de inventario sea cero. El redondeo residual tiene un movimiento independiente (número 5).  

 En la tabla siguiente se muestran los movimientos de valoración resultantes.  

|Fecha registro|Cantidad|Importe costo (Real)|Nº mov. producto|Nº mov.|  
|------------------|--------------|----------------------------|---------------------------|---------------|  
|01-01-20|3|10|1|1|  
|01-02-20|-1|-3,33|2|2|  
|01-03-20|-1|-3,33|3|3|  
|01-04-20|-1|-3,33|4|4|  
|01-01-20|0|-0,01|0|5|  

## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Costo de inventario](design-details-inventory-costing.md)   
 [Detalles de diseño: Ajuste de costo](design-details-cost-adjustment.md)   
 [Detalles de diseño: Valoraciones existencias](design-details-costing-methods.md) [Administración de costos de inventario](finance-manage-inventory-costs.md)  
 [Finanzas](finance.md)  
 [Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

