---
title: Planificar los picking en la hoja de trabajo
description: "Si el almacén está configurado para requerir los procesos de picking y envío, el almacén puede trabajar de forma que las líneas de los documentos de envío no se transformen automáticamente en instrucciones de picking, si no hacerlas disponibles en vez de llevarlas a la hoja de trabajo de picking."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 9483eda38a9db7cd50d7167b45d0c6b6d21ace8c
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-picks-in-worksheets"></a>Cómo planificar los picking en la hoja de trabajo
Si el almacén está configurado para requerir los procesos de picking y envío, el almacén puede trabajar de forma que las líneas de los documentos de envío no se transformen automáticamente en instrucciones de picking, si no hacerlas disponibles en vez de llevarlas a la hoja de trabajo de picking.  

> [!NOTE]  
>  Si ya se han creado las instrucciones de picking de almacén y desea combinarlas en una instrucción de picking más eficaz debe eliminar los picking de almacén individuales. Las líneas de las que se va a realizar el picking se pueden listar en la hoja de trabajo.  

En la hoja de trabajo de picking, puede configurar listas de picking para empleados que minimicen el tiempo que el empleado tarda en mover los productos de picking de almacén. Hay campos que contienen información acerca de las cantidades de productos disponibles en las ubicaciones de tránsito directo. Esto es útil en situaciones de tránsito directo para planificar las tareas de trabajo, ya que el programa siempre sugerirá un picking de una ubicación de tránsito directo antes de cualquier otra ubicación, independientemente de la unidad de medida. Las líneas de la hoja de trabajo pueden proceder de varios documentos de origen y estar ordenadas por producto, número de estante, documento de origen, fecha de vencimiento o dirección de envío.  

Si ordena por fecha de vencimiento, puede eliminar de la hoja de trabajo todas las líneas excepto las que necesiten atención inmediata. Las líneas menos urgentes no se eliminan, sólo se devuelven a la hoja de trabajo de **Selección de picking**. Al crear el picking, las líneas ya se han ordenado por fecha de vencimiento y puede elegir asignar el picking a un empleado determinado.  

> [!NOTE]  
>  Picking en el envío de almacén de los productos que se ensamblan al pedido de venta que se envía sigue los mismos pasos que para picking de almacén normales para envío, tal como se describe en este tema. Sin embargo, el número de líneas de picking por la cantidad a enviar puede ser de "muchas a una" porque realiza el picking de los componentes, no el producto de ensamblado.  
>   
>  Las líneas de picking de almacén se crean para el valor del campo **Cantidad pendiente** en las líneas de pedido de ensamblado vinculado a la línea de pedido de venta que se envía. Esto garantiza que se realice el picking de todos los componentes en una acción.  
>   
>  Para obtener más información, consulte "Tratamiento de productos ensamblar para pedido en los envíos de almacén" en Envíos de almacén.  
>   
>  Para obtener información acerca de la realización de picking de componentes para pedidos de ensamblado en general, incluidas las situaciones en las que no caduca el producto de ensamblado en una remisión de venta, consulte [Procedimiento: Picking para ensamblado o producción en configuraciones avanzadas de almacén](warehouse-how-to-pick-for-internal-operations-in-advanced-warehousing.md).  

## <a name="to-plan-picks-in-the-worksheet"></a>Para planificar los picking en la hoja de trabajo  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja trabajo picking** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Tomar documentos almacén**.  
3.  Introduzca el envío para el que desea preparar el picking. Ahora puede ordenar las líneas, pero el método ordenación que ejecute no se aplicará a la instrucción de picking. También puede eliminar algunas líneas para realizar un picking más eficaz. Por ejemplo, si hay varias líneas con productos en ubicaciones de tránsito directo, es posible que desee realizar un picking de todas las líneas asociadas con estas líneas. Se enviarán los productos de tránsito directo junto con el resto de los productos de los envíos, y las ubicaciones de tránsito directo tendrán espacio para la entrada de más productos.  
4.  Elija la acción **Crear picking** y rellene la ventana de solicitud **Crear picking**. El método de ordenación que ha solicitado ordenará las líneas de picking que cree. Por ejemplo, puede crear un picking para cada zona y ordenar las líneas por ranking de ubicación en cada picking.  
5.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Picking** y, a continuación, seleccione el vínculo relacionado. Se abre la ventana **Picking**.  
6.  Ahora puede encontrar la asignación de picking que acaba de crear seleccionando el picking con el número más alto.  
7.  En el picking, aún puede modificar el Id. de usuario asignado y el orden de las líneas.  
8.  Elija la acción **Imprimir** para que se impriman las instrucciones de picking.  
9. Una vez haya realizado el picking, elija la acción **Registrar**.  

Si las ubicaciones se han numerado de forma que reflejen el diseño físico del almacén, las líneas ordenadas por código de ubicación permitirán al encargado realizar el picking de los envíos en una sola vez. El encargado obtiene los productos necesarios para cada línea de envío de cada ubicación y los coloca junto con el resto de los productos para el envío determinado. Un encargado de picking puede ahorrar mucho tiempo realizando el picking de varios envíos en una sola visita a una ubicación.  

Otra opción de ordenación eficaz es el ranking de ubicación, si el diseño físico del almacén está más adaptado al ranking de ubicación en vez de al código de ubicación.  

En la hoja de trabajo de picking, también puede ordenar por dirección de envío, lo que le permite agrupar y enviar los pedidos a los clientes más alejados primero.  

## <a name="see-also"></a>Consulte también
[Gestión almacén](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

