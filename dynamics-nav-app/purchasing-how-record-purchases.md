---
title: Registro de compras
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 6d1933bf1e1c9236d34d429a4da84c907df13708
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-purchases"></a>Registro de compras
Cree una factura o una orden de compra para registrar el costo de las compras y para realizar el seguimiento de los pagos. Si necesita controlar un inventario, las facturas y las órdenes de compra también se utilizan para actualizar dinámicamente los niveles de inventario para que pueda minimizar sus costos de inventario y proporcionar un mejor servicio al cliente. Los costos de compra, incluidos los gastos del servicio y los valores de inventario resultantes del registro de las facturas o las órdenes de compra, contribuyen a las cifras de ganancias y otros KPI financieros en su página principal.

**Nota**: Debe usar órdenes de compra si el proceso de compra requiere que registre recibos parciales de una cantidad de la orden, por ejemplo, porque el proveedor no disponía de la cantidad total. Si vende productos que se entregan directamente desde el proveedor al cliente, como remisión directa, debe usar también órdenes de compra. Para obtener más información, vea [Procedimiento: Realizar envíos directos](sales-how-drop-shipment.md). En todos los demás aspectos, las órdenes de compra funcionan de la misma forma que las facturas de compra. El procedimiento siguiente se basa en una factura de compra. Los pasos son parecidos para una orden de compra.

Cuando se reciben los productos de inventario, o cuando se completa el servicio comprado, se registra la factura o la orden de compra para actualizar el inventario y los registros financieros, y para activar el pago al proveedor según los términos de pago. Para obtener más información, consulte [Realizar pagos](payables-make-payments.md).

**Atención**: No registre una factura de compra hasta que reciba los productos y conozca el costo final de la compra, incluidos los gastos adicionales. De lo contrario, las cifras de valor de inventario y de ganancias pueden estar sesgadas.

Si ya ha pagado productos en la factura de compra registrada, deberá crear una nota de crédito de compras para revertir la compra. Para obtener más información, vea [Procedimiento: Procesar devoluciones de compra o cancelaciones](purchasing-how-process-purchase-returns-cancellations.md).

Los productos pueden ser productos de inventario y servicios. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md). El proceso de la factura de compra es el mismo para ambos tipos de producto.



Puede rellenar los campos del proveedor en la factura de compra de dos maneras dependiendo de si el proveedor ya está registrado.

## <a name="to-create-a-purchase-invoice"></a>Para crear una nueva factura de compra
1. En la página Inicio, seleccione la acción **Factura de compra**.  
2. En el campo **Proveedor**, escriba el nombre de un cliente existente.

    Otros campos de la ventana **Factura de compra** se rellenarán con la información estándar del proveedor seleccionado. Si el proveedor no está registrado, realice los pasos siguientes:
3. En el campo **Proveedor**, especifique el nombre del proveedor nuevo.
4. En el cuadro de diálogo que registra al nuevo proveedor, seleccione el botón **Sí**.
5. En la ventana **Seleccionar una plantilla para un proveedor nuevo**, seleccione una plantilla en la que se basará la nueva ficha de proveedor y, a continuación, haga clic en el botón **Aceptar**.
6. Una nueva ficha de proveedor se abre, prellenada con información sobre la plantilla de proveedor seleccionada. El campo **Nombre** se rellena previamente con el nombre del nuevo proveedor que especificó en la factura de compra.
7. Rellene los campos restantes de la ficha de proveedor. Para obtener más información, vea [Procedimiento: Registrar nuevos proveedores](purchasing-how-register-new-vendors.md).  
8. Cuando haya completado la ficha de proveedor, seleccione el botón **Aceptar** para devolver a la ventana **Factura de compra**.

    Varios campos de la ventana **Factura de compra** ahora están rellenados con la información especificada en la nueva ficha del proveedor.
9. Rellene los campos en la ventana **Factura de compra** según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

    Ya puede empezar a rellenar las líneas de la factura de compra con los productos de inventario o los servicios que ha comprado del proveedor.

    **Nota**: Si ha configurado líneas de compra periódicas para el proveedor, como una orden de reabastecimiento mensual, puede insertarlas en la factura eligiendo el botón **Obtener líneas de compra periódicas**.
10. En la ficha desplegable **Líneas**, en el campo **N.º producto**,  introduzca el número de un producto de inventario o servicio.
11. En el campo **Cantidad**, introduzca el número de productos que se van a comprar.

    **Nota**: Para los producto de tipo **Servicio** la cantidad es una unidad de tiempo, por ejemplo horas, según se indica en el campo **Cód. unidad medida** en la línea.

    El campo **Importe línea** se actualiza para mostrar el valor del campo **Costo unit. directo** multiplicado por el valor del campo **Cantidad**.

    El precio y el importe de las líneas se muestran con o sin IVA dependiendo de qué seleccione en el campo **Precios incluyendo IVA** en la ficha del proveedor.
12. En el campo **Importe descuento factura**, especifique un importe que se debe descontar del valor que aparece en el campo **Total IVA incl.** en la parte inferior de la factura.

    **Nota**: Si ha configurado descuentos en factura para el proveedor, el valor porcentual especificado se inserta automáticamente en el campo **% descuento en factura de proveedor** si se cumplen los criterios, y el importe relacionado se inserta en el campo **Importe descuento factura**.
13. Cuando reciba los productos o servicios comprados, seleccione **Registrar**.

La compra ahora se refleja en el inventario y en los registros financieros, y se activa el pago al proveedor. La factura de compra se elimina de la lista de facturas de compra y se reemplaza con un nuevo documento de la lista de facturas de compra registradas.

## <a name="see-also"></a>Consulte también  
[Gestionar compras](purchasing-manage-purchasing.md)  
[Configurar compra](purchasing-setup-purchasing.md)  
[Compra de productos para una venta](purchasing-how-purchase-products-sale.md)  
[Registro de proveedores nuevos](purchasing-how-register-new-vendors.md)  
[Procedimiento: Preparar envíos directos](sales-how-drop-shipment.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)
