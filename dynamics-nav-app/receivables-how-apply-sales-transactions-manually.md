---
title: 'Procedimiento: Conciliar pagos de cliente manualmente'
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
ms.openlocfilehash: de0c94386ad5a0bbfba5cc0516fa7faa5cdcc0b4
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-customer-payments-manually"></a>Procedimiento: Conciliar pagos de cliente manualmente
Cuando cobra de un cliente o efectúa una recepción de efectivo, debe decidir si va a liquidar el pago o a reembolsarlo a uno o varios movimientos de crédito o débito pendientes. Puede especificar el importe exacto que desea liquidar. Por ejemplo, es posible que solo desee liquidar parte del pago, y así, liquidar solo parcialmente movimientos de cliente. En algún momento, es importante cerrar (liquidar) todos los movimientos de cliente para obtener estadísticas y copias impresas correctas de los estados de cuenta y los cargos financieros configurados de los clientes.

Puede liquidar movimientos de cliente de tres formas distintas:

- Al especificar información en ventanas específicas, como **Diario de recepciones de efectivo** y **Diario de conciliación de pagos**.
- Desde documentos de nota de crédito de venta.
- Movimientos de cliente después de que los documentos de ventas se registran pero no se liquidan.

**Nota**: Si el campo **Método liquidación** de la ficha cliente contiene **Liq. por antigüedad**, los pagos se liquidarán automáticamente en el movimiento de crédito pendiente más antiguo si no especifica manualmente en qué movimiento quiere liquidar. Si el método de liquidación para un cliente es **Manual**, entonces deberá liquidar los movimientos manualmente.

Puede liquidar pagos de cliente manualmente en la ventana **Diario de recepciones de efectivo**. Un diario de recepciones de efectivo es un tipo de diario general, por lo que puede usarlo para registrar transacciones en cuentas contables, de banco, cliente, proveedor y activos fijos. Puede liquidar el pago de uno o más movimientos de débito cuando registra el pago o puede liquidarlos desde movimientos registrados posteriormente.

También puede liquidar pagos de cliente y de proveedor, en la ventana **Diario de conciliación de pagos** mediante funciones para la importación de estados de cuenta bancarios, la liquidación automática y la conciliación de cuentas bancarias. Para obtener más información, vea [Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md). De forma alternativa, puede conciliar los pagos de clientes basados en una lista de documentos de ventas sin abonar en la ventana **Registro de pagos**. Para obtener más información, consulte [Procedimiento: Conciliar pagos de cliente desde una lista de documentos de ventas sin abonar](receivables-how-reconcile-customer-payments-list-unpaid-sales-documents.md).

## <a name="to-fill-and-post-a-cash-receipt-journal"></a>Para rellenar y registrar un diario de recepciones de efectivo
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario de recepciones de efectivo** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la sección de diario que le interese en el campo **Nombre sección**.
3. Rellene el campo **Fecha registro**.  
4. En el campo **Tipo documento**, seleccione **Pago**.

    El campo **N.º de documento** se rellena con la serie numérica asignada al proceso.
5. Use el campo **N.º de documento externo** para almacenar un identificador como el número de comprobación del cliente.
6. En el campo **Tipo mov.**, seleccione **Cliente**.
7. En el campo **N.º cuenta** seleccione la cuenta de contabilidad pertinente.
8. Si desea registrar la aplicación al mismo tiempo que el diario, elija una de estas acciones.
9. En el campo **Tipo contrapartida**, seleccione **Cuenta** para los pagos en efectivo y **Banco** para otros pagos.
10. En el campo **N.º de cuenta de saldo** seleccione la cuenta de efectivo para los pagos en efectivo, o la cuenta bancaria correspondiente para otros pagos.
11. Registre el diario.

## <a name="to-apply-a-payment-to-a-single-customer-ledger-entry"></a>Para liquidar un pago a un solo movimiento de cliente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario de recepciones de efectivo** y seleccione el enlace relacionado.
2. En la primera línea del diario, escriba la información correspondiente sobre el movimiento que se va a liquidar.
3. En el campo **Tipo documento**, introduzca **Pago**.
4. En el campo **Tipo mov.**, introduzca **Cliente**.
5. En el campo **Tipo contrapartida**, introduzca **Banco**.
6. En el campo **Liq. por n.º documento** seleccione el campo para abrir la ventana **Movs. pendientes cliente**.
7. En la ventana **Movs. pendientes cliente**, seleccione el movimiento al que quiere liquidar el pago.
8. En el campo **Importe a liquidar**, introduzca el importe con el que desea liquidar el movimiento. Si no especifica ningún importe, se usa el importe máximo.

    Al final de la ventana **Liquidar movs. cliente**, podrá ver el importe específico incluido en el campo **Importe liquidado** y también si la liquidación está cuadrada.
