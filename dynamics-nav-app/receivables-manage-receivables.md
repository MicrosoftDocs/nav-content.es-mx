---
title: Resumen de tareas para administrar los cobros
description: Describe tareas para administrar los cobros y liquidar los pagos en los movimientos de cliente o proveedor.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customer payment, debtor, balance due, AR
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: b9a486d099a6a52bec6ac6b23c21a3c341c20b14
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="managing-receivables"></a>Administrar cobros
Un paso normal en el ritmo financiero es conciliar las cuentas bancarias, lo que requiere liquidar pagos en las movimientos de cliente o propiedad para cerrar las facturas de venta y los abonos de compra.  

En [!INCLUDE[d365fin](includes/d365fin_md.md)], una de las formas más rápidas de registrar pagos desde la ventana **Diario de conciliación de pagos** mediante la importación de un archivo de extracto bancario o una fuente. Los pagos se liquidan en los movimientos de cliente o proveedor abiertos en función de las coincidencias de datos entre el texto de pago y la información de movimiento. Puede revisar y modificar las coincidencias antes de registrar el diario, y cerrar los movimientos de banco para los movimientos al registrar el diario. La cuenta bancaria se concilia cuando se liquidan todos los pagos.

No obstante, existen otros lugares prácticos para liquidar los pagos y para conciliar las cuentas bancarias:  

* La ventana **Conciliación banco**, que también le permite comprobar los movimientos contables. Para obtener más información, vea [Procedimiento: Conciliar cuentas bancarias por separado](bank-how-reconcile-bank-accounts-separately.md).  
* La ventana **Registro de pagos**, donde puede liquidar y comprobar manualmente los pagos recibidos como efectivo, cheque o transacción bancaria frente a una lista de documentos de ventas sin pagar. Tenga en cuenta que esta funcionalidad solo está disponible para documentos de ventas.  
* La ventana **Diario de recibos de efectivo**, donde puede registrar manualmente los albaranes en el libro mayor, cliente u otra cuenta pertinente introduciendo una línea de pago. Puede liquidar la recepción o el reembolso a uno o varios movimientos abiertos antes de registrar la recepción de efectivo o desde movimientos de cliente.  

Otra parte de la gestión de cobros es recopilar saldos pendientes, incluidos intereses, y emitir recordatorios. [!INCLUDE[d365fin](includes/d365fin_md.md)] también ofrece formas de realizar estas acciones. Para obtener más información, vea [Cobrar saldos pendientes](receivables-collect-outstanding-balances.md).  

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.  

| Para | Vea |
| --- | --- |
| Liquide pagos en los movimientos pendientes de cliente o proveedor en función de un archivo o una fuente de estado de cuenta bancario importado y concilie la cuenta bancaria una vez liquidados todos los pagos. |[Liquidación de pagos automáticamente y conciliación de cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md) |
| Liquide pagos para abrir movimientos de cliente basados en una introducción manual de datos en una lista de documentos de ventas sin pagar. |[Conciliar pagos manualmente de una lista de documentos de venta sin abonar](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md) |
| Registre reembolsos o recepciones de efectivo de clientes en el diario de cobros y aplíquelos a movimientos de cliente, ya sea desde el diario o desde movimientos registrados. |[Conciliar pagos de cliente manualmente](receivables-how-apply-sales-transactions-manually.md) |
| Recordar a los clientes los importes vencidos, calcular intereses y administrar los cobros. |[Cobrar saldos pendientes](receivables-collect-outstanding-balances.md) |
|Asegúrese de conocer el costo de los productos enviados. Para ello, asigne los costos de producto adicionales, tales como fletes, manipulación física, seguros y transporte, en los que incurra después de la venta.|[Utilizar los cargos de producto a cuenta para los costes comerciales adicionales](payables-how-assign-item-charges.md)|
|Configure una tolerancia por la que el sistema cierre una factura aunque el pago, incluido el descuento, no cubra totalmente el importe de la factura.|[Trabajar con tolerancias de pago y tolerancias de descuento de pago](finance-payment-tolerance-and-payment-discount-tolerance.md)|
## <a name="see-also"></a>Consulte también
[Ccial](sales-manage-sales.md)  
[Administrar pagos](payables-manage-payables.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Funciones empresariales generales](ui-across-business-areas.md)

