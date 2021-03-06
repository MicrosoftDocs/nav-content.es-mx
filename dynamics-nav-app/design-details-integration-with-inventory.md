---
title: "Detalles de diseño: Integración con inventario"
description: "Las áreas de aplicación de Gestión de almacén e Inventario interactúan entre sí en el inventario físico y en el ajuste de inventario o de almacén."
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
ms.openlocfilehash: ca9a1b5b1ea20fc125107f3fb5b7a74814a85837
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-integration-with-inventory"></a>Detalles de diseño: Integración con inventario
Las áreas de aplicación de Gestión de almacén e Inventario interactúan entre sí en el inventario físico y en el ajuste de inventario o de almacén.  
  
## <a name="physical-inventory"></a>Physical Inventory  
 La ventana **Diario de inventario físico de almacén** se usa en la ventana **Diario inventario físico** para todas las ubicaciones de almacén avanzadas. Se calcula el inventario en el nivel de ubicación y se proporciona una lista impresa al empleado del almacén. La lista muestra los productos en los que se deben contar las ubicaciones.  
  
 El empleado de almacén introduce la cantidad contada en la ventana **Diario de inventario físico de almacén** y, a continuación, registra el diario.  
  
 Si la cantidad contada es mayor que la cantidad en la línea del diario, se registra un movimiento para esta diferencia desde la ubicación de ajuste predeterminada a la ubicación contada. Esto aumenta la cantidad en la ubicación contada y reduce la cantidad en la ubicación de ajuste predeterminada.  
  
 Si la cantidad contada es menor que la cantidad en la línea del diario, se registra un movimiento para esta diferencia desde la ubicación contada a la ubicación de ajuste predeterminada. Esto reduce la cantidad en la ubicación contada y aumenta la cantidad en la ubicación de ajuste predeterminada.  
  
 En las configuraciones avanzadas de almacén, el valor del campo **Cantidad (calculada)** se recupera de los movimientos de producto, y valor del campo **Cantidad (inventario físico)** se recupera de los movimientos de almacén, excepto el contenido de la ubicación de ajuste. El campo **Cantidad** especifica la diferencia entre los dos primeros campos, que deben ser iguales al contenido de la ubicación de ajuste.  
  
 Cuando se registra el diario de inventario físico, se actualizan el inventario y la ubicación de ajuste predeterminada.  
  
### <a name="warehouse-adjustments-to-the-item-ledger"></a>Ajustes de almacén en los movimientos de productos  
 Use la ventana **Diario de producto** y la función **Calcular ajuste almacén** para ajustar el inventario en el movimiento de producto según un ajuste que se ha realizado en la cantidad de producto en una ubicación de almacén. Para crear un vínculo entre el inventario y el almacén, debe definir una ubicación de ajuste predeterminado por ubicación.  
  
 La ubicación de ajuste predeterminado registra los productos en el almacén al registrar una entrada de existencias. No obstante, si se registra una disminución, la cantidad en la ubicación predeterminada también disminuye. En ambos casos, se crean movimientos de producto y movimientos de almacén.  
  
> [!NOTE]  
>  La ubicación de ajuste no se incluye en el cálculo de disponibilidad.  
  
 Si desea ajustar el contenido de la ubicación, puede utilizar el diario de productos de almacén, desde el cual podrá introducir el número de producto, el código de la zona, el código de ubicación y la cantidad que se desee ajustar.  
  
 Si introduce una cantidad positiva y registra la línea, el inventario almacenado en la ubicación se incrementará, y la cantidad de la ubicación de ajuste predeterminada se reducirá en consecuencia.  
  
## <a name="see-also"></a>Consulte también  
 [Detalles de diseño: Gestión de almacén](design-details-warehouse-management.md)   
 [Detalles de diseño: Disponibilidad en el almacén](design-details-availability-in-the-warehouse.md)
