---
title: "Cerrar los movimientos de producto abiertos que se crean por una liquidación fija en el diario de productos"
description: "Puede utilizar el campo **Liquidar por mov.** en la ventana **Diario de productos** para crear manualmente una liquidación fija entre una transacción de entrada y la transacción de salida original. Por ejemplo, para corregir la transacción de salida o procesar su devolución."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/09/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b0b0daad01f8108d035739e387b38af4f0311ff9
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-close-open-item-ledger-entries-resulting-from-fixed-application-in-the-item-journal"></a>Cómo cerrar los movimientos de producto abiertos que se crean por una liquidación fija en el diario de productos
Puede utilizar el campo **Liquidar por mov.** en la ventana **Diario de productos** para crear manualmente una liquidación fija entre una transacción de entrada y la transacción de salida original. Por ejemplo, para corregir la transacción de salida o procesar su devolución. Para obtener más información, consulte Liquidar por mov.  

> [!IMPORTANT]  
>  Las liquidaciones fijas realizadas de esta forma aplican solo al costo, no a la cantidad. Por consiguiente, el movimiento de producto positivo registrado no cerrará la salida aplicado y seguirá abierto. Esto también aplica cuando se registra una liquidación fija para una positivo a un movimiento negativo que no se ha cerrado mediante un movimiento normal positivo, lo cual produce que tanto los movimientos negativos y positivos sigan abiertos.  
>   
>  Esto también significa que no puede cerrar un periodo de inventario si existe tal tipo de movimiento.  

El siguiente procedimiento muestra cómo cerrar los movimientos realizando dos registros correctores en el diario de productos.  

## <a name="to-close-open-item-ledger-entries-that-result-from-a-fixed-application-in-the-item-journal"></a>Para cerrar los movimientos de producto abiertos que se crean por una liquidación fija en el diario de productos  

1.  Utilice el campo **Liquidar por mov.** para registrar un ajuste positivo con la cantidad correspondiente. Esto cierra el movimiento negativo original con una liquidación fija.  
2.  Utilice el campo **Liquidar por mov.** para registrar un ajuste negativo. Esto cierra el movimiento positivo de corrección original con una liquidación fija.  

## <a name="see-also"></a>Consulte también  
[ Cómo eliminar y liquidar de nuevo los movimientos contables de producto](finance-how-to-remove-and-reapply-item-entries.md)  
 [Procesamiento de devoluciones de ventas y cancelaciones](sales-how-process-sales-returns-cancellations.md)   
 [Configuración de valuación de inventarios](finance-set-up-inventory-valuation-and-costing.md)   
 [Administración de costos de inventario](finance-manage-inventory-costs.md)   
 [Detalles de diseño: Métodos de costo](design-details-costing-methods.md)

