---
title: "Procedimiento: Revisar o liquidar pagos manualmente después de una liquidación automática"
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
ms.openlocfilehash: 556a0f74a7407d247008e2d74420803123056eff
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-review-or-apply-payments-manually-after-automatic-application"></a>Procedimiento: Revisar o liquidar pagos manualmente después de una liquidación automática
Para cada línea del diario que representa un pago en la ventana **Diario de conciliación de pagos**, puede abrir la ventana **Liquidación de pago** para ver todos los movimientos pendientes que son candidatos para el pago y puede ver información detallada para cada movimiento sobre la coincidencia de datos en la que se basa la liquidación de un pago. Aquí puede liquidar manualmente pagos o volver a liquidar pagos que se liquidaron de forma automática en un movimiento incorrecto. Para obtener más información acerca de la liquidación automática, vea [Procedimiento: Conciliar pagos usando la liquidación automática](receivables-how-reconcile-payments-auto-application.md).

**Importante**: Cuando la cuenta bancaria para la que se están conciliando pagos está configurada para la divisa local, la ventana **Liquidación de pago** mostrará todos los movimientos pendientes en la divisa local, incluidos los movimientos pendientes para documentos facturados originalmente en divisas extranjeras. Por tanto, los pagos liquidados en movimientos con divisas convertidas se pueden registrar con importes distintos al del documento original, ya que puede que el banco y Dynamics NAV usen tipos de cambio potencialmente diferentes.

Por tanto, es recomendable buscar los códigos de divisas extranjeras en el campo **Código de divisa** de la ventana **Liquidación de pago** para comprobar si las liquidaciones se basan en divisas convertidas. Para revisar el importe del documento original en la divisa extranjera y ver el tipo de cambio usado, seleccione el campo **Liq. por n.º mov.** y, a continuación, en el menú contextual seleccione el botón análisis para abrir la ventana de **Movs. cliente** o **Movs. proveedor**.

Dynamics NAV no gestiona automáticamente los ajustes de ganancia y pérdida necesarios debido a las conversiones de la divisa.

**Nota**: No puede liquidar movimientos con signo diferente al signo en el pago. Por ejemplo, para cerrar una nota de crédito negativa y su factura positiva, primero deberá liquidar la nota de crédito para la factura y, a continuación, liquidar el pago para la factura con el importe pendiente reducido.

**Advertencia**: Si usa descuentos por pronto pago, y si la fecha de pago es anterior a la fecha de vencimiento del pago, el campo **Importe pendiente incl. descuento** de la ventana **Liquidación de pagos** se usará en la coincidencia. En caso contrario, se usará el valor del campo **Importe pendiente**. Si el pago se realizó con un importe de descuento después de la fecha de vencimiento del pago, o se pagó el importe completo pero se concedió un descuento, entonces el importe no coincidirá.

**Nota**: Puede liquidar solo un pago en una cuenta. Si desea dividir la liquidación en varios movimientos pendientes, por ejemplo para liquidar un pago de suma total, los movimientos pendientes deben serlo para la misma cuenta. Para obtener más información, consulte los pasos 7 y 8 del procedimiento de este tema.

## <a name="to-review-or-apply-payments-after-automatic-application"></a>Para revisar o aplicar pagos después de una liquidación automática
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de conciliación de pagos** y, a continuación, seleccione el enlace relacionado.
2. Abra el diario de conciliación de pagos de un banco para el que desee conciliar los pagos. Para obtener más información, vea [Procedimiento: Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).
3. En la ventana **Diario de conciliación de pagos**, seleccione un pago que desee revisar o liquidar manualmente a uno o varios movimientos pendientes y, a continuación, seleccione la acción **Liquidación manual**.
4. Active la casilla **Liquidado** en la línea correspondiente al movimiento pendiente en el que desea liquidar el pago.
5. El importe de pago, que también se mostrará en el campo **Importe de la transacción** en la ventana **Liquidación de pagos**, se inserta en el campo **Importe liquidado**; no obstante, puede modificar el campo, por ejemplo, si desea liquidar el importe en varios movimientos pendientes.
6. Para liquidar una parte del importe abonado a otro movimiento pendiente para la cuenta, por ejemplo, para liquidar un pago de suma total, active la casilla **Liquidado** de la línea. El importe liquidado se deduce automáticamente del importe de las transacciones para reflejar la distribución en los dos movimientos pendientes.
7. Para liquidar una parte de un pago a uno o varios movimientos pendientes que no existe en la base de datos, cree una línea nueva debajo de la línea para la misma cuenta. En el campo **Importe liquidado**, indique el importe pendiente de liquidar en la nueva línea y, a continuación, ajuste el campo **Importe liquidado** en la línea existente.
8. Repita el paso 5, 6 o 7 para otros movimientos pendientes en los que desee liquidar el importe de pago completa o parcialmente.
9. Cuando haya revisado una liquidación de pago o la haya liquidado manualmente en uno o varios movimientos pendientes, seleccione la acción **Aceptar liquidación**.

Se cierra la ventana **Liquidación de pagos** y, en la ventana **Diario de conciliación de pagos**, el valor del campo **Confianza de la coincidencia** cambia a **Aceptado** para indicarle que ha revisado o ha liquidado manualmente el pago.

## <a name="see-also"></a>Consulte también
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar ventas](sales-manage-sales.md)