9. Elija el botón **Aceptar**. La ventana **Diario de recepciones de efectivo** ahora muestra el movimiento que ha especificado en **Liq. por tipo documento** y **Liq. por n.º documento**. .
10. Registre el diario de recepciones de efectivo.

## <a name="to-apply-a-payment-to-multiple-customer-ledger-entries"></a>Para liquidar un pago a varios movimientos de cliente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario de recepciones de efectivo** y seleccione el enlace relacionado.
2. En la primera línea del diario, escriba la información correspondiente sobre el movimiento que se va a liquidar.
3. En el campo **Tipo documento**, introduzca **Pago**.
4. En el campo **Tipo mov.**, introduzca **Cliente**.
5. En el campo **Tipo contrapartida**, introduzca **Banco**.
6. En el campo **Importe**, introduzca el pago completo como un importe negativo.
7. Para liquidar los pagos de varios movimientos de cliente cuando registre, seleccione la acción **Liquidar movs.**
8. Seleccione las líneas que incluyen los movimientos a los que desea aplicar el movimiento de liquidación y, a continuación, seleccione la acción **Marcar id. de liquidación**.
9. En cada línea del campo **Importe a liquidar**, introduzca el importe con el que desea liquidar cada movimiento. Si no especifica ningún importe, se usa el importe máximo.

    Al final de la ventana **Liquidar movs. cliente**, podrá ver el importe específico incluido en el campo **Importe liquidado** y también si la liquidación está cuadrada.
10. Elija el botón **Aceptar**.
11. Registre el diario de recepciones de efectivo.

## <a name="to-apply-a-credit-memo-to-a-single-customer-ledger-entry"></a>Para liquidar una nota de crédito a un único movimiento de cliente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Abonos de venta** y, a continuación, seleccione el enlace relacionado.
2. Abra la nota de crédito de venta correspondiente.
3. Para liquidar la nota de crédito en un solo movimiento de cliente cuando registre, en el campo **Liq. por n.º documento**, seleccione el movimiento que desea liquidar con el pago.
4. En la línea del campo **Importe a liquidar**, introduzca el importe con el que desea liquidar el movimiento.

    Si no especifica ninguna cantidad, el programa utilizará automáticamente el importe máximo. Al final de la ventana **Liquidar movs. cliente**, podrá ver el importe específico incluido en el campo **Importe liquidado** y también si la liquidación está cuadrada.
5. Elija el botón **Aceptar**. La ventana **Nota de crédito de venta** ahora muestra el movimiento que ha especificado en **Liq. por tipo documento** y **Liq. por n.º documento**. . Asimismo, muestra el importe de la nota de crédito que se va a registrar, ajustado con los posibles descuentos por pronto pago.
6. Registre la nota de crédito

## <a name="to-apply-a-credit-memo-to-multiple-customer-ledger-entries"></a>Para liquidar una nota de crédito a varios movimientos de cliente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Abonos de venta** y, a continuación, seleccione el enlace relacionado.
2. Abra la nota de crédito de venta correspondiente.
3. Para liquidar la nota de crédito en varios movimientos de cliente cuando registre, seleccione la acción **Liquidar movs**.
4. Seleccione las líneas que incluyen los movimientos a los que desea aplicar el movimiento de liquidación y, a continuación, seleccione la acción **Marcar id. de liquidación**.
5. En cada línea del campo **Importe a liquidar**, introduzca el importe con el que desea liquidar cada movimiento. Si no especifica ningún importe, se usa el importe máximo.

  Al final de la ventana **Liquidar movs. cliente**, podrá ver el importe específico incluido en el campo **Importe liquidado** y también si la liquidación está cuadrada.
6. Elija el botón **Aceptar**. La ventana **Nota de crédito de venta** ahora muestra el importe de la nota de crédito que se va a registrar, ajustado para los posibles descuentos por pronto pago.
7. Registre la nota de crédito

## <a name="to-apply-posted-customer-ledger-entries"></a>Para liquidar movimientos de clientes registrados
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Clientes** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de cliente para el cliente con los movimientos que desea liquidar.
3. Elija la acción **Movimientos** y, a continuación, seleccione la línea con el movimiento que se liquidará.
4. Seleccione la acción **Liquidar movs.**. La **Liquidar movs. cliente** se abre y muestra los movimientos pendientes del cliente.
5. Seleccione las líneas con los movimientos que desea aplicar el movimiento de liquidación y, a continuación, seleccione la acción **Marcar id. de liquidación** .
6. En cada línea del campo **Importe a liquidar**, introduzca el importe con el que desea liquidar cada movimiento. Si no especifica ningún importe, se usa el importe máximo.

    En la parte inferior de la ventana **Liquidar movs. cliente**, puede ver el importe específico en el campo **Importe liquidado**.
