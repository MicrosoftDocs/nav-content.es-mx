---
title: 'Procedimiento: Liquidar pagos a proveedores manualmente'
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
ms.openlocfilehash: d3aaafc9ac3dcfd1fba3802b1158bde890e09110
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-apply-vendor-payments-manually"></a>Procedimiento: Liquidar pagos a proveedores manualmente

Cuando envía un pago o recibe un reembolso de un proveedor, debe decidir si va a liquidar uno o varios movimientos pendientes con el pago o el reembolso. Puede especificar el importe exacto que desea liquidar con la recepción de pago o el reembolso, y liquidar sólo parcialmente movimientos del proveedor. Debe liquidar todos los movimientos de proveedores para obtener estadísticas e informes correctos de los extractos de cuentas y la configuración de los intereses.

**Nota**: A veces los proveedores pueden ofrecer reembolsos en lugar de notas de crédito para compensar futuras facturas, especialmente en los casos en que devuelven productos por los que ya han pagado o si han pagado de más en una factura.

Puede liquidar los movimientos de proveedor de tres formas distintas:

- Introduciendo información en ventanas específicas, como de **Diario de pagos** y **Diario de conciliación de pagos**.
- Desde documentos de nota de crédito de compra.
- Movimientos de proveedor después de que se registran los documentos de compras, pero no se liquidan.

**Nota**: Si el campo **Método liquidación** de la ficha de proveedor contiene **Liq. por antigüedad**, los pagos se liquidarán automáticamente en el movimiento de crédito pendiente más antiguo si no especifica manualmente en qué movimiento quiere liquidar. Si el método de liquidación para un cliente es **Manual**, entonces deberá liquidar los movimientos manualmente.

Puede liquidar pagos a proveedores manualmente a los documentos de compra relacionados cuando registre pagos en la ventana de **Diario de pagos**. Para obtener más información acerca del rellenar el diario de pagos, vea [Procedimiento: Efectuar pagos](payables-make-payments.md).

También puede liquidar los pagos a proveedores y los pagos a clientes, después los pagos aparecen como transacciones negativas en su banco. En la ventana **Diario de conciliación de pagos**, puede usar las funciones para importar estados de cuenta bancarios, para la liquidación automática y para la conciliación de cuentas bancarias. Para obtener más información, vea [Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).

## <a name="to-apply-a-payment-to-a-single-or-multiple-vendor-ledger-entries"></a>Para liquidar uno o varios movimientos del proveedor con un pago:
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario de pagos** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Diario de pagos**, en la primera línea del diario, escriba la información correspondiente sobre el movimiento de pago.
3. Para liquidar un solo movimiento de proveedor:
4. En el campo **Liq. por n.º documento** elija el campo para abrir la ventana **Movs. pendientes proveedor**.
5. En la ventana **Movs. pendientes proveedor**, seleccione el movimiento al que quiere liquidar el pago.
6. En la línea del campo **Importe pendiente de liquidar**, introduzca el importe para liquidar el movimiento.
7. O para liquidar múltiples movimientos de proveedor:
8. Seleccione la acción **Liquidar movs.**.
9. En la ventana **Movs. pendientes proveedor**, seleccione las líneas con los movimientos para liquidar con el pago.
10. Seleccione la acción **Marcar id. de liquidación**.  
11. En cada línea del campo **Importe pendiente de liquidar**, introduzca el importe para liquidar cada movimiento.

    Si no especifica ningún importe, se utiliza automáticamente el importe máximo. Al final de la ventana **Aplicar movs. proveedor**, podrá ver el importe específico incluido en el campo Importe liquidado y también si la liquidación está cuadrada.
12. Elija el botón **Aceptar**.
13. Seleccione la acción **Registrar**, para registrar el diario de pagos.

## <a name="to-apply-a-credit-memo-to-a-single-or-multiple-vendor-ledger-entries"></a>Para liquidar una nota de crédito con uno o varios movimientos de proveedor
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Nota de crédito compra** y, a continuación, elija el enlace relacionado.
2. Abra la nota de crédito que desea liquidar.
3. Escriba la información relevante en la cabecera.
4. Para liquidar un solo movimiento de proveedor:
5. En la ficha desplegable **Liquidación**, en el campo **Liq. por n.º documento**, seleccione el movimiento para liquidar el abono.
6. En la línea del campo **Importe pendiente de liquidar**, introduzca el importe para liquidar el movimiento.
7. O para liquidar múltiples movimientos de proveedor:
8. Seleccione la acción **Liquidar movs.**.
9. Seleccione las líneas que contienen los movimientos para liquidar la nota de crédito.
10. Seleccione la acción **Marcar id. de liquidación**.  
11. En cada línea del campo **Importe pendiente de liquidar**, introduzca el importe para liquidar cada movimiento.

    Si no especifica ningún importe, se utiliza automáticamente el importe máximo. Al final de la ventana **Aplicar movs. proveedor**, podrá ver el importe específico incluido en el campo **Importe liquidado** y también si la liquidación está cuadrada.
