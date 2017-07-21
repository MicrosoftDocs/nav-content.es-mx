---
title: "Liquidar pagos automáticamente y conciliar cuentas bancarias"
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
ms.openlocfilehash: 11df387c16e19421090531fd03c209103b9989d9
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="apply-payments-automatically-and-reconcile-bank-accounts"></a>Liquidar pagos automáticamente y conciliar cuentas bancarias
Debe conciliar con frecuencia las cuentas bancarias, las de cobros y las de pagos en Dynamics NAV liquidando pagos registrados en el banco en sus facturas sin abonar relacionadas, abonos y otros movimientos pendientes en Dynamics NAV.

Puede realizar esta tarea en la ventana **Diario de conciliación de pagos** importando una fuente o archivo de extracto bancario para registrar rápidamente los pagos en Dynamics NAV. Una función de liquidación automática liquida los pagos a sus movimientos de cliente o proveedor abiertos relacionados en función de las coincidencias de datos entre el texto de pago y la información de movimiento. Puede revisar y cambiar las liquidaciones automáticas entes de registrar el diario. Puede elegir cerrar los movimientos de banco pendientes relacionados con los movimientos liquidados cuando registra el diario. Significa que la cuenta bancaria se concilia automáticamente cuando se liquidan todos los pagos.

Para habilitar la importación de extractos bancarios como fuente de banco, primero debe configurar y habilitar el servicio de fuente de banco de Envestnet Yodlee y, a continuación, vincular sus cuentas bancarias a las cuentas bancarias en línea relacionadas. Para obtener más información, vea [Procedimiento: Configuración del servicio de fuentes de banco de Envestnet Yodlee](bank-how-setup-bank-statement-service.md)

**Nota**: es posible que el servicio Fuentes de banco de Envestnet Yodlee, o el servicio fuentes de banco de otro proveedor, no esté disponible en su sistema. Póngase en contacto con su socio de Microsoft si desea usar un servicio de fuentes de banco para importar extractos bancarios.

De forma alternativa, puede usar el servicio de conversión de datos bancarios para que se pueda importar a Dynamics NAV un archivo de estado de cuenta bancario en cualquier formato convertido a un flujo de datos. Para obtener más información, vea [Procedimiento: Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md).

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.

|Para |Vea |
|---|----|
|Liquide los pagos en los movimientos pendientes de cliente o proveedor importando un estado de cuenta bancario y concilie la cuenta bancaria cuando se liquiden todos los pagos. | [Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md) |
|Liquide manualmente pagos viendo información detallada sobre datos coincidentes y sugerencias para movimientos pendientes candidatos en los que liquidar pagos. | [Revisar o liquidar pagos después de una liquidación automática](receivables-how-review-apply-payments-auto-application.md)
|Resuelva los pagos que no se puedan liquidar automáticamente en sus movimientos pendientes relacionados, por ejemplo, porque los importes son diferentes o porque no hay ningún movimiento relacionado. | [Procedimiento: Conciliar pagos que no se pueden liquidar automáticamente](receivables-how-reconcile-payments-cannot-apply-auto.md)
|Vincule el texto sobre pagos con cuentas concretas de cliente, de proveedor o de contabilidad para que siempre se registren recepciones de cobro o gastos periódicos en dichas cuentas cuando no haya documentos a los que aplicarlos.| [Asignación de texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)|

## <a name="see-also"></a>Consulte también
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar ventas](sales-manage-sales.md)

