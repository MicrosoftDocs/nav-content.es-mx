---
title: "Convertir las ubicaciones existentes en ubicaciones de almacén"
description: "Puede activar una ubicación de inventario existente para utilizar zonas y ubicaciones, y para operar como ubicación de almacén."
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
ms.openlocfilehash: 16f1d8ac06c39361ee00e8c7514a282ad4d709e5
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-convert-existing-locations-to-warehouse-locations"></a>Procedimiento: convierta las ubicaciones existentes en ubicaciones de almacén
Puede activar una ubicación de inventario existente para utilizar zonas y ubicaciones, y para operar como ubicación de almacén.  

El proceso para activar un almacén para la operación de almacén crea movimientos de almacén iniciales para la ubicación de ajuste de almacén para todos los productos con existencias en el almacén. Estos movimientos iniciales se equilibrarán cuando se introduzcan los movimientos de inventario físicos después de que se ejecute el proceso.  

Puede crear zonas y ubicaciones antes o después de la conversión. La única ubicación que debe crear antes de la conversión es la que se va a utilizar como la futura ubicación de ajuste.  

> [!IMPORTANT]  
>  Para borrar todo el inventario negativo y los documentos de almacén abiertos antes de convertir la ubicación para la gestión de almacén, puede ejecutar un informe para identificar los artículos con el inventario negativo y abrir los documentos de almacén para la ubicación. Para obtener más información acerca de cómo crear picking de inventario, vea Comprobar el inventario negativo.  

## <a name="to-enable-an-existing-location-to-operate-as-a-warehouse-location"></a>Para activar una ubicación para que funcione como una ubicación de almacén  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Crear un almacén** y, a continuación, seleccione el vínculo relacionado.  
2.  En el campo de **Cód. almacén**, especifique la ubicación que desea activar para el procesamiento de almacén.  
3.  En el campo de **Cód. ubicación ajuste**, especifique la ubicación en el lugar de almacenamiento en donde se almacenan los movimientos de almacén no sincronizados. Para obtener más información, consulte “Sincronizar las entradas ajustadas de almacén con los movimientos de productos correspondientes" en [Procedimiento: Recuento, ajuste, y reclasificación de inventario](inventory-how-count-adjust-reclassify.md).  

    Mediante los movimientos de producto pendientes para el almacén especificado, se crean líneas de diario de almacén que suman las combinaciones de Nº producto, Cód. variante, Cód. unidad medida y, si es necesario, Nº lote y Nº serie en los movimientos del diario de productos. Entonces, se registrarán las líneas del diario de almacén. Este registro crea movimientos de almacén que colocan el inventario en la ubicación de ajuste de almacén. También se configura el **Cód. ubicación ajuste** en la ficha de almacén.  

4.  Para ver los productos que se han añadido a la ubicación de ajuste durante el proceso, ejecute el informe **Ubic. ajuste alm**.  
5.  Una vez que se ha completado el trabajo por lotes **Crear un almacén**, debe llevar a cabo y registrar el inventario físico del almacén. Para obtener más información, consulte [Procedimiento: Recuento, ajuste, y reclasificación de inventario](inventory-how-count-adjust-reclassify.md).  

> [!NOTE]  
>  Se recomienda que ejecute el proceso **Crear un almacén** en un momento en el que no tenga impacto en el trabajo diario del sistema. Esta tarea procesa todos los movimientos de la tabla **Mov. producto** y si hay un gran número de movimientos de productos, la tarea puede durar varias horas.  

 Para esas ubicaciones que no utilizaron documentos de gestión de almacenes antes de la conversión, debe volver a abrir y lanzar los documentos de origen que se recibieron parcialmente o se enviaron parcialmente antes de la conversión.  

## <a name="see-also"></a>Consulte también  
[Gestión de almacenes](warehouse-manage-warehouse.md)  
[Grupos contables inventario](inventory-manage-inventory.md)  
[Configuración de la gestión del almacén](warehouse-setup-warehouse.md)     
[Gestión de ensamblaje](assembly-assemble-items.md)    
[Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

