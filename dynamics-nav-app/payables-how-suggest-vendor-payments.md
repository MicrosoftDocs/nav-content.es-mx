---
title: Propuesta de pagos a proveedores
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
ms.openlocfilehash: 11bfba9f279f6bd84c5d169f6f97fd48759bc6df
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-suggest-vendor-payments"></a>Propuesta de pagos a proveedores
En la ventana **Diario de pagos**, puede usar una función para proponer líneas de pago según su configuración, como pagos que vencerán pronto o pagos a los que se puede aplicar un descuento.

Para beneficiarse totalmente de la función Proponer pagos de proveedor, primero debe dar prioridad a los proveedores. Para obtener más información, consulte [Procedimiento: Dar prioridad a proveedores](purchasing-how-prioritize-vendors.md).

Los movimientos del proveedor cuyo campo **En espera** no esté marcado, no se incluirán en el proceso.  

**Importante**: Si desea aprovechar los descuentos por pronto pago y ha introducido un importe disponible, el importe se usará primero para movimientos vencidos de proveedor con prioridad en orden de prioridad, después para movimientos vencidos de proveedor sin prioridad y, finalmente, para movimientos pendientes de proveedor a los que se puedan aplicar descuentos por pronto pago en orden de número de proveedor.

## <a name="to-use-the-suggest-vendor-payments-function"></a>Para usar la función Proponer pagos a proveedores
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de pago** y, a continuación, seleccione el enlace relacionado.
2. Abra el diario pertinente y, a continuación, elija la acción **Proponer pagos a proveedor**.
3. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
4. Elija el botón **Aceptar**.

## <a name="to-insert-the-due-date-as-posting-date-on-payment-journal-lines"></a>Para insertar la fecha de vencimiento como fecha de registro en líneas de diario de pagos
Cuando use el proceso **Proponer pagos a proveedores** para crear las líneas de pago para los proveedores, puede rellenar dos campos especiales para asegurarse de que las líneas de planificación usan la fecha de vencimiento para calcular la fecha de registro. Estos campos son **Calcular fecha de registro a partir de fecha de vencimiento de documento de aplicación** y **Desfase fecha de vencimiento de documento de aplicación**.

**Importante**: No puede usar el campo **Calcular fecha de registro a partir de fecha de vencimiento de documento de aplicación** junto con el campo **Buscar dtos. P.P.** o el campo **Una línea por proveedor**. El motivo es que si la fecha de registro se basa en la fecha de vencimiento, es posible que no se pueda calcular correctamente el descuento por pronto pago, porque la fecha de registro puede ser posterior a la fecha descuento pronto pago.
Además, si la fecha de registro calculada corresponde al pasado, la fecha de registro se adelantará a la fecha de trabajo y aparecerá una advertencia.

De forma alternativa, también puede crear manualmente las líneas de pago con la fecha de vencimiento a fin de calcular la fecha de registro. Una vez haya liquidado movimientos de proveedor, puede usar la acción **Calcular fecha de registro**. La fecha de registro en la línea del diario ahora se actualiza con la fecha de vencimiento de la factura de compra relacionada. Para obtener más información, consulte [Procedimiento: Liquidar transacciones de compra manualmente](payables-how-apply-purchase-transactions-manually.md).  

**Nota**: Si la factura de compra tiene fecha vencida, la fecha de registro se establecerá en la fecha de trabajo, y la fuente de la línea cambiará a color rojo.

## <a name="see-also"></a>Consulte también
[Gestionar pagos](payables-manage-payables.md)  
[Realizar pagos](payables-make-payments.md)  
[Trabajar con diarios generales](ui-work-general-journals.md)

