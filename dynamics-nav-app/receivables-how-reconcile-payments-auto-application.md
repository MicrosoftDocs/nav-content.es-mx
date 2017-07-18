---
title: "Conciliar pagos con liquidación automática"
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
ms.openlocfilehash: bde263424bb8e5b60d2c9a139ddc8bfef0a90062
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-reconcile-payments-using-automatic-application"></a>Conciliar pagos con liquidación automática
La ventana **Diario de conciliación de pagos** especifica pagos, bien entrantes de clientes o salientes a proveedores, que se han registrado como transacciones en la cuenta bancaria en línea y que puede liquidar a sus clientes, vendedores y movimientos de la cuenta pendientes. Las líneas del diario se rellenan importando un estado de cuenta bancario como una fuente o un archivo de banco.

Un diario de conciliación de pago está relacionado con una cuenta bancaria en Dynamics NAV que refleja la cuenta bancaria en línea donde se registran las transacciones de pago. Todos los movimientos de banco pendientes relacionados con los movimientos de cliente o proveedor se cerrarán cuando seleccione la acción **Registrar pagos y conciliar banco**. Eso significa que la cuenta bancaria se concilia automáticamente por los pagos que registró mediante el diario.

Si desea importar tanto extractos bancarios como la fuente de banco, primero debe configurar y habilitar el servicio de fuentes de banco de Envestnet Yodlee y, a continuación, vincular la cuenta bancaria a la cuentas bancaria en línea relacionada. El diario de conciliación de pagos detectará automáticamente las fuentes de banco cuando seleccione la acción **Importar transacciones de banco**. Además, puede configurar una cuenta bancaria para que importe nuevas fuentes de estados de cuenta bancarios cada hora. No se importarán las transacciones para los pagos que ya se hayan registrado como liquidados o conciliados. Para obtener más información, vea [Procedimiento: Configuración del servicio de fuentes de banco de Envestnet Yodlee](bank-how-setup-bank-statement-service.md)

**Nota**: es posible que el servicio Fuentes de banco de Envestnet Yodlee, o el servicio fuentes de banco de otro proveedor, no esté disponible en su sistema. Póngase en contacto con su socio de Microsoft si desea usar un servicio de fuentes de banco para importar extractos bancarios.

Con la acción **Asignar texto a cuenta** puede configurar asignaciones entre el texto de los pagos y la cuentas de débito, crédito y saldo específicas para que los pagos se contabilicen en las cuentas específicas cuando contabilices el diario de conciliación de pagos. Consulte el paso 9. Para más información, consulte [Procedimiento: Asignación de texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).

La funcionalidad similar existe para conciliar el exceso de importes en las líneas del diario de conciliación de pagos sobre una base ad hoc. Para obtener más información, vea [Procedimiento: Conciliar pagos que no pueden liquidarse.](receivables-how-reconcile-payments-cannot-apply-auto.md)

La función **Liquidar automáticamente** se usa automáticamente cuando se importa una fuente o un archivo bancario con transacciones de pago o cuando se activa para liquidar pagos en sus movimientos pendientes relacionados basándose en una coincidencia de datos en una línea del diario con datos en uno o varios movimientos pendientes.

En las líneas del diario donde un pago se ha liquidado automáticamente en uno o varios movimientos pendientes, el campo **Confianza de la coincidencia** tiene un valor entre Bajo y Alto para indicar la calidad de la coincidencia de datos en la que se basa la liquidación de pago sugerida. Además, los campos **Tipo cta.** y **N.º cuenta** se rellenan con información sobre el cliente o el proveedor para el que se liquidó el pago. Si ha configurado una asignación de texto a cuenta, la liquidación automática puede dar como resultado un valor de confianza de la coincidencia **Alta: asignación de texto a cuenta**.

Para cada línea del diario en la ventana **Diario de conciliación de pagos**, puede abrir la ventana **Liquidación de pago** para ver todos los movimientos pendientes que son candidatos para el pago y puede ver información detallada para cada movimiento sobre la coincidencia de datos en la que se basa la liquidación de un pago. Aquí puede liquidar manualmente pagos o volver a liquidar pagos que se liquidaron de forma automática en un movimiento incorrecto. Para obtener más información, vea [Procedimiento: Revisar o liquidar pagos después de una liquidación automática](receivables-how-review-apply-payments-auto-application.md).

