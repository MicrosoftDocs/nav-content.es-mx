---
title: "Detalles de diseño: Parámetros de la planificación"
description: "En este tema se describen los distintos parámetros de planificación que puede usar en [!INCLUDE[d365fin](includes/d365fin_md.md)]."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: planning, design
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7da4796793b793ab37d6d2660b9200bb5e684d9b
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="design-details-planning-parameters"></a>Detalles de diseño: Parámetros de la planificación
En este tema se describen los distintos parámetros de planificación que puede usar en [!INCLUDE[d365fin](includes/d365fin_md.md)].  

La forma en que el sistema de planificación controla el suministro de productos se determina mediante distintas opciones de configuración de la ficha de producto o UA, y las opciones de la configuración de fabricación. En la tabla siguiente se muestra cómo se usan estos parámetros para la planificación.  

|Propósito|Parámetro|  
|-------------|---------------|  
|Definir si se va a planificar el producto|Directiva reorden = En blanco|  
|Definir cuándo hacer la reorden|Ciclo<br /><br /> Punto de reorden<br /><br /> Plazo de seguridad|  
|Definir qué cantidad de la reorden|Inventario de seguridad<br /><br /> Directiva reorden:<br /><br /> -   Cdad. fija reordenada frente a Cantidad a pedir<br />-   Cantidad máxima más inventario máximo<br />-   Pedido<br />-   Lote a lote|  
|Optimizar cuando se produzca la reorden y según la cantidad de reorden|Periodo de reprogramación<br /><br /> Periodo de acumulación de lotes<br /><br /> Periodo de tolerancia|  
|Modificar los pedidos de suministro|Cantidad mínima pedido<br /><br /> Cantidad máxima pedido<br /><br /> Múltiplos de pedido|  
|Delimitación del producto planificado|Directiva fabricación:<br /><br /> -   Fab-contra-stock<br />-   Fab-contra-pedido|  

## <a name="define-if-the-item-will-be-planned"></a>Definir si se va a planificar el producto  
Para incluir un producto/UA en el proceso de planificación, debe tener una directiva de reorden, de lo contrario, se debe planificación manualmente, por ejemplo, con la característica Planificación de pedidos.  

## <a name="define-when-to-reorder"></a>Definir cuándo hacer la reorden  
Por lo general, las propuestas de reorden solo se lanzan cuando la cantidad disponible proyectada ha caído o está por debajo de una cantidad determinada. Esta cantidad se define mediante el punto de reorden. De lo contrario, será cero. Se puede ajustar cero si se especifica un inventario de seguridad. Si el usuario ha definido un plazo de seguridad, hará que la propuesta se entregue en el periodo anterior a la fecha de vencimiento requerida.  

Las directivas de punto de reorden (**Cdad. fija reordenada** y **Cdad. máxima**) usan el campo **Ciclo**, donde el nivel de inventario se comprueba después de cada ciclo. El primer ciclo comienza en la fecha inicial de planificación.  

> [!NOTE]  
>  Al calcular los ciclos, el sistema de planificación ignora los calendarios de trabajo que se definen en el campo **Código de calendario base** de las ventanas **Información de la empresa** y **Tarjeta de ubicación**.  

El plazo de seguridad genérico, en la ventana **Configuración fabricación**, se debe configurar en un día como mínimo. Se puede saber la fecha de vencimiento de la demanda, pero no el tiempo de vencimiento. La planificación realiza la programación hacia atrás para satisfacer la demanda bruta y, si no se ha definido ningún plazo de seguridad, las mercancías pueden llegar demasiado tarde para satisfacer la demanda.  

Tres campos de periodo de reorden adicionales, **Periodo de reprogramación**, **Periodo de acumulación de lotes** y **Periodo de tolerancia**, también desempeñan un rol en la definición de la necesidad de reordenar. Para obtener más información, vea la sección "Optimizar cuando y qué cantidad se reordena".  

## <a name="define-how-much-to-reorder"></a>Definir qué cantidad de la reorden  
Si el sistema de planificación detecta necesidad de reorden, la directiva de reorden seleccionada se utiliza para determinar el momento del pedido y la cantidad correspondiente.  

Independiente de la directiva de reorden, el sistema de planificación sigue normalmente esta lógica:  

