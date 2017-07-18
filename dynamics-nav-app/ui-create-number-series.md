---
title: "Crear numeración"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 22b3bcf71c99e106527d6bfa35478045d29b9629
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="create-number-series"></a>Crear numeración

Para cada empresa configurada, se necesitan asignar códigos de identificación exclusivos a elementos como cuentas de contabilidad, cuentas de proveedores y clientes, facturas y documentos. La numeración es importante no sólo para la identificación. Un sistema de numeración bien diseñado también permite facilitar la gestión y el análisis de la empresa, y puede reducir el número de errores que se producen en la introducción de datos.

Puede configurar un sistema de numeración completo con un número ilimitado de números de serie. Puede utilizar números de serie para todos los tipos de documentos y diarios, así como para los datos maestros como clientes, productos y proyectos.

Es posible combinar el uso de series numéricas con la numeración manual.

Para crear un sistema numérico, establezca uno o varios códigos para cada tipo de datos maestros o documento. Por ejemplo, puede establecer un código para la numeración de clientes, otro para la numeración de facturas de venta y aún otro para la numeración de documentos en los diarios generales.

Tras establecer un código, debe establecer al menos una línea de serie numérica. Ésta contiene información tal como el primer y último número de la serie y la fecha de inicio. Puede establecer más de una línea de serie numérica por código, con una fecha de inicio diferente para cada una. La serie se usará de manera consecutiva, a partir de la serie de cada fecha de inicio correspondiente.

Si desea usar más de un código de serie numérica para un tipo de datos maestros, por ejemplo, usar una serie numérica diferente para categorías de productos, puede establecer relaciones de series numéricas.

Además de los números que se asignan manualmente o mediante el sistema de numeración, a todas las transacciones (movimientos) se les asignan números consecutivos. Estos números se pueden ver en el campo **N.º mov.** de todas las ventanas de movimiento. Estos números no se pueden modificar ni eliminar.

## <a name="to-create-relationships-between-number-series"></a>Para crear relaciones entre números de serie
Si ha configurado más de un código de número de serie para el mismo tipo de información básica o transacciones, puede crear relaciones entre los códigos. Esta característica puede servirle de ayuda para decidir entre un código u otro cuando utilice un número.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Nos. serie** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la línea con las series numéricas que desea insertar para crear relaciones y, a continuación, elija **Relaciones**.
3. En el campo **Código serie**, escriba el código del número de serie con el que desee relacionar la serie seleccionada en el paso 2.
4. Agregue una línea para cada código que desee relacionar con el número de serie seleccionado.
5. Cierre la ventana.

En lo sucesivo, cuando configure algo que requiera un número, podrá utilizar las relaciones que haya creado para seleccionar uno de los números de serie relacionados.

## <a name="see-also"></a>Consulte también
[Trabajar con Dynamics NAV](ui-work-product.md)

