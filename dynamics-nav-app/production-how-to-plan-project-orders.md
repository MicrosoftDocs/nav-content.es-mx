---
title: "Procedimiento: Planifique las órdenes de proyecto"
description: "Esta tarea de planificación se inicia desde un pedido de venta y utiliza la ventana **Planificación pedido venta**. Una vez creada la orden de producción de un proyecto, puede seguir planificándola en la ventana **Planificación de pedidos**."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: a03cdaf16b25cbcf030e9a33c538ea3df96a1fe9
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-project-orders"></a>Procedimiento: Planifique las órdenes de proyecto
Esta tarea de planificación se inicia desde un pedido de venta y para realizarla se utiliza la ventana **Planificación pedido venta**. Una vez creada la orden de producción de un proyecto, puede seguir planificándola en la ventana **Planificación de pedidos**.  

## <a name="to-create-a-project-production-order"></a>Para crear una orden de producción de un proyecto  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione el pedido de venta que representa el proyecto de producción y después seleccione la acción **Planificación**.  
4.  En la ventana **Planificación de pedido de venta**, seleccione la acción **Crear orden de producción**.  
5.  En la ventana **Crear pedido a partir de las ventas**, en el campo **Tipo orden**, seleccione **Orden proyecto**.  
6.  Elija el botón **Sí**.  
7.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Órdenes de producción** y, a continuación, seleccione el vínculo relacionado.
8. Abra la orden de producción que acaba de crear.  

    Tenga en cuenta que el campo **Tipo de procedencia** de la orden de producción contiene **Cabecera de ventas** y la orden tiene varias líneas, una para cada producto de línea de venta que debe fabricarse.  
9. Seleccione la acción **Planificación**.
10. En la ventana **Planificación de pedidos**, seleccione la acción **Actualizar** para calcular una nueva demanda.  

Se mostrará la línea de cabecera de la orden del proyecto con todas las líneas de demanda no satisfecha expandidas bajo ella. Aunque la orden de producción contiene líneas para varios productos fabricados, la demanda total de todas las líneas de la orden de producción aparece bajo una línea de cabecera de la orden en la ventana **Programación de pedidos** y se muestra el nombre del cliente original. Ahora puede empezar a planificar la demanda, según se indica en [Planificación de una nueva demanda pedido por pedido](production-how-to-plan-for-new-demand.md).  

> [!NOTE]  
>  Las líneas de demanda en el orden de producción del proyecto que disponen de **Prod. Pedido** en el campo de **Sistema reposición** representan las órdenes de producción subyacentes. Después de generar estas órdenes de producción, deberá volver a calcular un plan en la ventana **Programación de pedidos** para identificar la demanda de componentes no satisfecha. En ese caso, estas líneas se muestran como líneas de demanda bajo una línea de cabecera de orden de producción normal, es decir, la relación del proyecto ya no se muestra en la ventana. Sin embargo, si utiliza la función Seguimiento pedido, puede retroceder y avanzar por todos los pedidos de suministro creados bajo el pedido de venta original.  

## <a name="see-also"></a>Consulte también
[Planificación](production-planning.md)   
[Configuración de fabricación](production-configure-production-processes.md)  
[Fabricación](production-manage-manufacturing.md)    
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)   
[Procedimientos recomendados de configuración: planificación de suministros](setup-best-practices-supply-planning.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

