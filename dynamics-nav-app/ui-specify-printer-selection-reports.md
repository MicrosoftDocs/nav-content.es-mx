---
title: "Especificar selección de impresora para informes"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 55b48aef2bc108ced7f581f0ff6c11263ee467df
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
    
# <a name="specify-printer-selection-for-reports"></a>Especificar selección de impresora para informes
Puede configurar los informes para que se deban imprimir en una impresora específica. A continuación, se indican algunos usos de la selección de la impresora: 

- Puede imprimir informes en papel con membrete especial de la empresa.
- Puede imprimir informes en distintos tamaños en papel.
- Puede imprimir informes en la impresora predeterminada de un empleado especificado.

Puede usar la ventana **Selección de impresoras** para establecer valores diferentes para obtener una salida distinta. Si establece una selección de impresora específica, tendrá preferencia sobre una selección de impresora más general. Por ejemplo, puede definir una selección de impresora que tenga valores en los campos **Id. usuario**, **Id. informe** y **Nombre impresora**. Esta selección de impresora tiene preferencia sobre una selección de impresora que tenga entradas en blanco en los campos **Id. usuario** o **Id. informe**. 

La tabla siguiente describe la combinación de valores que especificar al configurar selecciones de impresora para un informe.

|Para                                                 |Establecer los valores siguientes                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|Imprimir un informe en una impresora específica para todos los usuarios |Especifique los valores de los campos **Id. informe** y **Nombre impresora** y deje en blanco el campo **Id. usuario**.|
|Imprimir todos los informes en una impresora específica para un usuario específico|Especifique los valores de los campos **Id. usuario** y **Nombre impresora** y deje en blanco el campo **Id. informe**.|
|Establecer la impresora predeterminada para todos los informes|Especifique un valor en el campo **Nombre impresora** y deje en blanco los campos **Id. usuario** e **Id. informe**.|
|Imprimir un informe específico en la impresora predeterminada del usuario|Especifique un valor en el campo **Id. informe** y deje en blanco los campos **Id. usuario** y **Nombre impresora**.|
|Imprimir un informe específico en una impresora concreta para un usuario específico|Especifique los valores de los tres campos.|

## <a name="see-also"></a>Consulte también
[Trabajar con Dynamics NAV](ui-work-product.md)

