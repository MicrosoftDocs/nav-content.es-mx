---
title: "Detalles de diseño: Diseño de seguimiento de productos"
description: "En este tema se describe el diseño detrás del seguimiento de producto en [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, item, tracking, tracing
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: acbb706d154f164c4e33e0bebaf84cd5a47862cc
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-item-tracking-design"></a>Detalles de diseño: Diseño de seguimiento de productos
En la primera versión de seguimiento de productos de [!INCLUDE[d365fin](includes/d365fin_md.md)] 2.60, los números de serie o de lote se registraban directamente en los movimientos de producto. Este diseño proporcionó información de disponibilidad completa y un seguimiento sencillo del historial de movimientos, pero carecía de flexibilidad y funcionalidad.  

A partir de [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.00, la funcionalidad de seguimiento de productos pasa a ser una estructura de objetos independiente con vínculos complejos a documentos registrados y movimientos de producto. Este diseño era flexible y con muchas funcionalidades, pero los movimientos de seguimiento de producto no intervenían completamente en los cálculos de disponibilidad.  

Desde [!INCLUDE[d365fin](includes/d365fin_md.md)] 3,60, la funcionalidad del seguimiento de productos está integrada con el sistema de reservas, que controla la reserva, el seguimiento de pedidos y los mensajes de acciones. Para obtener más información, consulte "Detalles de diseño: Reserva, seguimiento de pedidos y mensajes de acciones” en “Detalles de diseño: Planificación de aprovisionamiento”.  

Este último diseño incorporar los movimientos de seguimiento de producto en los cálculos de disponibilidad total en todo el sistema, incluida la planificación, la fabricación y el almacenamiento. El antiguo concepto de transferir los números de serie y de lote a los movimientos de productos se vuelve a introducir para garantizar un acceso sencillo al historial de datos para realizar el seguimiento de productos. En relación con las mejoras del seguimiento de productos en [!INCLUDE[d365fin](includes/d365fin_md.md)] 3.60, el programa de reservas se ha ampliado a entidades de la red que no son pedidos, como diarios, facturas y abonos.  

Con la adición de los números de serie o de lote, el sistema de reservas controla los atributos de producto permanentes, a la vez que también controla los vínculos intermitentes entre el suministro y la demanda en forma de movimientos de seguimiento de pedidos y movimientos de reserva. Otra característica distinta de los números de serie o de lote comparados con los datos convencionales de reserva es el hecho de que se pueden registrar, tanto parcial como totalmente. Por lo tanto, la tabla **Mov. reserva** (T337) ahora funciona con una tabla relacionada, la tabla **Especificación seguimiento** (T336), que controla y muestra la suma de las cantidades de seguimiento de producto activas y registradas. Para obtener más información, consulte [Detalles de diseño: registros de seguimiento de productos históricos frente a activos](design-details-active-versus-historic-item-tracking-entries.md).  

En el diagrama siguiente se describe el diseño de la funcionalidad de seguimiento de productos en [!INCLUDE[d365fin](includes/d365fin_md.md)].  

![Diseño seguimiento de productos](media/design_details_item_tracking_design.png "design_details_item_tracking_design")  

El objeto de registro central se ha rediseñado para controlar la subclasificación única de una línea de documento con el formato de números de serie o de lote, y se han agregado tablas de relación especiales para crear relaciones de uno a varios entre los documentos registrados y sus movimientos de producto y de valoración divididos.  

La unidad de código 22, **Diario de productos – Línea de registro**, divide ahora el registro según los números de seguimiento de producto que se especifican en la línea de documento. Cada número de seguimiento de producto único en la línea crea su propio movimiento para el producto. Esto significa que el vínculo desde la línea de documento registrado a los movimientos de producto asociados ahora es una relación de uno a varios. Esta relación se controla mediante las siguientes tablas de relaciones de seguimiento de producto.  

|Campo|Descripción|  
|---------------|---------------------------------------|  
|**Relación mov. producto** (T6507)|Relaciona las líneas enviadas o recibidas a los movimientos de producto|  
|**Relación mov. valor** (T6508)|Relaciona las líneas facturadas con los movimientos de valoración|  

Para obtener más información, consulte [Detalles de diseño: Estructura de registro de seguimiento de productos](design-details-item-tracking-posting-structure.md).  

## <a name="see-also"></a>Consulte también  
[Detalles de diseño: Seguimiento de productos](design-details-item-tracking.md)

