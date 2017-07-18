---
title: Gestionar compras
author: SorenGP
ms.custom: na
ms.date: 11/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df94e447d7d4542f75f3c34105099016b0abbf32
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="manage-purchasing"></a>Gestionar compras
Cree una factura o una orden de compra para registrar el costo de las compras y para realizar el seguimiento de los pagos. Si necesita controlar un inventario, las facturas de compra también se utilizan para actualizar dinámicamente los niveles de inventario para que pueda minimizar sus costos de inventario y proporcionar un mejor servicio al cliente. Los costos de compra, incluidos los gastos del servicio y los valores de inventario resultantes del registro de las facturas de compra, contribuyen a las cifras de ganancias y otros KPI financieros en su página Inicio.

Debe usar órdenes de compra si el proceso de compra requiere que registre recibos parciales de una cantidad de la orden, por ejemplo, porque el proveedor no disponía de la cantidad total. Si vende productos que se entregan directamente desde el proveedor al cliente, como remisión directa, debe usar también órdenes de compra. Para obtener más información, vea [Procedimiento: Realizar envíos directos](sales-how-drop-shipment.md). En todos los demás aspectos, las órdenes de compra funcionan de la misma forma que las facturas de compra.

Puede crear facturas automáticamente mediante el servicio OCR (reconocimiento óptico de caracteres) para convertir facturas PDF de sus proveedores en documentos electrónicos, que se convierten en facturas de compra mediante un flujo de trabajo. Para usar esta funcionalidad, primero debe registrarse en el servicio OCR y, a continuación, realizar algunas configuraciones. Para obtener más información, vea [Procedimiento: Procesar documentos entrantes](across-process-income-documents.md).      

**Nota**: En Dynamics NAV, se usa el término "producto" para denominar los artículos.

Los productos pueden ser productos de inventario y servicios. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

Para todos los procesos de compra, puede introducir un flujo de trabajo de aprobación, por ejemplo, para requerir que el administrador de contabilidad apruebe las compras grandes. Para obtener más información, vea [Uso de flujos de trabajo de aprobación](across-how-use-approval-workflows.md).

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen. Dichas tareas se enumeran en el orden en el que generalmente se llevan a cabo.


|Para |Vea |
|---|----|
|Cree una factura de compra para registrar el contrato con un proveedor para comprar productos según términos de entrega y pago determinados. |[Registro de compras](purchasing-how-record-purchases.md)|
|Crear una factura de compra para todas las líneas en una factura de venta o las seleccionadas.|[Compra de productos para una venta](purchasing-how-purchase-products-sale.md)|
|Cree una nota de crédito de compras para revertir una factura de compra registrada específica para reflejar qué productos se están devolviendo al proveedor y qué importe de pago se cobrará.|[Procesamiento de devoluciones de compra o cancelaciones](purchasing-how-process-purchase-returns-cancellations.md)|
|Cree una ficha de proveedor para cada proveedor del que compre.|[Registro de proveedores nuevos](purchasing-how-register-new-vendors.md)|

## <a name="see-also"></a>Consulte también
[Configurar compra](purchasing-setup-purchasing.md)  
[Gestionar pagos](payables-manage-payables.md)    
[Trabajar con Dynamics NAV](ui-work-product.md)  
[Con varias áreas de negocio](ui-across-business-areas.md)

