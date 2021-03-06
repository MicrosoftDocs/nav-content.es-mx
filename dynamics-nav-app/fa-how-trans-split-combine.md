---
title: Reclasificar activos fijos
description: Un activo fijo se reclasifica para transferirlo a otro departamento, dividirlo o combinarlo con otros activos fijos.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 43b24201037de228faf4f58cc46bd92f796d72e3
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-transfer-split-or-combine-fixed-assets"></a>Procedimiento: Transferir, dividir o combinar activos fijos.
Puede utilizar el diario de reclasificación de activos fijos para transferir, dividir y combinar activos fijos. En el informe **A/F - Valor contable 02** puede ver o imprimir los resultados de la reclasificación de los activos fijos.

## <a name="to-transfer-a-fixed-asset-to-a-different-department"></a>Para transferir un activo fijo a otro departamento
Puede que necesite transferir un activo fijo a un departamento diferente cuando, por ejemplo, coloca un activo en el departamento de producción mientras está en construcción y luego lo mueve al departamento de administración cuando está terminado.  

1. Configure un activo fijo nuevo. Especifique el nuevo departamento en el campo **Cód. departamento**.
2. Asigne un libro de amortización de activo al nuevo activo fijo. Para obtener más información, vea [Procedimiento: Activos fijos adquiridos](fa-how-acquire.md).
3. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Diarios reclasif.** y, a continuación, seleccione el vínculo relacionado.
4. Cree un diario de reclasificación donde el campo **A/F N. º** contenga el activo original, y el campo **A/F N. º nuevo** los nuevos activos fijos que se moverán.  
5. Seleccione la acción **Reclasificación**.

    Se han creado dos líneas en el diario de activos con la plantilla y sección que ha especificado en la ventana **Config. diario activos** para el libro de amortización especificado. Para obtener más información, consulte [Procedimiento: Configurar amortización de activos fijos](fa-how-setup-depreciation.md).
6. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.    
7. En la ventana **A/F diario general**, seleccione la acción **Registrar** para registrar la reclasificación que se ha realizado en los pasos 4 y 5.

Si registró el costo de adquisición de un activo, puede utilizar el diario de reclasificación de activos fijos para dividir el costo de adquisición entre varios activos.  

## <a name="to-split-a-fixed-asset-into-three-fixed-assets"></a>Para dividir un activo en tres activos fijos
Puede dividir un activo fijo en varios activos fijos, por ejemplo, cuando necesita distribuir un activo fijo entre tres departamentos diferentes. En este caso, puede mover, por ejemplo, el 25 % del costo de adquisición y la amortización del activo fijo original al segundo activo fijo y un 45 % al tercero. El 30 % restante permanece en el activo fijo original.

1. Configure dos activos fijos nuevos. Especifique el nuevo departamento en el campo **Cód. departamento**.
2. Asigne libros de amortización de activo a los nuevos activos fijos. Para obtener más información, vea [Procedimiento: Activos fijos adquiridos](fa-how-acquire.md).
3. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Diarios reclasif.** y, a continuación, seleccione el vínculo relacionado.
4. Cree dos líneas del diario de reclasificación, una para cada activo fijo nuevo.
5. En la primera línea, introduzca el segundo activo en el campo **A/F N. º nuevo** y 25 en el campo **% Costo reclasif**.
6. En la segunda línea, introduzca el tercer activo en el campo **A/F N. º nuevo** y 40 en el campo **% Costo reclasif**.
7. En ambas líneas, seleccione las casillas **Costo reclasif.** y **Amortización reclasif.**   
8. Seleccione la acción **Reclasificación**.

    Se han creado dos líneas en el diario de activos con la plantilla y sección que ha especificado en la ventana **Config. diario activos** para el libro de amortización especificado. Para obtener más información, consulte [Procedimiento: Configurar amortización de activos fijos](fa-how-setup-depreciation.md).    
9. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.
10. En la ventana **A/F diario general**, seleccione la acción **Registrar** para registrar la reclasificación que se ha realizado en los pasos del 4 al 8.

## <a name="to-combine-two-fixed-assets-into-one"></a>Para combinar dos activos fijos en uno
Puede combinar varios activos en uno, por ejemplo, cuando mueve los activos fijos distribuidos a un solo departamento. Si ha registrado los costos de adquisición y la amortización de los activos fijos que se moverán, esos valores se combinarán con el activo fijo simple.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **A/F Diarios reclasif.** y, a continuación, seleccione el vínculo relacionado.
2. Cree un diario de reclasificación donde el campo **A/F N. º** contenga el activo que se moverá o combinará, y el campo **A/F N. º nuevo** el activo con el que se combinará.
3. Deje el campo **% Costo reclasif.** vacío para mover o combinar el costo de adquisición completo.    
4. Seleccione las casillas **Costo reclasif.** y **Amortización reclasif.**
5. En la pestaña **Acciones**, elija **Reclasificar**.

    Se han creado dos líneas en el diario de activos con la plantilla y sección que ha especificado en la ventana **Config. diario activos** para el libro de amortización especificado. Para obtener más información, consulte [Procedimiento: Configurar amortización de activos fijos](fa-how-setup-depreciation.md).   
6. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.
7. En la ventana **A/F diario general**, seleccione la acción **Registrar** para registrar la reclasificación que se ha realizado en los pasos del 2 al 5.

## <a name="to-view-changed-depreciation-book-values-due-to-fixed-asset-reclassification"></a>Para ver los cambios en los valores del libro de amortización debido a la reclasificación de activos fijos
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Valor contable A/F 02** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.
3. Haga clic en el botón **Imprimir** o **Vista previa**.  

## <a name="see-also"></a>Consulte también
[Activos fijos](fa-manage.md)  
[Configurar activos fijos](fa-setup.md)  
[Finanzas](finance.md)  
[[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

