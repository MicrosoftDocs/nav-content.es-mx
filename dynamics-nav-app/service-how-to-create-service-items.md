---
title: Crear productos de servicio
description: Cuando reciba un producto no registrado para servicio, puede registrarlo como un producto de servicio.
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0aa014ae2399e2eb23d9337797b09d45824db877
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-service-items"></a>Cómo crear productos de servicio
En [!INCLUDE[d365fin](includes/d365fin_md.md)], el término “producto de servicio” se refiere el equipo o productos que requieren servicio. Al crear un pedido de servicio, se especifican los productos que necesitan servicio. En el pedido, puede vincular un producto de servicio a un producto en existencias o un grupo de productos de servicio.    

Cuando reciba un producto que necesita servicio, puede registrarlo como un producto de servicio. Existen varias formas de hacerlo. Por ejemplo, puede crear un producto de servicio en la página **Productos de servicio**, o como parte de otro proceso, por ejemplo al trabajar con un pedido de servicio.   

## <a name="to-create-a-service-item"></a>Para crear un producto de servicio  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos servicio** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-create-service-items-within-a-service-order"></a>Para crear productos de servicio en un pedido de servicio  
Cuando se reciben productos para servicio que desea registrar como productos de servicio, puede crearlos como productos de servicio en las ventanas **Pedido servicio** o **Cotización servicio**.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Elija la acción **Crear producto de servicio**.  

    Se asignará un número al artículo de servicio y se creará una ficha de artículo de servicio. El campo **Nº producto servicio** se rellenará con el número del nuevo producto de servicio.

## <a name="to-create-a-service-item-when-shipping-items"></a>Para crear un producto de servicio al enviar productos  
Cuando se envían los artículos al registrar los pedidos o las facturas de servicio, los artículos enviados se registran automáticamente como artículos de servicio cuando se cumple la condición siguiente. Los artículos deben pertenecer a un grupo de artículo de servicio con la casilla **Crear prod. servicio** activada. Si los artículos tienen números de serie registrados en la ventana de líneas de seguimiento, esta información se copiará automáticamente al campo **Nº serie** en la ficha de artículo de servicio al crear artículos de servicio.  

El siguiente procedimiento muestra cómo crear productos de servicio al enviar productos de pedidos de servicio.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el pedido servicio que corresponda.  
3. Seleccione la acción **Registrar** o **Registrar e imprimir**.  
4. Seleccione la acción **Enviar** o **Enviar y facturar**.  
5. Se crearán automáticamente productos de servicio para los productos del pedido, siempre que pertenezcan a un grupo de productos de servicio que se ha configurado para crear productos de servicio. Si ha registrado números de serie específicos en la ventana **Líneas de seguimiento de producto**, éstos se asignarán a los productos de servicio.  

> [!NOTE]  
>  Si un producto es una L.M. y la ha desplegado, los productos de la L.M. desplegada se procesarán de la misma forma que los productos comunes. Los productos de servicio se crean en base a la condición del grupo de productos de servicio y, de manera opcional, en la condición de los números de serie. Además, si se crea un producto de servicio para un producto de la L.M. desplegada compuesto por otros componentes de la L.M., estos productos se crearán como componentes de un producto de servicio para el producto de servicio de la L.M. desplegada.  
>   
>  Si un producto es una L.M. y no ha desplegado la L.M., se crea un producto de servicio para aquel basándose en la condición del grupo de productos de servicio y, de manera opcional, en la condición de los números de serie.  

## <a name="to-insert-a-starting-fee-for-a-service-item"></a>Para insertar un gasto de inicio para un producto de servicio
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Tareas de servicio** y, a continuación, seleccione el vínculo relacionado.
2. Elija la acción **Hoja de producto**.
3. Seleccione la línea de servicio y, a continuación elija **Acciones**, seleccione **Funciones** y luego la acción **Insertar cuota inicial**.  

    Se insertará una línea de servicio del tipo **Costo** con el gasto de inicio. El gasto de inicio se aplica al producto de servicio seleccionado.

## <a name="see-also"></a>Consulte también  
[Cómo configurar componentes de servicio y de productos](service-how-setup-service-items.md)  
[Configurar la gestión de servicios](service-setup-service.md)  
[Gestión de servicios](service-service.md)  

