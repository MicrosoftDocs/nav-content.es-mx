---
title: 'Procedimiento: Trabajar con cheques'
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
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a>Procedimiento: Trabajar con cheques
Dynamics NAV admite la emisión de cheques electrónica y manual. Ambos métodos utilizan el diario de pagos para emitir los cheques a proveedores. También puede anular cheques y ver movimientos de cheques.

El proceso de emisión de cheques propone pagos, crea movimientos e imprime los cheques automáticos.

Su impresora tiene que haber configurado correctamente los documentos y usted deberá definir qué plantilla de cheques va a usar. Para obtener más información , vea [Procedimiento: Definir plantillas de cheques](finance-setup-how-define-check-layouts.md)

## <a name="to-issue-checks"></a>Para emitir cheques
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de pago** y, a continuación, seleccione el enlace relacionado.
2. Rellene el diario con los pagos relevantes, por ejemplo, mediante la función Proponer pagos a proveedores. Para obtener más información, vea [Procedimiento: Proponer pagos a proveedores](payables-how-suggest-vendor-payments.md).
3. En el campo **Tipo de pago bancario** en las líneas de diario para el pago que desea realizar mediante cheques, seleccione una de las opciones siguientes:

 - **Cheque automático**: Seleccione esta opción si desea imprimir un cheque por el importe de la línea del diario de pagos. Debe imprimir los cheques antes de que pueda registrar las líneas del diario. solo puede seleccionar **Cheque automático** si el valor de **Tipo contrapartida** o el de **Tipo mov.** es **Cuenta banco**.

 - **Cheque manual**: Seleccione esta opción si ha creado manualmente un cheque y desea crear el movimiento de cheque correspondiente a ese importe. Usando esta opción no puede imprimir cheques de Dynamics NAV. solo puede seleccionar **Cheque manual** si el valor de **Tipo contrapartida** o el de **Tipo mov.** es **Cuenta banco**.

    **Nota**: Debe imprimir los cheques automáticos antes de registrar las líneas del diario relacionadas.
4. En el caso de los cheques automáticos, seleccione **Imprimir cheque**.
5. En la ventana **Cheque**, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
6. Elija el botón **Imprimir**.

**Nota**: Si desea imprimir cheques en varias divisas de cuentas bancarias distintas, deberá ejecutar el proceso **Imprimir cheque** por separado para cada divisa y especificar la cuenta bancaria correspondiente.

## <a name="to-cancel-printed-checks-that-are-not-posted"></a>Para anular los cheques imprimidos que no han sido registrados
Puede anular los cheques no registrados después de que hayan sido imprimidos usando la acción **Anular cheque** de la ventana **Diario de pagos**.
1. En la ventana **Diario de pagos**, seleccione **Anular cheque** y, a continuación, seleccione que cheques desea cancelar.

## <a name="to-void-checks"></a>Para anular cheques
Cuando se ha registrado el pago del cheque, solo puede cancelar (anular) cheques en los movimientos resultantes del banco.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la cuenta bancaria correspondiente, seleccione la acción **Editar** y, a continuación, seleccione la acción **Movs. cheques**.
3. En la ventana **Movs. cheques**, seleccione la acción **Anular cheque**.
4. Active la casilla **Anular cheque sólo**.
5. Elija el botón **Aceptar**.

## <a name="see-also"></a>Consulte también
[Gestionar pagos](payables-manage-payables.md)  
[Configurar la banca](bank-setup-banking.md)  

