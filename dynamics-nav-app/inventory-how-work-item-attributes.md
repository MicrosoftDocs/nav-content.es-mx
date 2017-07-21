---
title: 'Procedimiento: Trabajar con atributos de producto'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: eaf539f1d4d00c2cd5679f39f29a3428e33ee1fd
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-item-attributes"></a>Procedimiento: Trabajar con atributos de producto
Cuando los clientes hacen consultas sobre un producto, ya sea por correspondencia o en una tienda en línea integrada, pueden preguntar por las características como la altura y el año del modelo. Para proporcionar este servicio al cliente, puede asignar valores de atributo de producto de diferentes tipos a sus productos, que podrán usarse posteriormente en la búsqueda de productos.

También puede asignar los atributos de producto a categorías de producto que se aplican después a los productos que las utilizan. Para obtener más información, consulte [Procedimiento: Clasificar productos](inventory-how-categorize-items.md).

## <a name="to-create-item-attributes"></a>Para crear atributos de producto
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Atributos de producto** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Atributos de producto**, seleccione la acción **Nuevo**.
3. En la ventana **Atributos de producto**, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

**Nota**: Si selecciona **Opción** en el campo **Tipo**, puede seleccionar la acción **Valores de atributo de producto** para crear valores de atributo de producto. Para obtener más información, consulte la sección "Para crear valores de atributo de producto del tipo Opción".  

## <a name="to-create-values-for-item-attributes-of-type-option"></a>Para crear los valores de los atributos de producto del tipo Opción
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Atributos de producto** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Atributos de producto**, seleccione un atributo de producto del tipo Opción al que quiere asignarle un valor y, a continuación, seleccione la acción **Valores de atributo de producto**.
3. En la ventana **Valores de atributo de producto**, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

## <a name="to-assign-item-attributes-to-items"></a>Asignar un atributo de producto a productos
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Productos** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Producto**, seleccione el producto al que quiere asignarle un atributo de producto y, a continuación, seleccione la acción **Atributos**.
3. En la ventana **Valores de atributo de producto**, seleccione la acción **Nuevo**.
4. Seleccione el botón AssistEdit en el campo **Atributo** y seleccione un atributo de producto existente. De forma alternativa, elija la acción **Nuevo** para crear primero un nuevo atributo de producto como se explica en la sección "Para crear atributos de producto".
5. En el campo **Valor**, introduzca el valor del atributo de producto, como por ejemplo "2010" en el atributo Año de modelo.
6. Para los atributos de producto del tipo Opción, seleccione el botón AssistEdit en el campo **Valor** y seleccione un valor de atributo de producto. De forma alternativa, elija la acción **Nuevo** para crear primero un nuevo valor de atributo de producto como se explica en la sección "Para crear valores de atributo de producto del tipo Opción".
7. Repita los pasos del 4 al 6 para todos los atributos de producto que desea asignar al producto.

## <a name="to-assign-item-attributes-to-item-categories"></a>Asignar un atributo de producto a una categoría
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Categorías de producto** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Categoría de producto**, seleccione la categoría de producto al que quiere asignarle un atributo y, a continuación, seleccione la acción **Editar**.
3. En la ventana **Ficha de categoría de artículo**, en la ficha desplegable **Atributos**, seleccione la acción **Nuevo**.
4. Seleccione el botón AssistEdit en el campo **Atributo** y seleccione un atributo de producto existente. De forma alternativa, elija la acción **Nuevo** para crear primero un nuevo atributo de producto como se explica en la sección "Para crear un atributo de producto".
5. En el campo **Valor predeterminado**, seleccione el botón AssistEdit y seleccione un valor de atributo de producto.
6. Repita los pasos 4 y 5 para todos los atributos de producto que desea asignar a la categoría.

**Nota**: Las categorías de producto secundarias deben heredar los atributos de producto de las categorías principales. Esto está indicado en el campo **Origen de herencia** de la ficha desplegable **Atributos**. Para obtener más información, consulte [Procedimiento: Clasificar productos](inventory-how-categorize-items.md).

## <a name="to-filter-by-item-attributes"></a>Para filtrar por atributos de producto
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Productos** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Producto**, seleccione la acción **Filtrar por atributo**.
3. En la ventana **Filtrar productos por atributo** seleccione el botón AssistEdit en el campo **Atributo** y seleccione un atributo de producto.
4. En el campo **Valor**, seleccione el botón AssistEdit y seleccione un valor de atributo de producto para filtrar los productos.

    **Nota**: solo puede seleccionar los valores directamente para los atributos del producto que tienen valores fijos, como por ejemplo el Color. Para los atributos de producto que tienen valores variables, como por ejemplo el Ancho, debe especificar el valor del atributo de producto primero seleccionando una condición. Consulte el paso 5.
5. En el campo **Valor** para un atributo de producto variable, seleccione el botón AssistEdit.
6. En la ventana **Especificar valor de filtro**, en el campo **Condición**, haga clic en la flecha desplegable y seleccione una condición.
7. En el campo **Valor**, introduzca un valor de atributo para filtrar los productos.

    **Ejemplo**: Para filtrar los productos en que la descripción del material empieza por "azul", rellene los campos como se indica a continuación: campo **Atributo**: descripción de material; campo **Condición**: empieza por; campo **Valor**: azul.
8. Elija el botón **Aceptar**.   

Los productos de la ventana **Productos** se filtran por los valores de atributo de productos especificados.

## <a name="see-also"></a>Consulte también
[Procedimiento: Clasificar productos](inventory-how-categorize-items.md)    
[Registro de productos nuevos](inventory-how-register-new-products.md)  
[Gestionar inventario](inventory-manage-inventory.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

