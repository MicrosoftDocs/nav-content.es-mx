---
title: Asignar las ubicaciones predefinidas a los productos
description: "Si utiliza ubicaciones en un almacén, la asignación de ubicaciones genéricas a sus productos puede facilitar el proceso de envío, recepción y movimiento de sus productos. Cuando se asigna una ubicación genérica a un producto, se sugiere esta ubicación cada vez que se inicia una transacción de este producto."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c046cb3631cd690ba4bf4a1f1147f6e03d7cec9a
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-assign-default-bins-to-items"></a>Procedimiento: asigne las ubicaciones predefinidas a los productos
Si utiliza ubicaciones en un almacén, la asignación de ubicaciones genéricas a sus productos puede facilitar el proceso de envío, recepción y movimiento de sus productos. Cuando se asigna una ubicación genérica a un producto, se sugiere esta ubicación cada vez que se inicia una transacción de este producto. Las ubicaciones genéricas se definen en la ventana **Contenido ubicación**.  

## <a name="to-assign-a-default-bin-to-an-item"></a>Asignar una ubicación predeterminada a un producto
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Hoja trabajo creación contenido ubicación** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene la información del código de ubicación y del artículo para cada ubicación que desee configurar como valor predeterminado para un artículo. Asegúrese de seleccionar el campo **Predeterminado**.  
3.  Seleccione la acción **Crear contenido ubicación**. Las ubicaciones ya están asignadas a su producto.  

> [!NOTE]  
>  Cuando se ubica un producto, si el producto no tiene asignada una ubicación genérica, se asignará aquélla en la que se ubique como genérica.  

## <a name="to-change-the-default-bin-for-an-item"></a>Para cambiar las ubicaciones predefinidas de los productos  
Puede que tenga que cambiar la asignación de la ubicación predeterminada de un artículo o que tenga que asignar una ubicación predeterminada a un artículo nuevo.    
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Contenidos ubicación** y, a continuación, seleccione el vínculo relacionado.  
2.  En el campo **Filtro almacén**, seleccione el código de almacén correspondiente.  
3.  Busque el movimiento de contenido de ubicación actual del producto y desactive la casilla **Genérica**.  
4.  Busque la línea de contenido de la ubicación que desea que sea la nueva ubicación genérica. Seleccione la casilla de verificación **Ubicación predeterminada**.  

> [!NOTE]  
>  Cuando se ubica un producto por primera vez, si el producto no tienen asignada una ubicación genérica, el sistema asignará la ubicación como ubicación genérica del producto.  

## <a name="see-also"></a>Consulte también  
[Gestión almacén](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

