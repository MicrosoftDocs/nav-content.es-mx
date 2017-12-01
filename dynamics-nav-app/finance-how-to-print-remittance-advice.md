---
title: Imprimir un aviso de pago
description: "Puede ayudar a sus proveedores a realizar conciliaciones si imprime un aviso de pago antes de publicar un diario de pagos y después de registrar un pago."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: es-mx
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a>Imprimir un aviso de pago
Puede imprimir el aviso de pago antes de registrar el diario de pagos y después de registrar un pago. Este aviso muestra números de factura del proveedor que ayudan a los proveedores a realizar la conciliación.

##<a name="to-print-remittance-advice"></a>Para imprimir un aviso de pago
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios de pagos** y, a continuación, seleccione el vínculo relacionado.  
2. En la ventana **Diario de pagos**, seleccione el pago para el que se debe imprimir el aviso de pago.  
3. Seleccione la acción **Imprimir un aviso de pago**.  
4. En el proceso **Aviso de pago - Diario**, en la ficha desplegable **Lín. diario general**, seleccione los filtros apropiados.  
  
    >[!Note]
    > Puede filtrar mediante el número de documento externo del proveedor para hacer coincidir los pagos con las facturas.

5. En la ficha desplegable **Proveedor**, seleccione los filtros apropiados.  
6. Elija **Imprimir** para imprimir el informe o **Vista preliminar** para verlo ahora.  

## <a name="using-remittance-advice-reports"></a>Mediante informes de aviso de pago
En la tabla siguiente se describen los informes que se pueden utilizar con el aviso de pago:

|Informe|Descripción|
|----|----|
|Aviso de pago - Informe del diario|Este informe indica qué documentos se incluyen en el pago. Para las líneas del diario general, puede especificar el libro de diario y la sección de diario desde los que se imprimirán los avisos de remesa, la fecha de la primera actividad para imprimir y filtrar por número de documento. Para los proveedores, puede introducir los números de los proveedores que se incluirán en el informe. |
|Aviso pago - Informe de entradas| Este informe indica qué documentos se incluyen en el pago. Defina el contenido del informe estableciendo filtros. Puede definir campos adicionales en la ficha mediante el campo **Campo**. Para los movimientos de proveedor, puede especificar los proveedores que se incluirán en el informe, la fecha de la primera actividad a imprimir, la divisa y el número del movimiento. |

> [!Note]
> El Aviso de pago - Informe del diario no admite escenarios de aplicación de divisa cruzada ni tolerancias de pago. Para obtener más información vea, [Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas](finance-how-enable-application-ledger-entries-different-currencies.md).

> [!Tip]
> Para obtener más información sobre cómo usar los informes, consulte [Visualización de los informes de prueba antes de realizar el registro](ui-how-view-test-reports-posting.md), [Trabajar con informes](ui-work-report.md) y [Buscar, filtrar y ordenar datos](ui-enter-criteria-filters.md).

##<a name="see-also"></a>Consulte también  
[Dynamics NAV](across-get-started.md)