1. La cantidad de la propuesta de pedido se calcula para cubrir el nivel de inventario mínimo especificado del producto, normalmente el inventario de seguridad. Si no se especifica nada, el nivel de inventario mínimo es cero.  
2. Si las existencias disponibles proyectadas se encuentran por debajo de la cantidad de inventario de seguridad, se sugiere un pedido de aprovisionamiento con programación retroactiva. La cantidad de pedido al menos llenará el inventario de seguridad, y se puede aumentar mediante la demanda bruta dentro del ciclo, mediante la directiva de reorden y los modificadores de pedido.  
3. Si el inventario proyectado se encuentra por debajo del punto de reorden o lo ha alcanzado (calculado a partir de cambios agregados dentro del ciclo) y por encima del inventario de seguridad, se sugiere un pedido de excepción con programación anticipada. Tanto la demanda bruta que debe satisfacerse como la directiva de reorden determinarán la cantidad del pedido. Como mínimo, la cantidad del pedido coincidirá con el punto de reorden.  
4. Si hay más demanda bruta que vence antes de la fecha de fin de la propuesta de pedido anticipado y esta demanda lleva a las existencias disponibles proyectadas actualmente calculadas por debajo de la cantidad de inventario de seguridad, la cantidad del pedido se aumenta para suplir el déficit. El pedido de suministro sugerido se programa hacia atrás a partir de la fecha de vencimiento de la demanda bruta que habría infringido el inventario de seguridad.  
5. Si el campo **Ciclo** no está relleno, solo se agregará la demanda bruta en la misma fecha de vencimiento.  

     Los siguientes campos de periodo de reorden también desempeñan un rol en la definición de la cantidad de reorden: **Periodo de reprogramación**, **Periodo de acumulación de lotes** y **Periodo de tolerancia**. Para obtener más información, vea la sección "Optimizar cuando y qué cantidad se reordena".  

### <a name="reordering-policies"></a>Directivas de reorden  
Las siguientes directivas de reorden afectan a la cuenta que recibirá la reorden.  

|Directiva reorden|Descripción|  
|-----------------------|---------------------------------------|  
|**Cdad. fija reordenada**|Como mínimo, la cantidad del pedido debe se igual a la cantidad de reorden. Puede aumentarse para satisfacer la demanda o el nivel de inventario deseado. Normalmente, esta directiva de reorden se usa con un punto de reorden.|  
|**Cdad. máxima**|La cantidad de pedido se calculará para cubrir el inventario máximo. Si se utilizan modificadores de cantidad, puede infringirse el inventario máximo. No es recomendable usar el ciclo junto con la cantidad máxima. Normalmente, el ciclo se anulará. Normalmente, esta directiva de reorden se usa con un punto de reorden.|  
|**Pedido**|Se calculará la cantidad de pedido para cubrir cada evento de demanda individual y el conjunto de demanda-suministro permanecerá vinculado hasta su ejecución. No se tiene en cuenta ningún parámetro de planificación.|  
|**Lote a lote**|La cantidad se calcula para cubrir la suma de la demanda que vence en el ciclo.|  

##  <a name="optimize-when-and-how-much-to-reorder"></a> Optimizar cuando se produzca la solicitud de reorden y según la cantidad de reorden  
Para obtener un plan de suministro racional, el planificador optimizará los parámetros de planificación para limitar las sugerencias de reprogramación, acumular demanda (cantidad dinámica de reorden) o evitar acciones de planificación insignificantes. Los siguientes campos de periodo de reorden contribuyen a optimizar el momento y la cantidad de reorden.  

|Campo|Descripción|  
|---------------------------------|---------------------------------------|  
|**Periodo de reprogramación**|Este campo se usa para determinar si el mensaje de acción debe reprogramar un pedido existente o bien cancelarlo y crear otro nuevo. El pedido existente se reprogramará en un periodo de reprogramación antes del suministro actual y hasta el periodo de reprogramación después del suministro actual.|  
|**Periodo de acumulación de lotes**|Con la directiva de reorden Lote a lote, este campo se usa para acumular varias necesidades de suministro en un pedido de suministro. Desde la fecha del primer aprovisionamiento planificado, el sistema acumula todas las necesidades de aprovisionamiento del periodo de acumulación de lote siguiente en un aprovisionamiento que se coloca en la fecha del primer aprovisionamiento. Demanda que está fuera del periodo de acumulación del lote no cubierta por este aprovisionamiento.|  
|**Periodo de tolerancia**|Este campo se usa para evitar la reprogramación menor del suministro existente fuera de plazo. Los cambios de la fecha de aprovisionamiento hasta un periodo de tolerancia a partir de la fecha de aprovisionamiento no generarán ningún mensaje de acción.<br /><br /> Como resultado, un delta positivo entre la nueva fecha de aprovisionamiento propuesta y la fecha de aprovisionamiento original será siempre mayor que el periodo de tolerancia.|  

