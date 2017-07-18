---
title: "Procedimiento: Realizar envíos directos"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f636de789dc6b006a449ec59c390fab85e62b443
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-drop-shipments"></a>Procedimiento: Realizar envíos directos
Una remisión directa es la remisión de los productos de uno de sus proveedores directamente a uno de sus clientes.

Cuando marca una orden de venta para envío directo y crea una orden especificando el cliente en el campo **Venta a-N.º cliente**. puede vincular los dos documentos y así asignar instrucciones al proveedor para que envíe el producto directamente al cliente.

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Para crear una orden de venta de remisión directa
Para preparar una remisión directa, cree una orden de venta como si fuese normal, pero indique en la línea de ventas que dicha venta requiere una remisión directa.

1. Cree una orden de venta para un artículo. Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).
2. En la línea de la orden de venta del artículo con envío directo, seleccione la casilla **Envío directo**.

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
1. Seleccione la línea de la orden de compra de envío directo, elija las acciones **Orden**, **Envío directo** y, a continuación, **Orden de compra**.

Se abre la orden de compra vinculada.

## <a name="to-post-a-drop-shipment"></a>Para registrar una remisión directa
Cuando el proveedor ha enviado los artículos, puede establecer las órdenes de venta como enviadas. También puede registrar la orden de compra, pero solo con la opción **Recibir** hasta que se haya facturado la orden de venta.
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Órdenes de venta** y, a continuación, seleccione el vínculo relacionado.
2. Abra la orden de venta que ha creado en la sección "Para crear una orden de venta de remisión directa".
3. En el campo **Cantidad a enviar**, especifiqué qué cantidad de la orden debe enviarse, todo o solo una parte.
3. Seleccione la acción **Registrar** o **Registrar y enviar**.
4. Elija la opción **Enviar** para facturar más adelante o la opción **Enviar y facturar** para facturar ahora.

## <a name="see-also"></a>Consulte también
[Vender productos](sales-how-sell-products.md)    
[Registro de compras](purchasing-how-record-purchases.md)  
[Gestionar ventas](sales-manage-sales.md)  
[Gestionar inventario](inventory-manage-inventory.md)      
[Trabajar con Dynamics NAV](ui-work-product.md)

