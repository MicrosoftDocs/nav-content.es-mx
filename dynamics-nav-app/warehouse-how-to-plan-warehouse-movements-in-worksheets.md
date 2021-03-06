---
title: "Planificar movimientos de almacén en hojas de trabajo"
description: "Planifique los movimientos en la hoja de trabajo con una función de reposición de ubicación o manualmente mediante la planificación de las líneas que desea crear como instrucciones de movimiento."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/16/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: fcf44a681e597df1bd50e94e851810fa00656a96
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-plan-warehouse-movements-in-worksheets"></a>Procedimiento: planifique movimientos de almacén en hojas de trabajo
Planifique los movimientos en la hoja de trabajo con una función de reposición de ubicación o manualmente mediante la planificación de las líneas que desea crear como instrucciones de movimiento.  

## <a name="to-calculate-a-replenishment-movement"></a>Para calcular un movimiento de reposición  
Cuando el almacén envía los productos a los clientes, las ubicaciones con los ranking de ubicación más altos contienen cada vez menos productos. Para rellenar estas ubicaciones de picking de ranking más alto con productos de otras ubicaciones, ejecute la función **Calcular reposición ubicación** de la ventana **Hoja trabajo movimiento**.

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja movimiento** y, a continuación, seleccione el vínculo relacionado.  
2.  Elija la acción **Calcular reposición ubicación**.  

    [!INCLUDE[d365fin](includes/d365fin_md.md)] crea líneas que indican exactamente cómo debe mover los productos de las ubicaciones de ranking inferior a las ubicaciones de ranking superior.  

    > [!NOTE]  
    >  Un movimiento se sugiere según el FEFO cuando se activa la función **Crear movimiento** si cumple las siguientes condiciones para un artículo:  
    >   
    >  -   El producto tiene fecha de caducidad.  
    > -   Se selecciona la casilla **Picking según FEFO (Primero en caducar, primero en salir)** de la ficha de almacén.  
    > -   La casilla **Ubicac. obligatoria** de la ficha de almacén está seleccionada.  
    > -   Los campos **Desde zona** y **Desde ubicación** están en blanco.  

    Para obtener más información, consulte [Realización de picking por el FEFO](warehouse-picking-by-fefo.md).  

3.  Observe las líneas y cámbielas si es necesario, o elimine algunas si no tiene tiempo suficiente para ejecutar todas.  
4.  Elija la acción **Crear movimiento** para crear una instrucción de almacén para que los empleados de almacén realicen una acción.  

## <a name="to-move-the-entire-contents-of-one-or-more-bins-by-using-the-get-bin-content-function"></a>Mover todo el contenido de una o varias ubicaciones con la función Tomar contenido ubicación  
También puede utilizar la hoja de trabajo de movimiento para planificar otros movimientos de inventario en el almacén. Por ejemplo, cuando desee colocar productos en una ubicación para controlar la calidad, puede utilizar la hoja de trabajo de movimiento para planificar esta acción y, a continuación, crear un movimiento para darle instrucciones a un empleado.  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja movimiento** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Tomar conten. ubicac**. Utilice la ventana de solicitud para filtrar las ubicaciones y productos que desea que aparezcan en las líneas de la hoja de trabajo de movimiento.  
3.  Rellene los campos correspondientes de la ventana de condiciones del proceso. Por ejemplo, si desea ver el contenido de todas las ubicaciones en una determinada zona del almacén, rellene el campo **Cód. zona**. Si desea recuperar líneas de cada ubicación que contenga un producto determinado, rellene el campo **Nº producto**.  

    > [!NOTE]  
    >  No puede mover manualmente productos dentro o fuera de una ubicación de tipo RECEPCIÓN, porque los productos que están en una ubicación de tipo RECEPCIÓN deben ubicarse antes de que formen parte de las existencias disponibles.  

4.  Si recupera muchas líneas, seleccione **Ordenar** para seleccionar un método de ordenación que determine el orden en el que aparecerán las líneas en la hoja de trabajo y, a continuación, haga clic en **Aceptar**.  

    > [!NOTE]  
    >  Las líneas de movimiento se recuperan según el FEFO cuando se activa la función **Tomar conten. ubicac.** si cumple las siguientes condiciones para un producto:  
    >   
    >  -   El producto tiene fecha de caducidad.  
    > -   Se selecciona la casilla **Picking según FEFO (Primero en caducar, primero en salir)** de la ficha de almacén.  
    > -   La casilla **Ubicac. obligatoria** de la ficha de almacén está seleccionada.  
    > -   Los campos **Desde zona** y **Desde ubicación** están en blanco.  

5.  Complete algunas de las líneas recuperadas para reflejar los cambios que desea realizar. En cada producto que desee mover, debe rellenar los campos **Nº producto**, **Desde cód. ubicación**, **Hasta cód. ubicación** y **Cantidad**.  
6.  Elimine las líneas incompletas que ha utilizado para su información.  
7.  Cuando las líneas de la hoja de trabajo de movimiento reflejen exactamente cómo debe realizar el empleado del almacén la acción de movimiento, elija la acción **Crear movimiento** para crear las instrucciones para el empleado.  

## <a name="see-also"></a>Consulte también  
[Gestión almacén](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

