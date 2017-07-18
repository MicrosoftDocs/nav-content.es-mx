---
title: Dimensiones
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: a1b38e74717e87bea6efb46f8f4e5236b6ec4e64
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

#<a name="dimensions"></a>Dimensiones
Las dimensiones son datos que añade a movimientos para clasificarlos para su análisis. Por ejemplo, puede tener dimensiones que indiquen de qué proyecto o departamento procede un movimiento.
A continuación, puede usar las dimensiones en lugar de tener que configurar cuentas contables generales independientes para cada departamento y proyecto. De este modo, dispondrá de una amplia información de análisis en sus datos sin tener que usar un complicado catálogo de cuentas.
Puede definir un número ilimitado de dimensiones con un número ilimitado de valores de dimensiones.  

Por ejemplo, debe configurar una dimensión que se llame *Departamento* y puede usarla junto con un valor de dimensión cuando registre documentos de ventas. A continuación, puede obtener más tarde los datos de inteligencia empresarial sobre qué artículos se han vendido y por qué departamentos, por ejemplo.
Cuantas más dimensiones configure y use, más detallados serán los informes en los que pueda basar sus decisiones empresariales. Por ejemplo, un movimiento de ventas individual puede incluir información de múltiples dimensiones sobre la cuenta en la que se ha registrado la venta del producto, el lugar donde se vendió el producto, la persona que lo vendió y la clase de cliente que realizó la compra.  

## <a name="using-dimensions"></a>Usar dimensiones
En un documento como una orden de venta, puede agregar información de dimensión de una línea en particular y del mismo documento. Por ejemplo, en la ventana **Orden de venta**, puede introducir valores de dimensión para las dos primeras dimensiones abreviadas directamente en el documento y puede agregar más información de dimensión si elige el botón **Dimensiones**.  
Si, en cambio, trabaja con un diario, también puede agregar información de dimensiones a un movimiento del mismo modo, si ha configurado dimensiones abreviadas como campos directamente en las líneas de diario.  
Puede configurar dimensiones predeterminadas para cuentas o tipos de cuenta, para que esas dimensiones o valores de dimensión se completen automáticamente.  

## <a name="dimension-sets"></a>Grupos de dimensiones
Un grupo de dimensiones es una combinación única de valores de dimensión. Se almacena como movimientos de grupo de dimensiones en la base de datos. Cada movimiento de grupo de dimensiones representa un valor de dimensión único. El grupo de dimensiones se identifica por medio de un id común del grupo de dimensiones que está asignado a cada movimiento de grupo de dimensiones que pertenece al grupo de dimensiones.  

Cuando crea una nueva línea de diario, cabecera de documentos o línea de documentos, puede especificar una combinación de valores de dimensión. En lugar de explícitamente guardar cada valor de dimensión en la base de datos, un Id. de grupo de dimensiones se asigna a la línea de diario, cabecera de documentos o línea de documentos para especificar el grupo de dimensiones.  

## <a name="see-also"></a>Consulte también
[Finanzas](finance-setup.md)  
[Configurar dimensiones](finance-setup-setup-dimensions.md)  

