---
title: "Configurar la asignación de texto a cuenta para pagos periódicos | Documentos de Microsoft"
description: "Puede vincular el texto de los pagos con cuentas específicas, de modo que los pagos se registren en las cuentas al registrar el diario de conciliación de pagos."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account linking, direct payment posting, automatic payment processing, reconcile payment, recurring expense, recurring cash receipt
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 284dcac805ef34b433b4cb18499d47249dc8d01b
ms.contentlocale: es-mx
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Asignación de texto en pagos periódicos a cuentas para conciliación automática
En la ventana **Asignación de texto a cuenta**, que se abre desde la ventana **Diario de conciliación de pagos**, puede configurar asignaciones entre el texto de los pagos y las cuentas de débito, crédito y saldo específicas para que los pagos se registren en las cuentas específicas cuando registre el diario de conciliación de pagos.

La funcionalidad similar existe para conciliar el exceso de importes en las líneas del diario de conciliación de pagos sobre una base ad hoc. Para obtener más información, vea [Procedimiento: Conciliar pagos que no pueden liquidarse automáticamente](receivables-how-reconcile-payments-cannot-apply-auto.md).

Los pagos registrados según la asignación de texto a cuenta no se aplican a movimientos pendientes, sino que simplemente se registran en las cuentas especificadas además de crear movimientos de bancos. Por consiguiente, la asignación de texto a cuenta es adecuada para recepciones de efectivo o gastos periódicos, como las compras frecuentes de combustible para vehículos o los honorarios bancarios e intereses que se producen normalmente en el estado de cuenta bancario y no necesitan un documento comercial relacionado. Para más información, consulte la sección "Ejemplo: Asignación de texto a cuenta para gasto de combustible" de este tema.

> [!NOTE]  
>   Los pagos en las líneas de diario de conciliación solo están configuradas para el registro según el mapeo de texto a cuenta si la función de liquidación automática únicamente puede proporcionar una confianza de coincidencia de **Baja** o **Media**. Si la función de liquidación automática proporciona confianza de la coincidencia Alta, el pago se liquida automáticamente en uno o varios movimientos pendientes y no se contabiliza en las cuentas especificadas de la ventana **Asignación de texto a cuenta**. En otras palabras, una confianza de coincidencia **Alta** invalida el mapeo de texto a cuenta.

En una línea del diario de conciliación de pagos en la que el pago se estableció en contabilizarse según la asignación de texto a cuenta, el campo **Confianza de la coincidencia** contiene **Alta: asignación de texto a cuentas** y los campos **Tipo de cuenta** y **N.º de cuenta** contienen las cuentas asociadas.

## <a name="to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Para asignar texto en pagos periódicos a cuentas para conciliación automática
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios de conciliación de pagos** y, a continuación, seleccione el vínculo relacionado.
2. Abra un diario de conciliación de pagos. Para obtener más información, vea [Procedimiento: Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).
3. Seleccione la acción **Asociar texto a cuenta**. Se abre la ventana **Asignación de texto a cuenta**.
4. En el campo **Texto de asignación**, introduzca cualquier texto de los pagos que quiera registrar en unas cuentas específicas sin aplicarlo a un movimiento pendiente. Puede escribir hasta 50 caracteres.

    > [!NOTE]  
>   Si no existen otros pagos con la asignación de texto en cuestión, la asignación tendrá lugar incluso cuando solo una parte del texto del pago exista como texto asignado.
5. En el campo **Nº proveedor**, escriba el proveedor al que se enviarán los pagos.
6. En el campo **Tipo origen contr.**, especifique si el pago se contabilizará en una cuenta contable o en una cuenta de cliente o proveedor.
7. En el campo **N.º origen contr.** especifique la cuenta a la que se contabilizará el pago dependiendo de su elección en el campo **Tipo origen contr.**

    > [!NOTE]
    > No utilice los campos **N.º cta. débito** y **N.º cta. crédito** en relación con la conciliación de pagos. Se utilizan solo para los documentos entrantes. Para obtener más información, vea [Procedimiento: Usar el servicio OCR para convertir archivos PDF y de imagen en documentos](across-how-use-ocr-pdf-images-files.md).

8. Repita los pasos del 3 al 7 para todo el texto de los pagos que desea asignar a las cuentas para el registro directo sin liquidación.

La próxima vez que importe un archivo de un estado de cuenta de banco o seleccione la función **Liquidar automáticamente** de la ventana **Diario de conciliación de pagos**, las líneas de diario de los pagos que contienen el texto asignado especificado, incluirán las cuentas asignadas en los campos **Tipo de cuenta** y **N.º cuenta**. El campo **Confianza de la coincidencia** contendrá **Alta: asignación de texto a cuenta**. Esto es así siempre que la función de liquidación automática solo pueda proporcionar una confianza de correspondencia **Baja** o **Media**.

## <a name="example-text-to-account-mapping-for-fuel-expense"></a>Ejemplo: Asignación de texto a cuenta para gasto de combustible
Para que los gastos de combustible de las gasolineras Shell siempre se contabilicen en la cuenta contable para la gasolina (cuenta 8510), rellene una línea en la ventana **Asignación de texto a cuenta** como se indica a continuación.

| Asignación de texto | N.º cta. débito | N.º cta. crédito | Tipo origen contr. | N.º origen contr. |
| --- | --- | --- | --- | --- |
| Shell |EN BLANCO |8510 |Cuenta |EN BLANCO |

> [!TIP]  
>   Para obtener más información sobre cómo usar campos y columnas, consulte [Trabajar con [!INCLUDE[d365fin](includes/d365fin_long_md.md)]](ui-work-product.md). Para obtener más información sobre la búsqueda de páginas específicas, consulte [Buscar](ui-search.md).

## <a name="see-also"></a>Consulte también
[Administrar cobros](receivables-manage-receivables.md)  
[Ventas](sales-manage-sales.md)  
[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] usando extensiones](ui-extensions.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