**Nota**: Puede iniciar la importación de las transacciones bancarias al mismo tiempo que abre la ventana **Conciliación de pagos** para un diario de conciliación de pagos existente en la ventana **Diarios de conciliación de pago**. El procedimiento siguiente describe cómo importar transacciones bancarias a la ventana **Diario de conciliación de pagos** una vez creado un nuevo diario.

## <a name="to-reconcile-payments-using-automatic-application"></a>Para conciliar los pagos con liquidación automática
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de conciliación de pagos** y, a continuación, seleccione el enlace relacionado.
2. Para trabajar en un nuevo diario de conciliación de pago, seleccione la acción **Nuevo diario**.
3. En la ventana **Lista cuentas bancarias pago**, seleccione la cuenta bancaria que desee conciliar los pagos y, a continuación, haga clic en **Aceptar**.
La ventana **Diario de conciliación de pagos** abre una ventana preparada para la cuenta bancaria seleccionada.
4. Seleccione la acción **Importar transacciones bancarias**.
Si la cuenta bancaria del diario seleccionado no está configurada para el importe de transacciones bancarias, se abrirá un cuadro de diálogo para ayudarle a rellenar los campos pertinentes.
5. En la ventana **Seleccionar un archivo para importarlo**, seleccione el archivo que contiene las transacciones bancarias para los pagos que desee conciliar y, a continuación, haga clic en **Abrir**.  
6. Si se ha habilitado el servicio Estado de cuenta bancario, en la ventana **Filtro de estado de cuenta bancario** que se abre automáticamente, especifique el intervalo de fechas para que se importen los estados de cuenta bancarios.

    La ventana **Diario de conciliación de pagos** se rellena con líneas para pagos que representan transacciones bancarias en el estado de cuenta bancario importado.

    En las líneas de los pagos que se han liquidado automáticamente en sus movimientos pendientes relacionados, el campo **Confianza de la coincidencia** tiene un valor entre **Bajo** y **Alto** para indicar la calidad de la coincidencia de datos en la que se basa la liquidación de pago sugerida. Además, los campos **Tipo cta.** y **N.º cuenta** se rellenan con información sobre el cliente o el proveedor para el que se liquidó el pago.
7. Seleccione una línea de diario y, a continuación, seleccione la acción **Liquidar manualmente** para revisar, volver a liquidar o liquidar el pago manualmente en la ventana **Liquidación de pago**. Para obtener más información, vea [Procedimiento: Revisar o liquidar pagos después de una liquidación automática](receivables-how-review-apply-payments-auto-application.md).

    Cuando termine la liquidación manual, el campo **Confianza de la correspondencia** en la línea de diario que ha procesado manualmente contendrá la palabra **Aceptado**.
8. Seleccione una línea del diario desliquidado para una recepción de efectivo o un gasto periódicos, como el de repostar gasolina y, a continuación, en la pestaña Inicio, en el grupo Revisar, seleccione Asignar texto a cuenta. Para más información, consulte [Procedimiento: Asignación de texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)
9. Cuando haya terminado con la asignación de texto de pago a las cuentas, seleccione la acción **Liquidar manualmente**.
10. Si está seguro de que todos los pagos en las líneas del diario se han liquidado correctamente, o se han establecido para un registro directo, elija la acción **Registrar**.

Cuando se registra el diario de conciliación de pagos, los créditos de movimientos pendientes aplicados se cierran y las cuentas de cliente, proveedor o contabilidad general relacionadas se actualizan. En el caso de los pagos en las líneas del diario basados en la asignación de texto a cuenta, se actualizan las cuentas de cliente, proveedor y contabilidad especificadas. Para todas las líneas de diario, se crean movimientos de banco. Si selecciona la acción **Registrar pagos y conciliar banco**, se cerrarán todos los movimientos de banco pendientes relacionados con los movimientos de los clientes o los proveedores. Eso significa que la cuenta bancaria se concilia automáticamente por los pagos que registró mediante el diario.

Puede comparar el valor del campo **Saldo en cuenta bancaria después del registro** con el valor del campo **Saldo final estado de cuenta** para hacer un seguimiento cuando la cuenta bancaria se concilie según los pagos registrados.

**Nota**: Si no desea conciliar la cuenta bancaria de la ventana **Diario de conciliación de pagos**, debe usar la ventana **Conciliación banco**. Para obtener más información, vea [Conciliar cuentas bancarias por separado](bank-how-reconcile-bank-accounts-separately.md).

## <a name="see-also"></a>Consulte también
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar ventas](sales-manage-sales.md)

