---
title: Tareas para conciliar cuentas bancarias y liquidar pagos de los movimientos relacionados
description: "Describe las tareas para conciliar las cuentas de banco, cobros y pagos, registrar recibos de efectivo o gastos, y liquidar los pagos automáticamente."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: payment process, direct payment posting, reconcile payment, expenses, cash receipts
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 33c0661a2ebf9b8d9b817c026a8c9abf0f0eff91
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="applying-payments-automatically-and-reconciling-bank-accounts"></a>Liquidación de pagos automáticamente y conciliación de cuentas bancarias
Debe conciliar con frecuencia las cuentas bancarias, las de cobros y las de pagos liquidando pagos registrados en el banco en sus facturas sin abonar relacionadas, abonos y otros movimientos pendientes en [!INCLUDE[d365fin](includes/d365fin_long_md.md)].  

Puede realizar esta tarea en la ventana **Diario de conciliación de pagos** importando una fuente o archivo de extracto bancario para registrar rápidamente los pagos. Los pagos se liquidan en los movimientos de cliente o proveedor abiertos en función de las coincidencias entre el texto de pago y la información de movimiento. Puede revisar y cambiar las liquidaciones automáticas entes de registrar el diario. Puede elegir cerrar los movimientos de banco pendientes relacionados con los movimientos liquidados cuando registra el diario. La cuenta bancaria se concilia automáticamente cuando se liquidan todos los pagos.  

Para importar estados de cuenta bancarios como fuente de banco, primero debe configurar y habilitar el servicio de conversión de datos bancarios. Para obtener más información, vea [Procedimiento: Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md).  

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.  

| Para | Vea |
| --- | --- |
| Liquide los pagos en los movimientos pendientes de cliente o proveedor importando un estado de cuenta bancario y concilie la cuenta bancaria cuando se liquiden todos los pagos. |[Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md) |
| Liquide manualmente pagos viendo información detallada sobre datos coincidentes y sugerencias para movimientos pendientes candidatos en los que liquidar pagos. |[Revisar o liquidar pagos después de una liquidación automática](receivables-how-review-apply-payments-auto-application.md) |
| Resuelva los pagos que no se pueden liquidar automáticamente a sus movimientos pendientes relacionados. Por ejemplo, porque los importes son distintos o porque no existe ningún movimiento relacionado. |[Conciliar pagos que no se pueden liquidar automáticamente](receivables-how-reconcile-payments-cannot-apply-auto.md) |
| Vincule el texto sobre pagos con cuentas concretas de cliente, de proveedor o de contabilidad para que siempre se registren recepciones de cobro o gastos periódicos en dichas cuentas cuando no haya documentos a los que aplicarlos. |[Asignación de texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md) |

## <a name="see-also"></a>Consulte también
[Administrar cobros](receivables-manage-receivables.md)  
[Ventas](sales-manage-sales.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

