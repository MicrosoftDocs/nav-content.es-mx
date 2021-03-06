---
title: "Detalles de diseño: Cierre de aprovisionamiento y demanda"
description: Cuando se han realizado los procedimientos de equilibrado del suministro, existen tres situaciones finales posibles.
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
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 337fdb4c625e17e72f4adb692cbf0f2729ae96b7
ms.contentlocale: es-mx
ms.lasthandoff: 10/26/2017

---
# <a name="design-details-closing-demand-and-supply"></a>Detalles de diseño: Cierre de aprovisionamiento y demanda
Cuando se han realizado los procedimientos de equilibrado del suministro, existen tres situaciones finales posibles:  

-   Se han cumplido la cantidad necesaria y la fecha de los eventos de demanda, y se puede cerrar la planificación de ellos. El evento de suministro aún está abierto y puede cubrir la demanda siguiente, por lo que el procedimiento de contrapartida puede empezar con el evento de suministro actual y la demanda siguiente.  

-   El pedido de suministro no se puede modificar para cubrir toda la demanda. El evento de demanda sigue abierto, con una cantidad sin cubrir que se puede cubrir mediante el evento de suministro siguiente. Por lo tanto, se cierra el evento de suministro, por lo que el equilibrado puede empezar con la demanda actual y el siguiente evento de suministro.  

-   Se ha cubierto toda la demanda; no hay demanda subsiguiente (o no ha habido demanda en absoluto). Si hay algún aprovisionamiento de excedente, se puede reducir (o cancelarse) y después cerrar. Es posible que existan eventos de suministro adicionales más adelante en la cadena y también se deben cancelar.  

 Por último, el sistema de planificación creará una conexión de seguimiento de pedidos entre el suministro y la demanda.  

## <a name="creating-the-planning-line-suggested-action"></a>Crear la línea de planificación (acción sugerida)  
 Si se sugiere alguna acción (nueva, cambiar de cantidad, reprogramar, reprogramar y cambiar de cantidad o cancelar) para revisar el pedido de aprovisionamiento, el sistema de planificación crea una línea de planificación en la hoja de trabajo de planificación. El seguimiento de pedidos obliga a la creación de la línea de planificación no solo cuando se cierra el evento de aprovisionamiento, sino también si se cierra el evento de demanda, aunque el evento de aprovisionamiento esté aún abierto y puede estar sujeto a los cambios adicionales cuando se procesa el evento de demanda siguiente. Esto significa que la línea de planificación se puede modificar de nuevo cuando se crea por primera vez.  

 Para minimizar el acceso de base de datos al manipular las órdenes de producción, la línea de planificación se puede mantener en tres niveles, a la vez que se intenta realizar el nivel de mantenimiento menos exigente:  

-   Crear solo la línea de planificación con la fecha de vencimiento y la cantidad actuales, pero sin la ruta y los componentes.  

-   Incluir ruta: la ruta planificada se diseña incluyendo el cálculo de las fechas y las horas de inicio y fin. Esto exige muchos accesos a la base de datos. Para determinar las fechas finales y de vencimiento, es posible que sea necesario calcularlo aunque el evento de suministro no se haya cerrado (en el caso de la programación hacia delante).  

-   Incluir despliegue de L.M.: esto puede esperar a justo antes de cerrar el evento de aprovisionamiento.  

 De este modo concluyen las descripciones de cómo el sistema de planificación carga, da prioridad y equilibra la demanda y el suministro. En integración con esta actividad de planificación de aprovisionamientos, el programa debe garantizar que el nivel de inventario requerido de cada producto planificado se mantiene según sus directivas de reorden.  

## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Equilibrio de aprovisionamiento y demanda](design-details-balancing-demand-and-supply.md)   
 [Detalles de diseño: Conceptos centrales del sistema de planificación](design-details-central-concepts-of-the-planning-system.md)   
 [Detalles de diseño: Planificación de aprovisionamiento](design-details-supply-planning.md)

