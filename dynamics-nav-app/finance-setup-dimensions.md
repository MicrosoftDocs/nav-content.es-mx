---
title: Configurar dimensiones
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 1b7a293982dfc7ff73c163ad1711e2bce098e98e
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---

# <a name="set-up-dimensions"></a>Configurar dimensiones
Debe definir qué dimensiones y valores de dimensión desea utilizar en la empresa. También debe definir qué dimensiones desea utilizar como dimensiones abreviadas y globales. Debe pensar detenidamente qué dimensiones serán más eficaces como dimensiones globales y abreviadas para la empresa.  
Puede configurar todas las diferentes dimensiones de las que desee realizar un seguimiento en la ventana **Dimensiones**. Esta ventana contiene una línea para cada dimensión, como *Proyecto*, *Departamento*, *Área* y *Vendedor*.  

Para cada dimensión, también debe configurar los valores de dimensiones, por ejemplo, todos los departamentos de su empresa. Los valores de dimensiones se pueden configurar en una estructura jerárquica similar al catálogo de cuentas, de modo que los datos se puedan desglosar en diversos niveles de granularidad y se puedan totalizar subconjuntos de valores de dimensiones.  

Puede especificar dos dimensiones globales que estarán automáticamente disponibles en todas partes, por ejemplo en informes y procesos. También puede especificar seis dimensiones abreviadas que estarán disponibles como campo en diarios y líneas de documento. Las dimensiones restantes se pueden usar accediendo a una ventana independiente que muestre las dimensiones para la línea.  

Puede definir tantas dimensiones como necesite la empresa, así como definir un número ilimitado de valores de dimensión para cada dimensión. Se pueden utilizar todas las dimensiones que defina en los movimientos de diarios y documentos, así como en los procesos e informes relacionados con las dimensiones.  

## <a name="set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Configurar dimensiones predeterminadas para clientes, proveedores, y otras cuentas
Puede configurar una dimensión predeterminada para una determinada cuenta. El programa se copia al diario o documento cuando el campo de número de cuenta se rellena en la línea. Sin embargo, puede eliminar o cambiar el código en caso necesario. También puede hacer que una dimensión sea obligatoria, de forma que no sea posible registrar un movimiento con un tipo de cuenta específico salvo que la cuenta tenga un valor de dimensión asignado.  

Además, puede configurar una dimensión predeterminada para cada tipo de cuenta, así que este código se copia al diario o documento cuando el tipo de cuenta se rellena en la línea. Sin embargo, siempre puede cambiar el código del documento si es necesario.  

Finalmente, también puede hacer que una dimensión sea obligatoria, de forma que no sea posible registrar un movimiento con un tipo de cuenta específico salvo que la cuenta tenga un valor de dimensión asignado.

## <a name="see-also"></a>Consulte también
[Trabajar con dimensiones](finance-dimensions.md)  
[Configurar los procesos financieros más importantes](finance-setup-finance.md)

