---
title: "Crear una orden de venta asociada a una orden de compra para un envío directo"
description: "Describe cómo crear una orden de venta vinculada a una orden de compra para habilitar el envío directo del proveedor al cliente."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: direct shipment
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 6a8210808532ff8945660c23f0bf91719e2f2963
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-make-drop-shipments"></a>Procedimiento: Realizar envíos directos
Un envío directo es el envío de los productos de uno de sus proveedores directamente a uno de sus clientes.

Cuando marca una orden de venta para envío directo y crea una orden especificando el cliente en el campo **Venta a-N.º cliente**. puede vincular los dos documentos y así asignar instrucciones al proveedor para que envíe el producto directamente al cliente.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Para crear una orden de venta de remisión directa
Para preparar una remisión directa, cree una orden de venta como si fuese normal, pero indique en la línea de ventas que dicha venta requiere una remisión directa.

1. Cree una orden de venta para un artículo. Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).
2. En la línea del pedido de venta del envío directo, seleccione la casilla **Envío directo**. Use la función **Elegir columnas** si el campo no está visible. Para obtener más información, vea [Personalización del usuario](ui-user-personalization.md).

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>Para crear órdenes de compra de remisión directa
Para preparar una remisión directa de un producto que se va a vender, cree una orden de compra como si fuese normal, pero indique en dicha orden que el producto debe enviarse directamente al cliente no a usted.

1. Cree una orden de compra. No rellene ningún campo en las líneas. Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).
2. En el campo **Venta a-N.º cliente**, seleccione el cliente al que le está vendiendo.
3. Elija la acción **Envíos directos** y, a continuación, **Tomar orden venta**.
4. En la ventana **Lista ventas**, seleccione la orden de venta que ha preparado en la sección "Para crear una orden de venta de envío directo".
5. Elija el botón **Aceptar**.

La información de la línea de la orden de venta se inserta en las líneas de la orden de compra.

Ahora puede asignar instrucciones al proveedor para que envíe los productos al cliente, por ejemplo, enviando la orden de compra por correo electrónico en formato PDF.     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>Para ver la orden de compra vinculada a la orden de venta
* Seleccione la línea de la orden de compra de envío directo, elija las acciones **Orden**, **Envío directo** y, a continuación, **Orden de compra**.

## <a name="to-post-a-drop-shipment"></a>Para registrar un envío directo
Después de que el proveedor envíe los productos, puede establecer los pedidos de venta como enviados. También puede registrar la orden de compra, pero solo con la opción **Recibir** hasta que se haya facturado la orden de venta.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.
2. Abra la orden de venta que ha creado en la sección "Para crear una orden de venta de remisión directa".
3. En el campo **Cantidad a enviar**, especifiqué qué cantidad de la orden debe enviarse, todo o solo una parte.
4. Seleccione la acción **Registrar** o **Registrar y enviar**.
5. Elija la opción **Enviar** para facturar más adelante o la opción **Enviar y facturar** para facturar ahora.

## <a name="see-also"></a>Consulte también
[Cómo crear pedidos especiales](sales-how-to-create-special-orders.md)|  
[Vender productos](sales-how-sell-products.md)  
[Registro de compras](purchasing-how-record-purchases.md)  
[Ccial](sales-manage-sales.md)  
[Inventario](inventory-manage-inventory.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

