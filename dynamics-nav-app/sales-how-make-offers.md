---
title: "Realización de cotizaciones"
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
ms.openlocfilehash: e126c755a9121c3a91f3af72f3f1ae14702a4701
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-make-offers"></a>Realización de cotizaciones
Puede crear una cotización venta para registrar la oferta realizada a un cliente para vender determinados productos según ciertos términos de entrega y pago. Puede enviar la cotización venta al cliente para comunicar la oferta. Puede enviar por correo electrónico el documento como un documento PDF anexo. También puede rellenar previamente el cuerpo del correo electrónico con un resumen de la cotización. Para obtener más información, vea [Procedimiento: Enviar documentos por correo electrónico](ui-how-send-documents-email.md).

Mientras negocia con el cliente, puede cambiar y reenviar la cotización venta el número de veces que sea necesario. Cuando el cliente acepte la cotización, convierta la cotización venta en una factura de venta o una orden de venta en la que se procese la venta. Para obtener más información, consulte [Procedimiento: Facturar ventas](sales-how-invoice-sales.md) o [Procedimiento: Vender productos](sales-how-sell-products.md).

Los productos pueden ser productos de inventario y servicios. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md). El proceso de cotización venta es el mismo para ambos tipos de producto.

**Nota**: En Dynamics NAV, se usa el término "producto" para denominar los artículos.

Puede rellenar los campos de cliente en la cotización venta de dos formas si el cliente ya está registrado.

## <a name="to-create-a-sales-quote"></a>Para crear una cotización venta
1. En la página Inicio, seleccione la acción **Cotización venta**.  
2. En el campo **Cliente**, escriba el nombre de un cliente existente.

    Otros campos de la ventana **Cotización venta** se rellenarán con la información estándar del cliente seleccionado. Si el cliente no está registrado, realice los pasos siguientes:

3. En el campo **Cliente**, escriba el nombre del cliente nuevo.
4. En el cuadro de diálogo de registro de nuevos clientes, haga clic en el botón **Sí**.
5. En la ventana **Seleccionar una plantilla para un cliente nuevo**, seleccione una plantilla en la que se basará la nueva ficha de cliente y, a continuación, haga clic en el botón **Aceptar**.
6. Una nueva ficha de cliente se abre, prellenada con información sobre la plantilla de cliente seleccionada. El campo **Nombre** se rellena con el nombre del nuevo cliente que especificó en la factura de venta.
7. Rellene los campos restantes de la ficha de cliente. Para obtener más información, vea [Procedimiento: Registrar nuevos clientes](sales-how-register-new-customers.md).  
8. Cuando haya completado la ficha cliente, haga clic en el botón **Aceptar** para volver a la ventana **Cotización venta**.

    Muchos campos de la cotización venta se rellenan con la información especificada en la nueva ficha cliente.
9. Rellene los campos en la ventana **Cotización de venta** según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

    Ya está preparado para rellenar las líneas de la cotización venta con los productos de inventario o los servicios que quiera ofrecer al cliente.

    **Nota**: Si ha configurado líneas de venta periódicas para el cliente, como una orden de reabastecimiento mensual, puede insertar estas líneas en la cotización al elegir la acción **Obtener líneas de venta periódicas**.
10. En la ficha desplegable **Líneas**, en el campo **N.º producto**,  introduzca el número de un producto de inventario o servicio.
11. En el campo **Cantidad**, escriba el número de productos que se van a ofrecer.

    **Nota**: Para los producto de tipo Servicio la cantidad es una unidad de tiempo, por ejemplo horas, según se indica en el campo **Cód. unidad medida** en la línea.

    El campo **Importe línea** se actualiza para mostrar el valor del campo **Precio unitario** multiplicado por el valor del campo **Cantidad**.

    El precio y el importe de las líneas se muestran con o sin IVA dependiendo de qué seleccione en el campo **Precios incluyendo el impuesto de ventas** en la ficha del cliente.
12. En el campo **% Descuento línea**, especifique un porcentaje si desea conceder al cliente un descuento para el producto. El valor del campo **Importe de línea** se actualiza según corresponde.

    **Nota**: Si ha configurado precios de producto especiales en la ficha desplegable **Precios venta y descuentos línea ventas** en la ficha del producto o en la del cliente, el porcentaje de descuento y el precio que figuran en la línea de cotización se actualizan automáticamente si se cumplen los criterios acordados respecto del precio. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).
13. Para agregar un comentario acerca de la línea de cotización que el cliente puede ver en la cotización de venta impresa, escriba un texto en el campo **Descripción** en una línea vacía.  
14. Repita los pasos 10 a 13 para cada producto que desee ofertar al cliente.

    Los totales por debajo de las líneas se calculan automáticamente cuando se crean o modifican las líneas.
15. En el campo **Importe descuento factura**, especifique un importe que se debe descontar del valor que aparece en el campo **Total impuesto incl.** en la parte inferior de la factura.

    **Nota**: Si ha configurado descuentos en factura para el cliente, el valor porcentual especificado se inserta automáticamente en el campo **% descuento en factura** si se cumplen los criterios, y el importe relacionado se inserta en el campo **Descuento en factura excluyendo IVA**. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).
16. Cuando las líneas de la cotización de venta ya estén completas, seleccione la acción **Enviar por correo electrónico** o **Imprimir**.

    Si ha seleccionado la acción **Enviar por correo electrónico**, se adjunta automáticamente un archivo PDF a un mensaje correo electrónico para el cliente. Puede configurar el correo electrónico para que contenga un resumen de la cotización. Para obtener más información, vea [Procedimiento: Enviar documentos por correo electrónico](ui-how-send-documents-email.md).
17. Si el cliente acepta la cotización, seleccione la acción **Generar factura** o **Realizar orden**.

La cotización venta se quita de la base de datos. Una factura de venta o una orden de venta se crea a partir de la información de la cotización venta en la que puede procesar la venta. En el campo **N.º cotización**, de la factura de venta o de la orden de venta puede ver el número de la cotización venta a partir de la que se creó. Para obtener más información, consulte [Procedimiento: Facturar ventas](sales-how-invoice-sales.md) o [Procedimiento: Vender productos](sales-how-sell-products.md).

## <a name="see-also"></a>Consulte también  
[Gestionar ventas](sales-manage-sales.md)  
[Configurar ventas](sales-setup-sales.md)  
[Enviar documentos por correo electrónico](ui-how-send-documents-email.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

