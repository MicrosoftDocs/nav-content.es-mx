---
title: Gestionar cobros
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 3f2be627dfda9720e9f31fd227164d1c27116d2c
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="manage-receivables"></a>Gestionar cobros#
Una tarea principal en la gestión de los cobros es liquidar pagos entrantes a sus movimientos de proveedor o cliente relacionados y cerrar las facturas de ventas relacionadas o los abonos de compra como pagados. Cuando se liquidan todos los pagos, puede conciliar la cuenta bancaria.  

Puede realizar esta tarea en la ventana **Diario de conciliación de pagos** importando una fuente o archivo de extracto bancario para registrar rápidamente los pagos en Dynamics NAV. Una función de liquidación automática liquida los pagos a sus movimientos de cliente o proveedor abiertos relacionados en función de las coincidencias de datos entre el texto de pago y la información de movimiento. Puede revisar y cambiar las liquidaciones automáticas entes de registrar el diario. Puede elegir cerrar los movimientos de banco pendientes relacionados con los movimientos liquidados cuando registra el diario. Significa que la cuenta bancaria se concilia automáticamente cuando se liquidan todos los pagos.

**Nota**: Concilie cuentas bancarias como una tarea independiente en la ventana **Conciliación de cuentas bancarias**, que también admite movimientos de cheque. Para obtener más información, vea [Procedimiento: Conciliar cuentas bancarias por separado](bank-how-reconcile-bank-accounts-separately.md).

De forma alternativa, puede liquidar pagos en la ventana **Registro de pagos** comprobando manualmente los pagos recibidos como efectivo, cheque o transacción bancaria frente a una lista de documentos de ventas sin pagar. Tenga en cuenta que esta funcionalidad solo esta disponible para documentos de ventas.

Como cualquier otra conciliación de pagos manual, puede registrar cada recepción en la cuenta de contabilidad, cliente u otra cuenta pertinente al especificar una línea de pago en la ventana **Diario de recepciones de efectivo**. En ese caso, puede liquidar la recepción o el reembolso en uno o varios movimientos pendientes antes de registrar el diario de recepciones de efectivo o puede liquidarlos desde movimientos de cliente creados.

Otra tarea de la gestión de cobros es recopilar saldos pendientes, incluso para gestionar la configuración de los intereses y emitir recordatorios.

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.

|Para |Vea |
|---|----|
|Liquide pagos en los movimientos pendientes de cliente o proveedor en función de un archivo o una fuente de estado de cuenta bancario importado y concilie la cuenta bancaria una vez liquidados todos los pagos.|[Liquidar pagos automáticamente y conciliar cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|Liquide pagos para abrir movimientos de cliente basados en una introducción manual de datos en una lista de documentos de ventas sin pagar. | [Conciliar pagos manualmente de una lista de documentos de venta sin abonar](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md)|
|Registre reembolsos o recepciones de efectivo de clientes en el diario de cobros y aplíquelos a movimientos de cliente, ya sea desde el diario o desde movimientos registrados. | [Conciliar pagos de cliente manualmente](receivables-how-apply-sales-transactions-manually.md) |
|Recordar a los clientes los importes vencidos, calcular intereses y administrar los cobros. | [Cobrar saldos pendientes](receivables-collect-outstanding-balances.md) |

## <a name="see-also"></a>Consulte también
[Gestionar ventas](sales-manage-sales.md)  
[Gestionar pagos](payables-manage-payables.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)  
[Con varias áreas de negocio](ui-across-business-areas.md)

