---
title: "Deshacer un registro registrando el movimiento de reversión"
description: "Si ha realizado un registro erróneo en el diario general, puede utilizar la función Revertir transacción para deshacer el registro con un seguimiento de auditoria correcto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reimbursement
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 2970914c36f892a5610509e9dc4015d0fb159642
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-reverse-postings"></a>Revertir registros
Para deshacer un registro erróneo del diario, seleccione un movimiento y cree un movimiento de reversión (movimientos idénticos al original, pero con el signo contrario en el campo de importe) con el mismo número de documento y la misma fecha de registro que el movimiento original. Después de revertir un movimiento, debe registrar el movimiento correcto.

Solo se pueden revertir los movimientos que están registrados desde una línea del diario general. Un movimiento solo se puede revertir una vez.

Para obtener más información sobre el registro desde un diario general, vea [Registrar transacciones directamente en la contabilidad](finance-how-post-transactions-directly.md).

Si ha realizado un registro de una cantidad negativa errónea, como un pedido de compra con un número de productos erróneo y lo ha registrado como recibido, pero no facturado, puede deshacer el registro.

Si ha realizado un registro de una cantidad positiva errónea, como un pedido de devolución de compra con un número de productos erróneo y lo ha registrado como enviado, pero no facturado, puede deshacer el registro.   

## <a name="to-reverse-the-journal-posting-of-a-general-ledger-entry"></a>Para revertir el registro de diario de un movimiento de contabilidad
Se pueden revertir movimientos desde todas las ventanas **Movimientos**. El siguiente procedimiento se basa en la ventana **Movs. contabilidad**.
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Movs. contabilidad** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el movimiento que desea revertir y, después, seleccione **Revertir transacción**. Tenga en cuenta que debe proceder de un registro de diario.
3. En la ventana **Revertir movs. trans.**, seleccione el movimiento relevante y, después, seleccione la acción **Revertir**.
4. Elija el botón **Sí** para en el mensaje de confirmación.

## <a name="to-undo-a-quantity-posting-on-a-posted-purchase-receipt"></a>Para deshacer la cantidad registrada en un albarán de compra registrado  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Histórico albaranes compra** y, a continuación, seleccione el vínculo relacionado.  
2.  Abra la recepción registrada que desea deshacer.  
3.  Selecciones las líneas del diario que desea deshacer.  
4.  Seleccione la acción **Deshacer albarán**.

    Una línea correctiva se inserta bajo la línea de recepción seleccionada.  

    Si la cantidad se ha recibido en una recepción de almacén, entonces se inserta una línea de corrección en la recepción de almacén registrado.  

    Los campos de **Cantidad recibida** y de **Cdad. Rec. no facturada** en el pedido de compra relacionado se establecerán a cero.

## <a name="to-undo-and-then-redo-a-quantity-posting-on-a-posted-return-shipment"></a>Deshacer y rehacer una cantidad registrada en un envío devuelto registrado

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Histórico envíos devolución** y, a continuación, seleccione el vínculo relacionado.  
2.  Abra el envío devolución registrado que desea deshacer.
3. Selecciones las líneas del diario que desea deshacer.  

4.  Elija la acción **Deshacer envío dev.**.  

    Se insertará una línea de corrección en el documento registrado y los campos **Cantidad dev. enviada** y **Dev. enviadas no facturadas** del pedido de devolución se establecerán en cero.  

    Ahora vuelva al pedido de devolución de compra para volver a realizar el registro.  

5.  En la ventana **Histórico envío devolución**, tome una nota del número en el campo **Nº devolución** .  
6.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de devolución de compra** y, a continuación, seleccione el vínculo relacionado.  
7.  Abra el pedido de devolución en cuestión y, a continuación, elija la acción **Volver a abrir**.  
8.  Corrija el movimiento en el campo **Cantidad** y vuelva a publicar la orden de devolución de la compra.  

## <a name="see-also"></a>Consulte también
[Registrar transacciones directamente en la contabilidad](finance-how-post-transactions-directly.md)  
[Trabajar con diarios generales](ui-work-general-journals.md)  
[Finanzas](finance.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

