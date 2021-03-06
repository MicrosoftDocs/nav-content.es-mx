---
title: Crear una factura o un pedido de venta
description: "Describe cómo crear un recibo, o una factura o un pedido de venta, para registrar el acuerdo con un cliente para vender productos con condiciones específicas."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bill, sale, invoice, order
ms.date: 10/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7da07d1491fde4e555ea259f61babc02664094a8
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-invoice-sales"></a>Facturación de ventas
Puede crear una factura o una orden de venta para registrar el contrato con un cliente para vender determinados productos según términos de entrega y pago determinados.  

Hay un par de escenarios en los que debe usar un pedido de venta en lugar de una factura de venta:  

* Si necesita enviar solo parte de una cantidad del pedido, por ejemplo, porque no esté disponible toda la cantidad.  
* Si vende productos que el proveedor entrega directamente al cliente, lo que se denomina envío directo. Para obtener más información, vea [Procedimiento: Realizar envíos directos](sales-how-drop-shipment.md).  

En todos los demás aspectos, los pedidos de venta y las facturas de venta funcionan de la misma forma. Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).

Puede negocias con el cliente creando primero creando una cotización de venta, que puede convertir en una factura de venta cuando acuerde la venta. Para obtener más información, vea [Procedimiento: Realización de cotizaciones](sales-how-make-offers.md).

Si el cliente decide comprar, registre la factura de venta para crear los movimientos de cantidad y valor relacionados. Cuando registre la factura de venta, también puede enviar por correo electrónico el documento como un PDF anexo. Puede tener el cuerpo de correo electrónico rellenado con un resumen de la factura y la información de pagos, como un vínculo a PayPal. Para obtener más información, vea [Procedimiento: Enviar documentos por correo electrónico](ui-how-send-documents-email.md).

En entornos de negocio donde el cliente debe pagar antes de que los productos se entreguen, por ejemplo en la venta minorista, debe esperar la recepción del pago antes de entregar los productos. En la mayoría de casos, puede procesar los pagos entrantes algunas semanas después de la salida liquidando los pagos a las facturas relacionadas, registradas como facturas de ventas no pagadas . Para obtener más información, vea [Procedimiento: Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).

Puede corregir o cancelar fácilmente una factura de venta registrada antes de que se pague. Por ejemplo, esto es útil si se desea corregir un error de escritura o si el cliente solicita un cambio temprano en el proceso de pedido. Para obtener más información, vea [Procedimiento: Corregir o cancelar las facturas de venta sin abonar](sales-how-correct-cancel-sales-invoice.md) Si la factura de venta registrada se ha pagado, deberá crear una nota de crédito de ventas para revertir la venta. Para obtener más información, vea [Procedimiento: Procesar devoluciones de ventas o cancelaciones](sales-how-process-sales-returns-cancellations.md).

Puede rellenar los campos de clientes en la factura de venta de dos formas en función de si el cliente ya está registrado. Consulte los pasos 2 y 3 del siguiente procedimiento.

## <a name="to-create-a-sales-invoice"></a>Para crear una factura de venta
1. En la página Inicio, seleccione la acción **Facturas de ventas**.  
2. En el campo **Cliente**, escriba el nombre de un cliente existente.

   Otros campos de la ventana **Factura venta** contienen información estándar sobre el cliente seleccionado. Si el cliente no está registrado, realice los pasos siguientes:
3. En el campo **Cliente**, escriba el nombre del cliente nuevo.
4. En el cuadro de diálogo de registro de nuevos clientes, haga clic en el botón **Sí**.
5. En la ventana **Seleccionar una plantilla para un cliente nuevo**, seleccione una plantilla en la que se basará la nueva ficha de cliente y, a continuación, haga clic en el botón **Aceptar**.
6. Una nueva ficha de cliente muestra la información sobre la plantilla de cliente seleccionada. Rellene el resto de campos. Para obtener más información, vea [Procedimiento: Registrar nuevos clientes](sales-how-register-new-customers.md).  
7. Cuando haya completado la ficha cliente, haga clic en el botón **Aceptar** para volver a la ventana **Factura venta**.

   Muchos campos de la factura de venta se rellenan con la información especificada en la nueva ficha de cliente.  
8. Rellene los campos en la ventana **Factura de venta** según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

Ahora podrá rellenar las líneas de la factura de venta de los productos que vende al cliente o para cualquier transacción con el cliente que desee registrar en una cuenta de contabilidad.   

Si ha configurado líneas de venta periódicas para el cliente, por ejemplo, una orden de reabastecimiento mensual, puede insertar estas líneas en la orden al elegir la acción **Obtener líneas de venta periódicas**.  
9. En la ficha desplegable **Líneas** del campo **Tipo**, seleccione qué tipo de producto, cargo o transacción registrará para el cliente en la línea de venta.
10. En el campo **N.º**, seleccione un registro para registrar según el valor del campo **Tipo**.

 Deje el campo **N.º** vacío en los casos siguientes: - Si la línea es de un comentario. Escriba el comentario en el campo **Descripción**.
 - Si la línea es de un producto no inventariable. Elija la acción **Seleccionar artículos sin stock**. Para obtener más información, consulte [Trabajar con productos sin stock](inventory-how-work-nonstock-items.md).

11. En el campo **Cantidad**, especifique cuántas unidades de producto, cargo o transacción registrará la línea para el cliente.  

    El valor del campo **Importe línea** se calculará como *Precio venta* x *Cantidad*.  

    El precio y el importe de las líneas tienen IVA o no, dependiendo de qué seleccione en el campo **Precios incluyendo IVA** en la ficha del cliente.  
12. Si desea ofrecer un descuento, introduzca un porcentaje en el campo **% Descuento línea**. El valor del campo **Importe de línea** se actualiza según corresponde.  

    Si hay configurados precios de producto especiales en la ficha desplegable **Precios venta y descuentos línea ventas** en la ficha del producto o en la del cliente, el precio y el importe de la línea de venta se actualizan automáticamente si se cumplen los criterios acordados para el precio. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).  
13. Repita los pasos 9 a 12 para cada producto o cargo que desee vender al cliente.  

    Los totales por debajo de las líneas se calculan automáticamente cuando se crean o modifican las líneas.  
14. En el campo **Importe descuento factura**, especifique un importe que se debe descontar del valor que aparece en el campo **Total impuesto incl.** en la parte inferior de la factura.

    Si ha configurado descuentos en factura para el cliente, el valor porcentual especificado se inserta automáticamente en el campo **% descuento en factura** si se cumplen los criterios, y el importe relacionado se inserta en el campo **Descuento en factura excluyendo impuesto** . Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).  
15. Cuando las líneas de la factura de venta ya estén completas, seleccione la acción **Registrar y enviar**.  

El cuadro de diálogo **Registrar y enviar confirmación** muestra el método preferido del cliente para recibir documentos. Puede cambiar el método de envío seleccionando el botón de búsqueda en el campo **Enviar documento a**. Para obtener más información, vea [Procedimiento: Configurar los perfiles de envío de documentos](sales-how-setup-document-send-profiles.md).

El producto relacionado y los movimientos de cliente se han creado ahora en su sistema y la factura de venta se genera como un documento PDF. La factura de venta se elimina de la lista de facturas de venta y se reemplaza con un nuevo documento de la lista de facturas de venta registradas.

## <a name="see-also"></a>Consulte también
[Ventas](sales-manage-sales.md)  
[Configuración de ventas](sales-setup-sales.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Enviar documentos por correo electrónico.](ui-how-send-documents-email.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

