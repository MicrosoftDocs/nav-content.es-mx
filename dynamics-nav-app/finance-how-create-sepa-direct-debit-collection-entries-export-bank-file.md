---
title: "Exportar movimientos de domiciliación de adeudo directo SEPA"
description: "Cree una colección de débito directo que contenga información sobre la cuenta bancaria del cliente, las facturas de ventas afectadas y la orden de domiciliación de adeudo directo."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 68ae93fe5a71758b4f5b7eeaedd52f11721faaf9
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-create-sepa-direct-debit-collection-entries-and-export-to-a-bank-file"></a>Creación de movimientos de domiciliación de adeudo directo SEPA y exportación a un archivo bancario
Para indicar al banco que transfiera el importe de pago desde el banco del cliente al banco de su empresa, debe crear un cobro por adeudo directo que contiene información acerca de los bancos del cliente, las facturas de venta afectadas y la orden de domiciliación de adeudo directo. Desde el movimiento de pago por domiciliación, luego exporta un archivo XML que se envía o carga en el banco electrónico para su procesamiento. Los pagos que el banco no pudo procesar los comunicará el banco al usuario y este último deberá rechazar manualmente los movimientos de pago por adeudo directo en cuestión.  

> [!NOTE]  
>  Para cobrar los pagos mediante adeudo directo SEPA, la divisa de la factura de venta debe ser EURO.  

### <a name="to-create-a-direct-debit-collection"></a>Creación de un cobro por domiciliación  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cobros por adeudo directo** y, a continuación, seleccione el vínculo relacionado.  
2. En la ventana **Cobros por adeudo directo**, en la pestaña **Inicio**, en el grupo **Nuevo**, elija **Crear cobro por adeudo directo**.  
3. En la ventana **Crear cobro por adeudo directo**, rellene los campos tal como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Fecha vencimiento inicio**|Especifique la primera fecha de vencimiento de pago más temprana de las facturas de venta para las que desee crear un cobro por domiciliación.|  
    |**Fecha de vencimiento final**|Especifique la fecha de vencimiento de pago más tarde de las facturas de venta para las que desee crear un cobro por domiciliación.|  
    |**Tipo socio**|Especifique el cobro por domiciliación se realiza para los clientes de tipo **Empresa** o **Persona**.|  
    |**Solo clientes con mandado válido**|Especifique si se crea un cobro por adeudo directo para los clientes que tienen una orden de domiciliación de adeudo directo válida. **Nota**: Se crea un cobro por domiciliación incluso si el campo **Id. de orden de domiciliación de adeudo directo** no se ha rellenado en la factura de venta.|  
    |**Solo facturas con orden de domiciliación válida**|Especifique si se crea un cobro de adeudo directo solo para las facturas de ventas si se selecciona una orden de domiciliación de adeudo directo válida en el campo **Id. de orden de domiciliación de adeudo directo** en la factura de ventas.|  
    |**Cód. cuenta banco**|Especifique a cuál de los bancos de su empresa se transferirá el pago cobrado desde el banco del cliente.|  
    |**Nombre banco**|Especifica el nombre del banco seleccionado en el campo **Cód. cuenta banco**. Este campo se rellena automáticamente.|  

4. Elija el botón **Aceptar**.  

     Se agrega un cobro por domiciliación a la ventana **Cobros por adeudo directo** y se crean uno o varios movimientos de cobros por domiciliación.  

### <a name="to-export-a-direct-debit-collection-entry-to-a-bank-file"></a>Exportación de movimientos de cobro por domiciliación a un archivo de banco  
1. En la ventana **Cobros por adeudo directo**, en la pestaña **Inicio**, en el grupo **Proceso**, elija **Movimientos de cobros por adeudo directo**.  
2. En la ventana **Movimientos de cobros por adeudo directo**, seleccione el movimiento que desee exportar y, a continuación, en la pestaña **Inicio**, en el grupo **Procesar**, elija **Crear archivo de cobro por adeudo directo**.  
3. Guarde el archivo de exportación en la ubicación desde donde envía o carga en el banco electrónico.  

     En la ventana **Direct Debit Collect. Movimientos**, el campo **Estado cobro por adeudo directo** se cambia el archivo creado. En la ventana **Órdenes de domiciliación de adeudo directo SEPA**, el campo **Contador debe** se actualiza con un recuento.  

Si el archivo exportado no se puede procesar, por ejemplo, porque el cliente es insolvente, puede rechazar el movimiento de cobro por domiciliación. Si el banco procesa correctamente el archivo exportado, los pagos por vencimientos de las facturas de venta implicadas se cobran automáticamente de los clientes implicados. En ese caso, puede cerrar el cobro.  

### <a name="to-reject-a-direct-debit-collection-entry"></a>Rechazo de un movimiento de cobro por domiciliación  

* En la ventana **Movimientos de cobros por adeudo directo**, seleccione el movimiento que no se procesó correctamente y, a continuación, en la pestaña **Inicio**, en el grupo **Procesar**, elija **Rechazar movimiento**.  

     El valor del campo **Estado** de la ventana **Movimientos de cobros por adeudo directo** se cambia a **Rechazada**.  

### <a name="to-close-a-direct-debit-collection"></a>Cierre de un cobro por domiciliación  
*  En la ventana **Movimientos de cobros por adeudo directo**, seleccione el movimiento que no se procesó correctamente y, a continuación, en la pestaña **Inicio**, en el grupo **Procesar**, elija **Cerrar cobro**.  

     El cobro por domiciliación relacionado está cerrado.  

Ahora podrá registrar las recepciones de pago para las facturas de venta implicadas. Puede hacerlo, ya que normalmente se registran recibos de pago, como en la ventana **Registro de pago**, o bien puede registrar los recibos de pago relacionados directamente en la ventana **Movimientos de cobros por adeudo directo**. Para obtener más información, consulte [Registro de recibos de pagos de domiciliación de adeudo directo SEPA](finance-how-to-post-sepa-direct-debit-payment-receipts.md).  

## <a name="see-also"></a>Consulte también  
[Configuración de domiciliaciones de adeudo directo SEPA](finance-how-to-set-up-sepa-direct-debit.md)  
[Registro de recibos de pagos de domiciliación de adeudo directo SEPA](finance-how-to-post-sepa-direct-debit-payment-receipts.md)  
[Cobro de pagos mediante adeudo directo SEPA](finance-collect-payments-with-sepa-direct-debit.md)  

