---
title: "Procedimiento: configurar origen y destinos de asignación"
description: "Cada asignación está formada por un origen de asignación y uno o varios destinos de asignación. El origen de asignación define qué costos se asignarán. Los destinos de asignación determinan dónde se deben asignar los costos."
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
ms.openlocfilehash: 91adabefc3e0b4a69b24b34a084f89c17711d573
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-allocation-source-and-targets"></a>Procedimiento: configurar origen y destinos de asignación
Cada asignación está formada por un origen de asignación y uno o varios destinos de asignación. El origen de asignación define qué costos se asignarán. Los destinos de asignación determinan dónde se deben asignar los costos.  

## <a name="to-set-up-cost-allocations"></a>Para configurar asignaciones de costo  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Asignación costos** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ventana **Asignación costos**, elija la acción **Editar**.  
3.  Especifique un identificador para el origen de asignación en el campo **ID**.  
4.  Defina un nivel como un número entre 1 y 99 en el campo **Nivel**. El registro de la asignación seguirá el orden de los niveles.  
5.  Escriba un tipo de costo para definir qué tipos de costo se asignarán en el campo **Intervalo tipo costo**. Si todos los costos de un tipo de costo se asignan, no se define ningún intervalo.  
6.  Especifique un centro de costo junto con los costos que se asignarán en el campo **Código centro costo**.  
7.  Especifique un objeto de costo junto con los costos que se asignarán en el campo **Código objeto costo**. Muy a menudo, este campo permanece vacío porque raramente los objetos de costo se asignan a otros objetos de costo.  
8.  Especifique un tipo de costo en el campo **Abonar en tipo de costo**. Los costos que asignen se abonarán en el tipo de costo de origen. El registro de haber se registrará en el tipo de costo que se indique aquí.  
9. En la ficha desplegable **Líneas**, define los destinos de asignación. En la primera línea, escriba un tipo de costo en el campo **Tipo costo destino**. Define a qué tipo de costo se carga la asignación.  
10. En la primera línea, introduzca el primer destino de asignación en el campo **Centro costo destino** o el campo **Objeto costo destino**. Estos dos campos definen en qué centro de costo u objeto de costo se carga la asignación. Sólo puede rellenar uno de ellos, pero no los dos.  
11. Repita los mismos pasos en la segunda línea para configurar los destinos de asignación adicionales.  
12. Una vez configurado el destino y los orígenes de asignación, elija la acción **Calcular clave de asignación** para calcular los valores compartidos totales.  

> [!NOTE]  
>  Seleccione la casilla **Bloqueado** para desactivar la configuración de asignación.  

## <a name="see-also"></a>Consulte también  
[Contabilidad para costos](finance-manage-cost-accounting.md)  
 [Configuración de filtros para las bases de la asignación dinámica](finance-setting-filters-for-dynamic-allocation-bases.md)   
 [Ejemplo: definición de asignaciones estáticas basadas en la proporción de asignación](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)   
 [Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
 [Definición y asignación de costos](finance-define-and-allocate-costs.md)   
 [Terminología en contabilidad de costos](finance-terminology-in-cost-accounting.md)  
 [Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