7. Seleccione la acción **Registrar liquidación marcada**. La ventana **Registrar liquidación** aparece con el número de documento del movimiento de liquidación y la fecha de registro del movimiento con la fecha más reciente.  
8. Para registrar la liquidación, elija el botón **Aceptar**.

    Si la liquidación registrada obtiene como resultado movimientos cerrados de cliente, se desactivará el campo **Pendiente** para dichos movimientos.
9. Para ver los movimientos, en la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Clientes** y, a continuación, seleccione el enlace relacionado. Busque la ficha del cliente correspondiente para ver los movimientos.

En la lista de movimientos, en la línea que contiene el movimiento que se liquidó completamente, puede ver que la casilla **Pendiente** no está marcada.  

**Nota**: Después de haber seleccionado un movimiento en la ventana **Liquidar movs. cliente** o varios movimientos estableciendo la opción **Liq. por id.**, el campo **Importe liquidado** de la línea del diario contendrá la suma de los importes restantes de los movimientos registrados que haya seleccionado, a menos que el campo ya contenga algún valor. Si selecciona **Liq. por antigüedad** en el campo **Método de liquidación** de la ficha de cliente, la liquidación se realizará automáticamente.

## <a name="to-apply-customer-ledger-entries-in-different-currencies-to-one-another"></a>Para liquidar movimientos de cliente en divisas diferentes
Si vende a un cliente en una divisa y cobra en otra, aún puede liquidar la factura con el pago.

Si con un movimiento (Movimiento 1) en una divisa liquida otro movimiento (Movimiento 2) en otra divisa, se usa la fecha de registro del Movimiento 1 para buscar el tipo de cambio adecuado para convertir los importes del Movimiento 2. El tipo de cambio relevante se encuentra en la ventana **Tipos cambio divisa**.

Se debe habilitar la liquidación de movimientos de cliente en divisas diferentes. Para obtener más información vea, [Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas](finance-setup-how-enable-application-ledger-entries-different-currencies.md).

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario de cobros** y seleccione el enlace relacionado.
2. Abra el diario que desea y rellene la primera línea de diario vacía utilizando un código de divisa.
3. Seleccione la acción **Liquidar movs.**.
4. Seleccione la línea que contiene el movimiento con el que desea liquidar el movimiento del diario de recepciones de efectivo, elija la acción **Marcar id. de liquidación** y, a continuación, seleccione el movimiento que desea liquidar.
5. Seleccione el botón **Aceptar** para volver al diario de recepciones de efectivo.
6. Registre el diario de ventas.

**Importante**: Si liquida movimientos en distintas divisas, los movimientos se convierten a divisa local. Aunque los tipos de cambio de las dos divisas son fijos, como entre USD y EUR, es posible que exista un pequeño importe residual al convertir los importes de divisa extranjera a USD. Estos importes residuales mínimos se registran como ganancias y pérdidas en la cuenta especificada en el campo **Cta. dif. pos. realizadas** o **Cta. dif. neg. realizadas** de la ventana **Divisas**. El campo **Importe (USD)** también se ajusta para los movimientos de proveedor correspondientes.

## <a name="to-unapply-an-application-of-customer-entries"></a>Para deshacer una liquidación de movimientos de clientes
Cuando se deshace una liquidación errónea, se crean y registran movimientos de corrección que son idénticos al original, pero de signo opuesto en el campo de importe, para todos los movimientos, incluidos todos los registros de contabilidad derivados de la liquidación, como los descuentos por pronto pago y las pérdidas y ganancias en divisas. Los movimientos que se cerraron con la liquidación se volverán a abrir.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Clientes** y, a continuación, seleccione el enlace relacionado.
2. Abrir la ficha de cliente correspondiente.
3. Seleccione la acción **Movimientos**.
4. Seleccione el movimiento relevante y, a continuación, seleccione la acción **Desliquidar entradas**.
5. De forma alternativa, seleccione la acción **Movimiento detallado**.
6. Seleccione el movimiento de liquidación relevante y, a continuación, seleccione la acción **Desliquidar entradas**.
7. Rellene los campos de la cabecera y, a continuación, seleccione la acción **Desliquidar**.

**Importante**: Si se ha liquidado un movimiento con más de un movimiento de liquidación, primero deberá deshacer la liquidación más reciente.

## <a name="see-also"></a>Consulte también
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar ventas](sales-manage-sales.md)

