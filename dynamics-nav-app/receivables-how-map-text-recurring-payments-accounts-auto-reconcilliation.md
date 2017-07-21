---
title: "Asignación de texto en pagos periódicos a cuentas para conciliación automática"
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
ms.openlocfilehash: 7f9bf8b0550f7da1cced995234e15ad7aab484ba
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Asignación de texto en pagos periódicos a cuentas para conciliación automática
En la ventana **Asignación de texto a cuenta**, que se abre desde la ventana **Diario de conciliación de pagos**, puede configurar asignaciones entre el texto de los pagos y las cuentas de débito, crédito y saldo específicas para que los pagos se registren en las cuentas específicas cuando registre el diario de conciliación de pagos.

**Nota**: El tema también se aplica a cuando utiliza la función **Asignar texto a cuenta** desde un registro de documento entrante para ayudar a convertir documentos electrónicos recibidos desde servicios externos a documentos en Dynamics NAV. Para obtener más información, vea [Procedimiento: Usar el servicio OCR para convertir archivos PDF y de imagen en documentos](across-how-use-ocr-pdf-images-files.md).   

La funcionalidad similar existe para conciliar el exceso de importes en las líneas del diario de conciliación de pagos sobre una base ad hoc. Para obtener más información, vea [Procedimiento: Conciliar pagos que no pueden liquidarse automáticamente](receivables-how-reconcile-payments-cannot-apply-auto.md).

Los pagos registrados según la asignación de texto a cuenta no se aplican a movimientos pendientes, sino que simplemente se registran en las cuentas especificadas además de crear movimientos de bancos. Por consiguiente, la asignación de texto a cuenta es adecuada para recepciones de efectivo o gastos periódicos, como las compras frecuentes de combustible para vehículos o los honorarios bancarios e intereses que se producen normalmente en el estado de cuenta bancario y no necesitan un documento comercial relacionado. Para más información, consulte la sección "Ejemplo: Asignación de texto a cuenta para gasto de combustible" de este tema.

**Nota**: Los pagos en las líneas del diario de conciliación solo están configuradas para el registro según la asignación de texto a cuenta si la función de liquidación automática únicamente puede proporcionar una confianza de coincidencia de tipo **Baja** o **Media**. Si la función de liquidación automática proporciona confianza de la coincidencia Alta, el pago se liquida automáticamente en uno o varios movimientos pendientes y no se contabiliza en las cuentas especificadas de la ventana **Asignación de texto a cuenta**. En otras palabras, una confianza de coincidencia **Alta** invalida el mapeo de texto a cuenta.

En una línea del diario de conciliación de pagos en la que el pago se estableció en contabilizarse según la asignación de texto a cuenta, el campo **Confianza de la coincidencia** contiene **Alta: asignación de texto a cuenta** y los campos **Tipo de cta.** y **N.º de cuenta**. contienen las cuentas asociadas.

## <a name="to-map-text-on-recurring-payments-to-accounts-for-automatic-reconciliation"></a>Para asignar texto en pagos periódicos a cuentas para conciliación automática
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de conciliación de pagos** y, a continuación, seleccione el enlace relacionado.
2. Abra un diario de conciliación de pagos. Para obtener más información, vea [Procedimiento: Conciliar pagos con liquidación automática](receivables-how-reconcile-payments-auto-application.md).
3. Seleccione la acción **Asociar texto a cuenta**. Se abre la ventana **Asignación de texto a cuenta**.
4. En el campo **Texto de asignación**, introduzca cualquier texto de los pagos que quiera registrar en unas cuentas específicas sin aplicarlo a un movimiento pendiente. Puede escribir hasta 50 caracteres.

    **Nota**: Si no existen otros pagos o documentos entrantes con la asignación de texto en cuestión, la asignación tendrá lugar incluso cuando solo una parte del texto en el pago o el documento entrante exista como texto de asignación.
5. En el campo **N.º proveedor**, introduzca el proveedor para el que se crearán documentos entrantes que contienen texto de asignación o se registrarán dichos documentos. Para obtener más información, vea [Procedimiento: Usar el servicio OCR para convertir archivos PDF y de imagen en documentos](across-how-use-ocr-pdf-images-files.md).      
6. En el campo **N.º cta. débito**, introduce la cuenta a la que se contabilizarán los pagos con texto de asignación en caso de haber pagos entrantes. Para los pagos entrantes, el signo del valor en el campo **Importe estado de cuenta** es positivo.
7. En el campo **N.º cta. crédito**, introduce la cuenta a la que se contabilizarán los pagos con texto de asignación en caso de haber pagos salientes. Para los pagos salientes, el signo del valor en el campo **Importe estado de cuenta** es negativo.
8. En el campo **Tipo origen contr.**, especifique si el pago se contabilizará en una cuenta contable o en una cuenta de cliente o proveedor.
9. En el campo **N.º origen contr.**, especifique la cuenta a la que se contabilizará el pago dependiendo de su elección en el campo **Tipo origen contr**.
10. Repita los pasos del 4 al 8 para todo el texto de los pagos que desea asignar a las cuentas para el registro directo sin liquidación.

La próxima vez que importe un archivo de estado de cuenta bancario o seleccione la función **Liquidar automáticamente** de la ventana **Diario de conciliación de pagos**, las líneas del diario de pagos que contienen el texto de asignación especificado incluirán las cuentas asignadas en **Tipo de cuenta** y **N.º cuenta**. . El campo **Confianza de la coincidencia** contendrá **Alta: asignación de texto a cuenta**. Esto es así siempre que la función de liquidación automática solo pueda proporcionar una confianza de correspondencia **Baja** o **Media**.

##<a name="example-text-to-account-mapping-for-fuel-expense"></a>Ejemplo: Asignación de texto a cuenta para gasto de combustible

Para que los gastos de combustible de las gasolineras Shell siempre se contabilicen en la cuenta contable para la gasolina (cuenta 8510), rellene una línea en la ventana **Asignación de texto a cuenta** como se indica a continuación.

|Asignación de texto |Cta. débito N.º |Cta. crédito N.º |Contrap. Tipo procedencia mov. |Contrap. N.º origen |
|-------------|---------------|----------------|-----------------|----------------|
|Shell |EN BLANCO |8510 |Cuenta|EN BLANCO|

**Sugerencia**: Para obtener más información sobre cómo usar campos y columnas, consulte [Trabajar con Dynamics NAV](ui-work-product.md). Para obtener más información sobre la búsqueda de páginas específicas, consulte [Buscar](ui-search.md).

## <a name="see-also"></a>Consulte también
[Gestionar cobros](receivables-manage-receivables.md)  
[Gestionar ventas](sales-manage-sales.md)  
[Configuración del servicio de fuentes de banco de Envestnet Yodlee](bank-how-setup-bank-statement-service.md)  
[Personalizar Dynamics NAV usando extensiones](ui-extensions.md)

