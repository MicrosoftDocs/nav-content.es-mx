---
title: "Procedimiento: Baje componentes según la producción de la operación"
description: "Para los productos que se configuran con el método de baja hacia atrás, el comportamiento predeterminado es calcular y registrar el consumo de componentes cuando cambie el estado de una orden de producción lanzada a **Terminada**. Para obtener más información, consulte Método de baja."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 48645ff5d943b2f7093224289ff3cad6cfa6537e
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-flush-components-according-to-operation-output"></a>Procedimiento: Baje componentes según la producción de la operación
Para los productos que se configuran con el método de baja hacia atrás, el comportamiento predeterminado es calcular y registrar el consumo de componentes cuando cambie el estado de una orden de producción lanzada a **Terminada**.  

Si también define los códigos de vínculo de ruta, el cálculo y el registro se producen cuando termina cada operación, y se registra la cantidad realmente consumida en la operación. Para obtener más información, consulte [Creación de conexiones de ruta](production-how-to-create-routings.md).  

Por ejemplo, si una orden de producción para producir 800 metros requiere 8 kg de un componente, cuando se registran 200 metros como salida, se registran automáticamente 2 kg de consumo.  

Esta funcionalidad se útil por los motivos siguientes:  

-   **Valuación de inventarios**: los movimientos de valores para la salida y el consumo se crean en paralelo según progresa la orden de producción. Sin los códigos de vínculo de ruta, el valor de inventario aumentará mientras se registra salida y después disminuirá en un momento posterior cuando el valor del consumo de componentes se registra con la orden de producción terminada.  
-   **Disponibilidad existencias**: con el registro gradual del consumo, la disponibilidad de productos de componentes está más actualizado, que es importante para mantener los saldos internos entre la demanda y el suministro. Sin los códigos de vínculo de ruta, otras demandas para el componente pueden creer que está disponible mientras se encuentre pendiente un registro retrasado del consumo.  
-   **A tiempo**: con la posibilidad de personalizar los productos para las solicitudes de cliente, puede minimizar la pérdida de tiempo de asegurarse de que solo se produzcan cambios de trabajo y del sistema si es necesario.  

El siguiente procedimiento muestra cómo combinar códigos de vínculo de ruta y baja hacia atrás de modo que la cantidad que se baja para cada operación es proporcional a la salida real de la operación terminada.  

## <a name="to-flush-components-according-to-operation-output"></a>Para bajar componentes según la salida de la operación  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Editar**.  
3.  En la ficha desplegable **Reposición**, en el campo **Método de baja**, seleccione **Anticipada**.  

    > [!NOTE]  
    >  Seleccione **Pick+ Adelante** si el componente se utiliza en un almacén que está configurado para la ubicación y picking directos.  

4.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Rutas** y, a continuación, seleccione el vínculo relacionado.  
5.  Defina los códigos de vínculo de ruta para cada operación que consume el componente. Para obtener más información, consulte [Creación de conexiones de ruta](production-how-to-create-routings.md).  
6.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **L.M. de producción** y, a continuación, seleccione el vínculo relacionado.  
7.  Defina los códigos de vínculo de ruta desde cada instancia del componente hasta la operación donde se consume.

    > [!IMPORTANT]  
    >  El componente debe tener un vínculo de ruta hasta la última operación en la ruta.  

## <a name="see-also"></a>Consulte también  
[Creación de L.M. de producción](production-how-to-create-production-boms.md)  
[Configuración de fabricación](production-configure-production-processes.md)  
[Fabricación](production-manage-manufacturing.md)    
[Planificación](production-planning.md)   
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

