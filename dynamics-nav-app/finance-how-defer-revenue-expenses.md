---
title: Fraccionar ingresos y gastos
description: "Para reconocer ingresos y gastos en periodos distintos del periodo en el que se registró la transacción, puede fraccionarlos o posponerlos automáticamente según una previsión especificada."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: postpone
ms.date: 06/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f06d241d07bc613bb54cc0a278de419fafffbb58
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-defer-revenues-and-expenses"></a>Procedimiento: fraccionar ingresos y gastos
Para reconocer un ingreso o un gasto en un periodo distinto del periodo en el que se registró la transacción, puede usar la funcionalidad para fraccionar automáticamente ingresos y gastos según una previsión especificada.

Para distribuir los ingresos o los gastos de los periodos contables relacionados, debe configurar una plantilla de fraccionamiento para el recurso, el producto o la cuenta de contabilidad para el que se registrará el ingreso o el gasto. Cuando registre el documento de venta o de compra relacionado, los ingresos o los gastos se fraccionan en los periodos contables relacionados, según la previsión de fraccionamiento que controle la configuración de la plantilla de fraccionamiento y la fecha de registro.

## <a name="to-set-up-a-gl-account-for-deferral"></a>Para configurar una cuenta de contabilidad para el fraccionamiento
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plan de cuentas** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. Rellene los campos según sea necesario para crear una cuenta de contabilidad para los ingresos fraccionados. Para obtener más información, consulte [Contabilidad y catálogo de cuentas](finance-general-ledger.md).
4. Repita los pasos 2 y 3 para crear una nueva cuenta de contabilidad para los gastos fraccionados.

Para ambos tipos de fraccionamiento seleccione **Balance** en el campo **Tipo** y asigne un nombre adecuado a las cuentas, por ejemplo "Ingresos anticipados" en el caso de los ingresos fraccionados y "Gastos no pagados" en el caso de los gastos fraccionados.

## <a name="to-set-up-a-deferral-template"></a>Para configurar una plantilla de fraccionamiento
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plantillas de fraccionamiento** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. Rellene los campos según sea necesario.
4. En el campo **Método de calc.**, especifique cómo se calcula el campo **Importe** para cada periodo de la ventana **Previsión fraccionamiento**. Puede elegir entre las opciones siguientes:

   * **Lineal**: los importes periódicos fraccionados se calculan según el número de periodos, distribuidos según la duración del periodo.
   * **Igual por periodo**: los importes periódicos fraccionados se calculan según el número de periodos, distribuidos equitativamente en los periodos.
   * **Días por periodo**: los importes periódicos fraccionados se calculan según el número de días en el periodo.
   * **Definido por el usuario**: no se calculan los importes periódicos de fraccionamiento. Debe rellenar manualmente el campo **Importe** para cada periodo de la ventana Previsión fraccionamiento. Para obtener más información, consulte la sección "Para cambiar una previsión de fraccionamiento de una factura de venta".
5. En el campo **Desc. del período**, especifique una descripción que se mostrará en los movimientos para el registro de fraccionamiento. Puede introducir los siguientes códigos de marcador de posición para valores habituales, que se insertarán automáticamente cuando se muestre la descripción del periodo.

   * %1 = el número de día de la fecha de registro del periodo
   * %2 = el número de semana de la fecha de registro del periodo
   * %3 = el número de mes de la fecha de registro del periodo
   * %4 = el nombre de mes de la fecha de registro del periodo
   * %5 = el nombre del periodo contable de la fecha de registro del periodo
   * %6 = el año fiscal de la fecha de registro del periodo

Ejemplo: la fecha de registro es 06/02/2016. Si introduce "Gastos fraccionados para %4 %6", la descripción mostrada será "Gastos fraccionados para febrero de 2016".

## <a name="to-assign-a-deferral-template-to-an-item"></a>Para asignar una plantilla de fraccionamiento a un producto
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plantillas de fraccionamiento** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha del producto para los que se deban fraccionar los ingresos o los gastos para los periodos contables cuando el artículo se ha vendido o comprado.
3. En el campo **Plantilla de fraccionamiento predeterminada**, seleccione la plantilla de fraccionamiento relevante.

## <a name="to-change-a-deferral-schedule-from-a-sales-invoice"></a>Para modificar una previsión de fraccionamiento de una factura de venta
> [!NOTE]  
>   Los pasos de este procedimiento son los mismos que al cambiar una previsión de fraccionamiento, para gastos, de una factura de compra.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Facturas venta** y, a continuación, seleccione el vínculo relacionado.
2. Cree una factura de ventas para un producto que tenga asignada una plantilla de fraccionamiento. Para obtener más información, vea [Procedimiento: Facturar ventas](sales-how-invoice-sales.md).

    Observe que tan pronto como se introduce el producto (recurso o cuenta de contabilidad) de la línea de factura, el campo **Código de fraccionamiento** se rellena con el código de la plantilla de fraccionamiento asignada.
3. Elija la acción **Previsión fraccionamiento**.
4. En la ventana **Previsión fraccionamiento**, cambie la configuración de la cabecera o los valores de las líneas, por ejemplo, para fraccionar el importe en un periodo contable adicional.
5. Elija la acción **Calcular previsión**.
6. Elija el botón **Aceptar**. La previsión de fraccionamiento se actualiza para la factura de venta. La plantilla de fraccionamiento relacionada no se cambia.

## <a name="to-preview-how-deferred-revenues-or-expenses-will-be-posted-to-the-general-ledger"></a>Para obtener una vista previa de cómo se registrarán los ingresos o los gastos fraccionados costes se registrarán en el libro mayor
> [!NOTE]  
>   Los pasos de este procedimiento son los mismos que al obtener una vista previa de cómo se registran los fraccionamientos de gastos.

1. En la ventana **Factura de ventas**, elija la acción **Vista previa de registro**.
2. En la ventana **Vista previa de registro**, elija la acción **Mov. contabilidad** y, a continuación, elija la acción **Mostrar movimientos relacionados**.

Los movimientos de contabilidad que se van a registrar en la cuenta de fraccionamiento especificada, por ejemplo, Ingresos anticipados, son indican mediante la descripción que ha introducido en el campo **Desc. del período** de la plantilla de fraccionamiento, por ejemplo, "Gastos fraccionados para febrero de 2016".

## <a name="to-review-posted-deferrals-in-the-sales-deferral-summary-report"></a>Para revisar los fraccionamientos registrados en el informe Resumen de fraccionamientos de ventas
> [!NOTE]  
>   Los pasos de este procedimiento son los mismos que al revisar el informe Resumen de fraccionamientos de compras.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Resumen de fraccionamientos de ventas** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Resumen de fraccionamientos de ventas**, en el campo **Saldo a partir de**, introduzca la fecha hasta la que desea ver ingresos fraccionados.
3. Haga clic en el botón **Vista previa**.

## <a name="see-also"></a>Consulte también
[Finanzas](finance.md)  
[Configurar las finanzas](finance-setup-finance.md)  
[Trabajar con diarios generales](ui-work-general-journals.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

