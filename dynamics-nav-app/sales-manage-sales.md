---
title: Gestor de ventas
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
ms.openlocfilehash: 20e380abb2f8f598391a66e50a7ec7a1c8b15fa1
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="manage-sales"></a>Gestor de ventas
Puede crear una factura o una orden de venta para registrar el contrato con un cliente para vender determinados productos según términos de entrega y pago determinados.

Debe usar órdenes de venta si el proceso de venta requiere que pueda enviar parte de una cantidad de la orden, por ejemplo, porque la cantidad total no está disponible a la vez. Si vende productos que se entregan directamente desde el proveedor al cliente, como remisión directa, deberá usar también órdenes de venta. En todos los demás aspectos, las órdenes de venta funcionan de la misma forma que las facturas de venta.  

Las buenas prácticas de ventas y marketing consisten en tomar las mejores decisiones en los momentos adecuados. La funcionalidad de marketing de Dynamics NAV proporciona un resumen preciso y puntual sobre la información de contacto para que pueda servir a sus clientes potenciales con más eficacia y aumentar la satisfacción de sus clientes. Para obtener más información, vea [Gestión de relaciones](marketing-relationship-management.md).

Puede negociar con el cliente creando primero una cotización venta, que puede convertir en una factura de venta cuando acuerde la venta. Después de que el cliente haya confirmado el contrato, por ejemplo, después de un proceso de cotización, puede enviar una confirmación de orden para registrar su obligación de entregar los productos según se ha acordado.

Cuando se entregan los productos, ya sea total o parcialmente, registra la factura de ventas o la orden de venta como enviadas o como enviadas y facturadas para crear el producto relacionado y los movimientos de cliente en su sistema.

En entornos de negocio donde el cliente debe pagar antes de que los productos se entreguen, por ejemplo en la venta minorista, debe esperar la recepción del pago antes de entregar los productos. En la mayoría de casos, puede procesar los pagos entrantes algunas semanas después de la salida liquidando los pagos a las facturas relacionadas, registradas como facturas de ventas no pagadas . Para obtener más información, vea [Procedimiento: Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).

Los documentos de ventas se pueden enviar como archivos PDF adjuntos al correo electrónico. El cuerpo del correo electrónico contendrá un extracto del documento de ventas, como los productos, el importe total y un vínculo al sitio web de PayPal. Para obtener más información, vea [Procedimiento: Enviar documentos por correo electrónico](ui-how-send-documents-email.md).

Para todos los procesos de ventas, puede introducir un flujo de trabajo de aprobación, por ejemplo, para requerir que el administrador de contabilidad apruebe las compras grandes para ciertos clientes. Para obtener más información, vea [Uso de flujos de trabajo de aprobación](across-how-use-approval-workflows.md).

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.

|Para |Vea |
|---|----|
|Crea una cotización venta donde ofrece los productos según los términos negociables antes de convertir la cotización en una factura de venta.|[Realización de ofertas](sales-how-make-offers.md)|
|Crea una factura de venta para registrar el contrato con un cliente para vender productos según términos de entrega y pago determinados.|[Facturación de ventas](sales-how-invoice-sales.md)|
|Procesar una orden de venta que requiera una remisión parcial o directa.|[Vender productos](sales-how-sell-products.md)|
|Vincular una orden de venta a una orden de compra para vender un producto de remisión directa que se entregará directamente desde el proveedor al cliente.|[Procedimiento: Realizar envíos directos](sales-how-drop-shipment.md)|
|Crea una nota de crédito de ventas para revertir una factura de venta registrada específica para reflejar qué productos devuelve el cliente y qué importe de pago se reembolsará.|[Procesamiento de devoluciones de ventas o cancelaciones](sales-how-process-sales-returns-cancellations.md)|
|Cree una ficha de cliente para cada cliente al que vende.|[Registro de clientes nuevos](sales-how-register-new-customers.md)|

## <a name="see-also"></a>Consulte también  
[Configurar ventas](sales-setup-sales.md)  
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar pagos](payables-manage-payables.MD)      
[Trabajar con Dynamics NAV](ui-work-product.md)  
[Con varias áreas de negocio](ui-across-business-areas.md)

