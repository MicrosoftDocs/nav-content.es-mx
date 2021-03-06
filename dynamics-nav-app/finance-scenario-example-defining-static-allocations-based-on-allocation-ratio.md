---
title: "Definición de asignaciones estáticas basadas en la proporción de asignación"
description: "El método de asignaciones estáticas se basa en un valor definido, por ejemplo los metros cuadrados utilizados, o una proporción de asignación establecida de 5:2:4."
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
ms.openlocfilehash: 5f7b627a415a39775dc49726cc655f47383abd17
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="scenario-example-defining-static-allocations-based-on-allocation-ratio"></a>Ejemplo: definición de asignaciones estáticas basadas en la proporción de asignación
El método de asignaciones estáticas se basa en un valor definido, por ejemplo los metros cuadrados utilizados, o una proporción de asignación establecida de 5:2:4.  

Este tema describe cómo definir tres nuevos objetos de costo de destino de asignación para el centro de costo PROD del origen de asignación mediante la proporción 5:2:4 de asignación establecida. Los tres objetos de costo de destino son ACCESORIOS, PINTURA y COLOCACIONES.  

> [!NOTE]  
>  El ejemplo utiliza los datos de demostración en [!INCLUDE[d365fin](includes/d365fin_md.md)].  

## <a name="to-define-the-allocation-source-prod-cost-center-on-the-general-fasttab"></a>Para definir el centro de costo PROD de origen de asignación en la ficha desplegable General  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Asignación costos** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ventana **Asignación costos**, elija la acción **Nuevo**.  
3.  En el campo **ID**, presione Entrar o escriba un Id.  
4.  En el campo **Nivel**, introduzca **1**.  
5.  Especifique las fechas del período en los campos **Válido desde** y **Válido hasta**.  
6.  En el campo **Código centro costo**, introduzca **PROD**.  
7.  En el campo **Abonar en tipo de costo**, especifique un tipo de costo **9903**.  

## <a name="to-define-the-allocation-target-cost-objects-on-the-lines-fasttab"></a>Para definir los objetos de costo de destino de asignación en la Ficha desplegable Líneas  

1.  En la primera línea, en el campo **Tipo costo destino**, especifique **9903**.  
2.  En la primera línea, en el campo **Objeto costo destino**, seleccione **ACCESORIOS**.  
3.  En la primera línea, en el campo **Tipo destino asignación**, seleccione **Todos los costos** para definir cómo se asignan todos los costos acumulados.  
4.  En la primera línea, en el campo **Base**, seleccione **Estático** para utilizar el método de asignación estática.  
5.  En la primera línea, en el campo **Compartir**, especifique la proporción de asignación **5**.  
6.  En la segunda línea, en el campo **Tipo costo destino**, especifique **9903**.  
7.  En la segunda línea, en el campo **Objeto costo destino**, seleccione **PINTURA**.  
8.  En la segunda línea, en el campo **Tipo destino asignación**, seleccione **Todos los costos** para definir cómo se asignan todos los costos acumulados.  
9. En la segunda línea, en el campo **Base**, seleccione **Estático** para utilizar el método de asignación estática.  
10. En la segunda línea, en el campo **Compartir**, especifique la proporción de asignación **2**.  
11. En la tercera línea, en el campo **Tipo costo destino**, especifique **9903**.  
12. En la tercera línea, en el campo **Objeto costo destino**, seleccione **COMPLEM**.  
13. En la tercera línea, en el campo **Tipo destino asignación**, seleccione **Todos los costos** para definir cómo se asignan todos los costos acumulados.  
14. En la tercera línea, en el campo **Base**, seleccione **Estático** para utilizar el método de asignación estática.  
15. En la tercera línea, en el campo **Compartir**, especifique la proporción de asignación **4**.  

> [!IMPORTANT]  
>  [!INCLUDE[d365fin](includes/d365fin_md.md)] calcula automáticamente el campo **Porcentaje** con un porcentaje que depende de las tres relaciones de asignación que se han introducido en el campo **Compartir** para las tres líneas.  

## <a name="see-also"></a>Consulte también  
[Procedimiento: configurar origen y destinos de asignación](finance-how-to-set-up-allocation-source-and-targets.md)   
[Definición y asignación de costos](finance-define-and-allocate-costs.md)   
[Ejemplo: definición de asignaciones dinámicas basándose en productos vendidos](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)   
[Definición y asignación de costos](finance-define-and-allocate-costs.md)

