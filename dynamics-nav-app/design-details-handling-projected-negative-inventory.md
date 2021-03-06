---
title: "Detalles de diseño: Gestión de inventario negativo proyectado"
description: "El punto de reorden expresa la demanda prevista durante el plazo del producto. Cuando se supera el punto de reorden, ha llegado el momento de pedir más. Pero el inventario proyectado debe ser lo suficientemente grande como para satisfacer la demanda hasta que se reciba el nuevo pedido. Mientras tanto, el stock de seguridad debe satisfacer las fluctuaciones en la demanda hasta un nivel de servicio objetivo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 66cf357ccd0489d789ec9c2036734ec9f04aad95
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-handling-projected-negative-inventory"></a>Detalles de diseño: Gestión de inventario negativo proyectado
El punto de reorden expresa la demanda prevista durante el plazo del producto. Cuando se supera el punto de reorden, ha llegado el momento de pedir más. Pero el inventario proyectado debe ser lo suficientemente grande como para satisfacer la demanda hasta que se reciba el nuevo pedido. Mientras tanto, el stock de seguridad debe satisfacer las fluctuaciones en la demanda hasta un nivel de servicio objetivo.  

 Por tanto, el sistema de planificación considera una emergencia el que una demanda futura no se pueda atender desde el inventario proyectado, o dicho de otro modo, que el inventario proyectado quede en negativo. El sistema se ocupa de dicha excepción mediante la sugerencia de un nuevo pedido de suministro para satisfacer la parte de la demanda que no se puede satisfacer mediante las existencias u otro suministro. El tamaño de pedido de reorden de suministro no tendrá en cuenta el inventario máximo o la cantidad de reorden Tampoco tendrá en cuenta los modificadores Cantidad máxima pedido, Cantidad mínima pedido y Múltiplos de pedido. En su lugar, reflejará la deficiencia exacta.  

 La línea de planificación para este tipo pedido de suministro mostrará un icono de advertencia de emergencia y, tras la búsqueda, se proporcionará información adicional para comunicar al usuario la situación.  

 En la ilustración siguiente, el aprovisionamiento D representa un pedido de emergencia que ajustar para inventario negativo.  

 ![](media/nav_app_supply_planning_2_negative_inventory.png "NAV_APP_supply_planning_2_negative_inventory")  

1.  El suministro **A**, inventario proyectado inicial, está por debajo del punto de reorden.  

2.  Se ha creado un nuevo aprovisionamiento programación de forma anticipada (**C**).  

     (Cantidad = Inventario máximo – Nivel de inventario proyectado)  

3.  El suministro **A** está cerrado por la demanda **B**, que no se cubre por completo.  

     (La demanda **B** podría intentar programar el aprovisionamiento C, pero esto no sucederá según el concepto de ciclo).  

4.  Se crea un nuevo suministro (**D**) para cubrir la cantidad restante de la demanda **B**.  

5.  La demanda **B** está cerrada (creando un aviso al inventario proyectado).  

6.  Se cierra el nuevo suministro **D**.  

7.  Se ha comprobado el inventario proyectado; no se ha superado el punto de reorden.  

8.  El suministro **C** está cerrado (no hay más demanda).  

9. Comprobación final: que no queden avisos pendientes en el nivel de inventario.  

> [!NOTE]  
>  El paso 4 refleja cómo reacciona el sistema en versiones anteriores a Microsoft Dynamics NAV 2009 SP1.  

 De este modo concluye la descripción de los principios básicos relacionados con la planificación de inventario basada en directivas de reorganización. En la sección siguiente se describen las características de las cuatro directivas de reorden admitidas.  

## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Directivas de reorden](design-details-reordering-policies.md)   
 [Detalles de diseño: Parámetros de la planificación](design-details-planning-parameters.md)   
 [Detalles de diseño: Gestión de directivas de reorden](design-details-handling-reordering-policies.md)   
 [Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)

