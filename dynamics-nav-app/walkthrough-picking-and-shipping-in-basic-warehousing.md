---
title: "Tutorial: picking y envío en la configuración del almacenamiento básico"
description: "En [!INCLUDE[d365fin](includes/d365fin_md.md)], los procesos de salida para el picking y el envío se pueden realizar de cuatro maneras utilizando distintas funciones según el nivel de complejidad del almacén."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: ce9d58f93edeebd4933a532deb7c4672ced6f76a
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-picking-and-shipping-in-basic-warehouse-configurations"></a>Tutorial: picking y envío en la configuración del almacenamiento básico
En [!INCLUDE[d365fin](includes/d365fin_md.md)], los procesos de salida para el picking y el envío se pueden realizar de cuatro maneras utilizando distintas funciones según el nivel de complejidad del almacén.  

|Método|Proceso de salida|Ubicaciones|Picking|Envíos|Nivel de complejidad (consulte [Detalles de diseño: configuración de almacén](design-details-warehouse-setup.md))|  
|------------|---------------------|----------|-----------|---------------|--------------------------------------------------------------------------------------------------------------------|  
|A|Registro de picking y envío desde la línea de pedido|X|||2|  
|P|Registro de picking y envío desde un documento de picking de inventario||X||3|  
|P|Registro de picking y envío desde un documento de envío de almacén|||X|5/4/6|  
|D|Registro de picking desde un documento de picking de almacén y registro de envío de un documento de envío de almacén||X|X|5/4/6|  

Para obtener más información, consulte [Detalles de diseño: Flujo de salida del almacén](design-details-outbound-warehouse-flow.md).  

En el siguiente tutorial se demuestra el método B de la tabla anterior.  

## <a name="about-this-walkthrough"></a>Acerca de este tutorial  
En la configuración del almacenamiento básico, donde el almacén está configurado para requerir proceso de picking, pero no de envío, utiliza la ventana **Picking inventario** para registrar la información de picking y envío de los documentos de origen salientes. El documento de origen de salida puede ser un pedido de venta, un pedido de devolución de compra, un pedido de transferencia de salida o una orden de producción con necesidad de componentes.  

En este tutorial, se demuestran las siguientes tareas:  

-   Configuración del almacén PLATA para el picking de inventario.  
-   Crear un pedido de venta para el cliente 10000 para 30 altavoces.  
-   Liberar el pedido de venta para la manipulación en almacén.  
-   Crear un picking de inventario basado en un documento de origen lanzado.  
-   Registrar el movimiento de almacén desde el almacén y, al mismo tiempo, registrar la remisión de venta para el pedido de venta de origen.  

## <a name="roles"></a>Acciones  
En este tutorial, se demuestran las tareas realizadas por los siguientes roles de usuario:  

-   Responsable de almacén  
-   Procesador de pedidos  
-   Trabajador de almacén  

## <a name="prerequisites"></a>Requisitos previos  
Para completar este tutorial, necesitará:  

-   CRONUS International Ltd. instalado.  
-   Para convertirse en un empleado de almacén en el almacén PLATA, realice los pasos siguientes:  

    1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Empleados almacén** y, a continuación, seleccione el vínculo relacionado.  
    2.  Elija el campo **Id. de usuario** y seleccione su propia cuenta de usuario en la ventana **Usuarios**.  
    3.  En el campo **Cód. almacén**, especifique PLATA.  
    4.  Seleccione el campo de **Predeterminado**.  

-   Haga que el producto LS-81 esté disponible en el almacén PLATA siguiendo estos pasos:  

    1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios producto** y, a continuación, seleccione el vínculo relacionado.  
    2.  Abra el diario predeterminado y después cree dos líneas del diario del producto con la siguiente información en la fecha de trabajo (23 de enero).  

        |Tipo mov.|Número de producto|Cód. almacén|Cód. ubicación|Cantidad|  
        |----------------|-----------------|-------------------|--------------|--------------|  
        |Entradas|LS-81|PLATA|S-01-0001 **Nota:** La ubicación predeterminada del producto en CRONUS|nº 20|  
        |Entradas|LS-81|PLATA|S-01-0002|nº 20|  

    3.  Elija la acción **Registrar** y, a continuación, seleccione el botón **Si**.  