El momento del periodo de reprogramación, el periodo de tolerancia y el periodo de acumulación de lotes se basa en una fecha de suministro. El ciclo se basa en la fecha de inicio de la planificación, tal como se muestra en la ilustración siguiente.  

![Elementos del ciclo](media/supply_planning_5_time_bucket_elements.png "supply_planning_5_time_bucket_elements")  

En los siguientes ejemplos, las flechas negras representan el aprovisionamiento existente (arriba) y demanda (abajo). Las flechas rojas, verdes y naranjas son sugerencias de planificación.  

**Ejemplo 1**: la fecha de modificación queda fuera del periodo de reprogramación, lo que hace que se cancele el aprovisionamiento existente. Se sugiere un nuevo aprovisionamiento para cubrir la demanda en el periodo de acumulación de lotes.  

![Periodo de reprogramación, Periodo de acumulación de lotes](media/supply_planning_5_recheduling_period_lot_accumulation_period.png "supply_planning_5_recheduling_period_lot_accumulation_period")  

**Ejemplo 2**: la fecha de modificación está dentro del periodo de reprogramación, lo que hace que se reprograme el aprovisionamiento existente. Se sugiere un nuevo aprovisionamiento para cubrir la demanda fuera del periodo de acumulación de lotes.  

![Periodo de reprogramación, Periodo de acumulación de lotes, Reprogramar](media/supply_planning_5_recheduling_period_lot_accum_period_reschedule.png "supply_planning_5_recheduling_period_lot_accum_period_reschedule")  

**Ejemplo 3**: hay una demanda en el periodo de tolerancia y la cantidad de aprovisionamiento en el periodo de acumulación de lotes coincide con la cantidad de aprovisionamiento. La siguiente demanda se queda sin cubrir y se sugieren un nuevo suministro.  

![Periodo de tolerancia, Periodo de acumulación de lotes](media/supply_planning_5_dampener_period_lot_accumulation_period.png "supply_planning_5_dampener_period_lot_accumulation_period")  

**Ejemplo 4**: hay una demanda en el periodo de tolerancia y el aprovisionamiento sigue en la misma fecha. No obstante, la cantidad de aprovisionamiento actual no es suficiente para cubrir la demanda en el periodo de acumulación de lotes, por lo que se sugiere aplicar una acción de cambio de cantidad para el pedido de aprovisionamiento existente.  

![Periodo de tolerancia, Periodo de acumulación de lotes, Cambiar cdad.](media/supply_planning_5_dampener_period_lot_accum_period_change_qty.png "supply_planning_5_dampener_period_lot_accum_period_change_qty")  

**Valores predeterminados:** el valor predeterminado del campo **Ciclo** y los tres campos del periodo de reorden están en blanco. Para todos los campos, excepto el campo **Periodo de tolerancia** esto significa 0D (cero días). Si el campo **Periodo de tolerancia** está en blanco, se usará el valor global en el campo **Periodo predet. amortiguador** en la ventana **Configuración fabricación**.  

## <a name="modify-the-supply-orders"></a>Modificar los pedidos de suministro  
Cuando se ha calculado la cantidad de la propuesta de pedido, uno o más de los modificadores de pedido pueden ajustarla. Por ejemplo, la cantidad de pedido máxima es mayor que o igual a la cantidad de pedido mínima, que es mayor que o igual al múltiplo de pedido.  

La cantidad se reduce si supera la cantidad de pedido máximo. A continuación, se aumenta si se encuentra por debajo de la cantidad de pedido mínima. Finalmente, se redondea hacia arriba de modo que coincida con un múltiplo de pedido especificado. Las cantidades pendientes utilizan los mismos ajustes hasta que la demanda total se haya convertido a propuestas de pedidos.  

## <a name="delimit-the-item"></a>Delimitación del producto  
La opción **Directiva fabricación** define los pedidos adicionales que propondrá el cálculo de MRP.  

Si utiliza la opción **Fab-contra-existencias**, los pedidos solo afectan al producto en cuestión.  

Si utiliza la opción **Fab-contra-pedido**, el sistema de planificación analizará la L.M. de producción del producto y creará propuestas de pedido vinculadas adicionales para los productos de nivel inferior que también se hayan definido como Fab-contra-pedido. Esto continúa siempre que haya productos de fabricación contra pedido en las estructuras de L.M. descendentes.  

## <a name="see-also"></a>Consulte también  
[Detalles de diseño: Gestión de directivas de reorden](design-details-handling-reordering-policies.md)   
[Detalles de diseño: Equilibrio de aprovisionamiento y demanda](design-details-balancing-demand-and-supply.md)   
[Detalles de diseño: Conceptos centrales del sistema de planificación](design-details-central-concepts-of-the-planning-system.md)

