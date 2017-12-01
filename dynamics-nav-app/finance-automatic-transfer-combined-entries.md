---
title: "Transferencia automática y movimientos combinados"
description: "En contabilidad de costos, puede transferir los movimientos de contabilidad a un tipo de costo mediante un registro combinado. Puede especificar si un tipo de costo recibe las movimientos agrupados en el campo **Combinar movimientos** en la definición del tipo de costo. La siguiente tabla describe las distintas opciones."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 638fc123d4113695d70102a94b9fce0bff6b43fa
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="automatic-transfer-and-combined-entries"></a>Transferencia automática y movimientos combinados
En contabilidad de costos, puede transferir los movimientos de contabilidad a un tipo de costo mediante un registro combinado. Puede especificar si un tipo de costo recibe las movimientos agrupados en el campo **Combinar movimientos** en la definición del tipo de costo. La siguiente tabla describe las distintas opciones.  

|Combinar movimientos|Descripción|  
|---------------------|-----------------|  
|Ninguno|Cada movimiento de contabilidad se transfiere individualmente al tipo de costo correspondiente.|  
|Día|Los movimientos de contabilidad que tienen la misma fecha de registro se transfieren como un solo movimiento al tipo de costo correspondiente.|  
|Mes|Todos los movimientos de contabilidad general que tienen el mismo mes de calendario se transfieren como un solo movimiento al tipo de costo correspondiente.|  

> [!IMPORTANT]  
>  Si ha seleccionado la casilla **Transf. autom. desde C/G** en la ventana **Configuración contabilidad costos**, [!INCLUDE[d365fin](includes/d365fin_md.md)] actualiza la contabilidad de costos después de cada registro en la contabilidad. Ya no se pueden realizar movimientos combinados.  

## <a name="see-also"></a>Consulte también  
 [Procedimiento: transferencia de movimientos de contabilidad a los movimientos de costo](finance-how-to-transfer-general-ledger-entries-to-cost-entries.md)   
 [Criterios para la transferencia de movimientos de contabilidad a movimientos de costo](finance-criteria-for-transferring-general-ledger-entries-to-cost-entries.md)   
 [Resultados de la transferencia](finance-results-of-the-transfer.md)   
 [Transferencia y registro de movimientos de costo](finance-transfer-and-post-cost-entries.md)  
 [Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

