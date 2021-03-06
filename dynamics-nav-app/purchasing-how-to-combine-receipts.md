---
title: "Combinación de albaranes"
description: "Si desea facturar varias recepciones de compra a la vez, puede utilizar la función Combinar recepciones."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/14/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 10749dc8d8d692d94c5405fbb0a4a965d482f013
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-combine-receipts-on-a-single-invoice"></a>Procedimiento: agrupar albaranes en una factura única
Si desea facturar varias recepciones de compra a la vez, puede utilizar la función **Combinar recepciones**.  

Para poder crear una recepción de compra combinada, es necesario haber registrado primero más de una recepción del mismo proveedor y en la misma divisa. En otras palabras, debe haber rellenado dos o más pedidos de compra, así como haberlos registrado como recibidos, pero no facturado.  

Cuando se combinan varias recepciones de compra en una factura y se registran, se crea una factura de compra registrada para las líneas facturadas. El campo **Cantidad facturada** del pedido de compra de origen, o del pedido abierto de compra, se actualiza en función de la cantidad facturada. Sin embargo, este documento de compra original no se elimina, aunque se haya recibido y facturado por completo, por lo que debe eliminar el documento de compra.  

## <a name="to-combine-receipts"></a>Para combinar recepciones  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Facturas compra** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione la acción **Nuevo**. Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).  
3. En la ficha desplegable Líneas, haga clic en **Acciones**, y elija la acción **Tomar líneas de envío**.  
4. Seleccione las distintas líneas de recepción que desee incluir en la factura.  

    Si se ha seleccionado una línea de recepción incorrecta o desea comenzar desde el principio, simplemente elimine las líneas de la factura de compra y vuelva a usar la función **Tomar líns. recep**.  
5. Para registrar la factura, elija la acción **Registrar**.  

## <a name="to-remove-open-purchase-orders-after-combined-receipt-posting"></a>Procedimiento para eliminar pedidos de compra abiertos después del registro de recepción combinada  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Eliminar peds. compra. factdos...** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].
3. Elija el botón **Aceptar**.  

También puede eliminar los pedidos individuales manualmente.

Repita las tareas 1 a 3 para cualquier otro documento asignado, como pedidos abiertos de compra.

## <a name="see-also"></a>Consulte también  
[Compras](purchasing-manage-purchasing.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