## <a name="story"></a>Historia  
Ellen, la administradora del almacén en CRONUS, configura el almacén PLATA para la manipulación de picking básica donde los trabajadores de almacén procesan los pedidos de salida individualmente. Susana, la encargada de procesamiento de pedidos, crea un pedido de venta de 30 unidades del producto LS-81 que se deben enviar al cliente 10000 desde el almacén PLATA. Juan, el trabajador de almacén debe comprobar que el envío se prepara y envía al cliente. Juan controla todas las tareas relacionadas con la ventana **Picking inventario**, que señala automáticamente a las ubicaciones donde se almacena LS-81.  

## <a name="setting-up-the-location"></a>Configuración del almacén  
La configuración de la ventana **Ficha almacén** define los flujos de almacén de la empresa.  

### <a name="to-set-up-the-location"></a>Configurar el almacén  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Almacenes** y, a continuación, seleccione el vínculo relacionado.  
2.  Abra la ficha de almacén PLATA.  
3.  Active la casilla **Picking requerido**.  

## <a name="creating-the-sales-order"></a>Crear el pedido de venta  
Los pedidos de venta son el tipo más común de documento de origen de salida.  

### <a name="to-create-the-sales-order"></a>Para crear el pedido de venta  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**.  
3.  Crea un pedido de venta para el cliente 10000 en la fecha de trabajo (23 de enero) con la línea de pedido de venta siguiente.  

    |Producto|Cód. almacén|Cantidad|  
    |----------|-------------------|--------------|  
    |LS_81|PLATA|30|  

     Empiece a notificar el almacén para el que el pedido de venta está preparado para la manipulación en almacén.  

4.  Seleccione la acción **Liberar**.  

    Juan comienza a realizar el picking y a enviar a productos vendidos.  

## <a name="picking-and-shipping-items"></a>Picking y envío de productos  
En la ventana **Picking inventario**, puede administrar todas las actividades de almacén de salida para un documento de origen determinado, como un pedido de venta.  

### <a name="to-pick-and-ship-items"></a>Realizar el picking y el envío de productos  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Picking inventario** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**.  
3.  Seleccione el campo **Documento origen** y luego **Pedido venta**.  
4.  Seleccione el campo **Nº origen**, la línea para la venta al cliente 10000 y, a continuación, el botón **Aceptar**.  

    De forma alternativa, seleccione la acción **Tomar documento origen** y, a continuación, seleccione la orden de venta.  
5.  Seleccione la acción **Autorrellenar el campo Cdad. para manipular**.  

    También, en el campo **Cdad. a manipular**, introduzca 10 y 30 respectivamente en las dos líneas del picking de existencias.  
6.  Seleccione la acción **Registrar**, seleccione **Enviar** y, a continuación, el botón **Aceptar**.  

    Los 30 altavoces ahora se registran como preparados desde las ubicaciones S-01-0001 y S-01-0002, y un movimiento de producto negativo se crea para reflejar el histórico de remisiones de venta.  

## <a name="see-also"></a>Consulte también  
 [Cómo realizar picking de productos con picking inventario](warehouse-how-to-pick-items-with-inventory-picks.md)   
 [Procedimiento: realice un picking de los artículos para el envío de almacén](warehouse-how-to-pick-items-for-warehouse-shipment.md)   
 [Procedimiento: configure almacenes básicos con áreas de operaciones](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md)   
 [Procedimiento: mueva componentes a un área de operaciones en configuraciones básicas de almacén](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md)   
 [Procedimiento: Selección de producción o la Lista montaje](warehouse-how-to-pick-for-production.md)   
 [Mover productos ad hoc en configuraciones básicas de almacén](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md)   
 [Detalles de diseño: Flujo de salida del almacén](design-details-outbound-warehouse-flow.md)   
 [Tutorial de procesos empresariales](walkthrough-business-process-walkthroughs.md)  
 [Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