12. Elija el botón **Aceptar**.  
La ventana **Nota de crédito compra** muestra el movimiento que ha especificado en **Liq. por tipo documento** y **Liq. por n.º documento**. . La ventana también muestra el importe de la nota de crédito para registrar, ajustado con los descuentos por pronto pago.
13. Seleccione el botón **Registrar** para crear la nota de crédito compra.

## <a name="to-apply-posted-vendor-ledger-entries"></a>Para liquidar movimientos de proveedor registrados

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proveedores** y, a continuación, seleccione el enlace relacionado.
2. Abra el proveedor pertinente con movimientos ya registrados.
3. Seleccione la acción **Movimientos** y, a continuación, seleccione la acción **Liquidar movs**.
4. En la ventana **Movs. pendientes proveedor** podrá ver los movimientos pendientes del proveedor.
5. Seleccione la línea con el movimiento que se liquidará.
6. Seleccione la acción **Marcar id. de liquidación**.
7. El campo **Liq. por id.** muestra tres asteriscos si trabaja con un sistema de usuario único o su identificador de usuario si trabaja con un sistema multiusuario.  
8. Para cada línea del campo **Importe a liquidar** introduzca el importe para liquidar cada movimiento.

    Si no especifica ningún importe, se utiliza automáticamente el importe máximo. Puede ver el importe en el campo **Importe liquidado** en la parte inferior de la ventana **Aplicar movs. proveedor**.
9. Seleccione la acción **Registrar liquidación marcada**.  
La ventana **Registrar liquidación marcada** se abre con el número de documento del movimiento de liquidación y la fecha de registro del movimiento que la tenga más reciente.
10. Para registrar la liquidación, elija el botón **Aceptar**.

## <a name="to-apply-vendor-ledger-entries-in-different-currencies-to-one-another"></a>Para liquidar movimientos de proveedor entre divisas distintas
Si se realiza una venta a un proveedor en una divisa y se efectúa el pago en otra divisa, todavía se puede solicitar la factura para el pago.

Si con un movimiento (Movimiento 1) en una divisa liquida otro movimiento (Movimiento 2) en otra divisa, se usa la fecha de registro del Movimiento 1 para buscar el tipo de cambio adecuado para convertir los importes del Movimiento 2. El tipo de cambio relevante se encuentra en la ventana **Tipos cambio divisa**.

Se debe habilitar la liquidación de movimientos de proveedor en divisas diferentes. Para obtener más información vea, [Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas](finance-setup-how-enable-application-ledger-entries-different-currencies.md)

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario de pago** y, seleccione el enlace relacionado.
2. Abra el diario que desea y rellene la primera línea de diario vacía utilizando un código de divisa.
3. Seleccione la acción **Liquidar movs.**.
4. Seleccione la línea que contiene el movimiento con el que desea liquidar el movimiento del diario de pagos, seleccione la acción **Marcar id. de liquidación** y, a continuación, seleccione el movimiento que desea liquidar.
5. Elija el botón **Aceptar** para volver al diario de pagos.
6. Registre el diario de pagos.

**Importante**: Si liquida movimientos en distintas divisas, los movimientos se convierten a divisa local. Aunque los tipos de cambio de las dos divisas son fijos, como entre USD y EUR, es posible que exista un pequeño importe residual al convertir los importes de divisa extranjera a USD. Estos importes residuales mínimos se registran como ganancias y pérdidas en la cuenta especificada en el campo **Cta. dif. pos. realizadas** o **Cta. dif. neg. realizadas** de la ventana **Divisas**. El campo **Importe (USD)** también se ajusta para los movimientos de proveedor correspondientes.

## <a name="to-unapply-an-application-of-vendor-entries"></a>Para deshacer un movimiento de liquidación de movimientos de proveedor
Cuando se deshace una liquidación errónea, se crean y registran movimientos de corrección que son idénticos al original, pero de signo opuesto en el campo de importe, para todos los movimientos, incluidos todos los registros de contabilidad derivados de la liquidación, como los descuentos por pronto pago y las pérdidas y ganancias en divisas. Los movimientos que se cerraron con la liquidación se volverán a abrir.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proveedores** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de proveedor correspondiente.
3. Seleccione la acción **Movimientos**.
4. Seleccione el movimiento relevante y, a continuación, seleccione la acción **Desliquidar entradas**.
5. De forma alternativa, seleccione la acción **Movimiento detallado**.
6. Seleccione el movimiento de liquidación relevante y, a continuación, seleccione la acción **Desliquidar entradas**.
7. Rellene los campos de la cabecera y, a continuación, seleccione la acción **Desliquidar**.

**Importante**: Si se ha liquidado un movimiento con más de un movimiento de liquidación, primero deberá deshacer la liquidación más reciente.

## <a name="see-also"></a>Consulte también
[Pagos](payables-manage-payables.md)  
[Gestionar compras](purchasing-manage-purchasing.md)

