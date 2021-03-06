---
title: "Detalles de diseño: registros de seguimiento de productos históricos frente a activos"
description: "Cuando se registran partes de una cantidad de línea de documento, solo dicha cantidad concreta se transfiere a los movimientos de producto y sus números de seguimiento de producto. No obstante, le interesará acceder a toda la información de seguimiento del producto relevante directamente desde la línea activa del documento. Es decir, no solo desea ver los movimientos que están relacionados con la cantidad restantes, sino que también desea información sobre las unidades que se han registrado. Cuando consulte o modifique la ventana **Líns. seguim. prod.**, el contenido colectivo de las tablas **Especificación seguimiento** (T336) y **Mov. reserva** (T337) se presentan en una versión temporal de T336. De este modo se garantiza que se obtiene acceso a los datos de seguimiento de producto históricos y activos como una sola unidad."
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
ms.openlocfilehash: 315b5317c2ac3e2cd6a56bd243e30d4e3445a6ec
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-active-versus-historic-item-tracking-entries"></a>Detalles de diseño: registros de seguimiento de productos históricos frente a activos
Cuando se registran partes de una cantidad de línea de documento, solo dicha cantidad concreta se transfiere a los movimientos de producto y sus números de seguimiento de producto. No obstante, le interesará acceder a toda la información de seguimiento del producto relevante directamente desde la línea activa del documento. Es decir, no solo desea ver los movimientos que están relacionados con la cantidad restantes, sino que también desea información sobre las unidades que se han registrado. Cuando consulte o modifique la ventana **Líns. seguim. prod.**, el contenido colectivo de las tablas **Especificación seguimiento** (T336) y **Mov. reserva** (T337) se presentan en una versión temporal de T336. De este modo se garantiza que se obtiene acceso a los datos de seguimiento de producto históricos y activos como una sola unidad.  

 En la tabla siguiente se muestra cómo se usan T336 y T337 en un escenario de compra. Las cifras en negrita representan los valores que el usuario especifica manualmente en la ventana **Líns. seguim. prod.**  

 Paso 1: cree una línea de pedido de compra de siete piezas con los números de seguimiento de producto.  

||**Cantidad (base)**|**Cdad.a manipular**|**Cdad. a facturar (base)**|**Cdad. manipulada (Base)**|**Cdad. facturada (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|**T337**|7|0|0|0|0|  
|**T336**|0|0|0|0|0|  

 Paso 2: reciba cuatro piezas.  

||**Cantidad (base)**|**Cdad.a manipular**|**Cdad. a facturar (base)**|**Cdad. manipulada (Base)**|**Cdad. facturada (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Ventana **Líns. seguim. prod.**|7|**4**|**0**|0|0|  
|**T337**|3|0|0|0|0|  
|**T336**|4|0|0|4|0|  

 Paso 3: reciba dos piezas y facture dos piezas.  

||**Cantidad (base)**|**Cdad.a manipular**|**Cdad. a facturar (base)**|**Cdad. manipulada (Base)**|**Cdad. facturada (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Ventana **Líns. seguim. prod.**|7|**2**|**2**|4|0|  
|**T337**|0|0|0|0|0|  
|**T336**|6|0|0|6|2|  

 Paso 4: reciba una pieza.  

||**Cantidad (base)**|**Cdad.a manipular**|**Cdad. a facturar (base)**|**Cdad. manipulada (Base)**|**Cdad. facturada (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Ventana **Líns. seguim. prod.**|7|**1**|**0**|6|2|  
|**T336**|7|0|0|7|2|  

 Facturar 5 piezas.  

||**Cantidad (base)**|**Cdad.a manipular**|**Cdad. a facturar (base)**|**Cdad. manipulada (Base)**|**Cdad. facturada (Base)**|  
|-|----------------------------------------------|--------------------------------------------|------------------------------------------------------|-------------------------------------------------------|--------------------------------------------------------|  
|Ventana **Líns. seguim. prod.**|7|0|**5**|7|2|  
|**T336**|7|0|0|7|7|  

## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Seguimiento de productos](design-details-item-tracking.md)   
 [Detalles de diseño: Ventana de líneas de seguimiento de productos](design-details-item-tracking-lines-window.md)

