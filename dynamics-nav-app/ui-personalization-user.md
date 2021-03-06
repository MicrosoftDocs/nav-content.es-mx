---
title: "Personalización del área de trabajo mediante el cliente web de Dynamics NAV"
description: Aprenda a personalizar la interfaz de usuario para que se adapte a su forma de trabajar.
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalize page, personalization, hide columns, remove fields, move fields
ms.date: 07/26/2017
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: c266842d4a64b62c90dab8db26f5206f9a10e4cc
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace-using-the-dynamics-nav-web-client"></a>Personalización del área de trabajo mediante el cliente web de Dynamics NAV
<!--NAV in the Web client-->
Puede *personalizar* el área de trabajo para que se adapte a su trabajo y preferencias cambiando las páginas de modo que muestren únicamente la información que necesite y donde la necesite. Los cambios de personalización que realice solo afectarán a su visualización y no a la de otros usuarios.

Según el tipo de página y lo que incluye, puede:

-   Agregar, mover y eliminar campos.
-   Agregar, mover y eliminar columnas de una lista.
-   Cambiar la inmovilización de panel de las columnas de una lista. La inmovilización de panel bloquea una o más columnas en el lado izquierdo de una lista para que estén siempre presentes, incluso cuando se desplaza horizontalmente.
-   Mover y eliminar pilas (iconos).
-   Mover y eliminar piezas. Las piezas son subdivisiones o áreas en una página que contienen elementos como múltiples campos, otra página, un gráfico o iconos.  

## <a name="to-personalize-a-page"></a>Para personalizar una página

1. En la esquina superior derecha, seleccione el icono ![Configuración](media/ui-experience/settings_icon_small.png "icono de Configuración para el área de tareas") y **Personalizar**.

    El banner **Personalización** aparece en la parte superior, lo que indica que puede empezar a realizar cambios.

    ![Modo Personalizar](media/ui_personalize_mode_small.png "Modo Personalizar")

2.  Vaya a una página que desee personalizar.

    Si ve un icono de bloqueo en el banner, vea [Por qué se ha bloqueado la página](ui-personalization-locked.md) para obtener más información.

3.  Señale un área que desee personalizar, como un encabezado de campo o columna en una lista. Todo lo que se pueda personalizar se resalta inmediatamente con una flecha o un borde.
<!--
    -  If a component can be personalized, an arrow head (![Personalization indicator arrow left](media/ui_personalize_arrow_left.png "Personalization indicator arrow left") or ![Personalization indicator arrow down](media/ui_personalize_arrow_down.png "Personalization indicator arrow down")) appears.
    -   If the component is a part, the extent of the part is indicated by a border.
    -   The freeze pane in a list is indicated by a vertical line along the entire right-side of the last column of the freeze pane.
    -->

4.  Utilice esta tabla para que le ayude a realizar cambios:     <table>
        <tr><th>Qué desea hacer</td><th>Cómo hacerlo</th></tr>
        <tr><td>Mueva algo, un campo, una columna de la lista, un icono o una pieza</td><td> Señale en cualquier lugar qué desea mover y arrástrelo a su nueva ubicación. La ubicación se indica con una fina línea vertical u horizontal.</td></tr>
        <tr><td>Elimine algún elemento</td><td>Seleccione la punta de flecha y elija <b>Eliminar</b>. </td></tr>
        <tr><td>Agregar un campo o columna</td><td>En el banner <b>Personalización</b>, elija <b>Más</b> y seleccione <b>Campo</b>.<br /></br>El panel <b>Agregar campo a página</b> se abre a la derecha. Muestra los campos que se pueden agregar a la página. Los campos marcados como <b>Colocado</b> ya están en la página. Los campos marcados como <b>Listo</b> aún no están en la página.<br /></br>Para agregar un campo, arrástrelo de panel a la ubicación que desee. La ubicación se indica con una fina línea vertical u horizontal.</td></tr>
        <tr><td>Cambiar la inmovilización de panel de una lista a otra columna</td><td>Seleccione la punta de la flecha de la columna que desee establecer como la última de la inmovilización de panel y, a continuación, elija <b>Establecer inmovilización de panel</b>.<br /><br/>Si desea volver a configurar la inmovilización de panel en su ubicación original diseñada, seleccione la punta de flecha para la columna actual y elija <b>Borrar inmovilización de panel</b>. Nota: No puede eliminar la inmovilización de panel original. Siempre habrá una inmovilización de panel que incluya al menos una columna.</td></tr>
      </table>

    > [!IMPORTANT]  
    >   No puede modificar una lista si se muestra como mosaicos. Primero debe cambiar la página a la vista de lista mediante el icono ![Mostrar como lista](media/ui_show_as_list_icon.png "Mostrar como lista de flecha izquierda").

5.  Puede seguir realizando cambios en la misma página o moverse a otra página. Los cambios se guardan automáticamente a medida que los crea. Cuando haya terminado, en el banner **Personalización**, elija **Hecho**.

## <a name="clear-personalization-to-change-a-page-back-to-its-original-layout"></a>Desactive la personalización para volver a cambiar una página al diseño original
En algún momento, es posible que desee borrar todos los cambios de personalización que hizo en esta página a lo largo del tiempo para que la página parezca como estaba al principio. Para ello, en el banner **Personalización**, elija **Más** y, a continuación, **Borrar personalización**.

## <a name="personalization-in-detail"></a>Personalización detallada
Para ayudarle a comprender mejor la personalización, le presentamos algunos consejos.  
-   Cuando realice cambios en una página de ficha que abre de una lista, los cambios tendrán efecto en todos los registros que abra de esa lista. Por ejemplo, digamos que abre un cliente específico desde la página de la lista Clientes y la personaliza agregando un campo. Cuando abra otros clientes de la lista, también se mostrará el campo que agregó.
-   Los cambios realizados tendrán efecto en todas las áreas de tareas. Por ejemplo, si realiza un cambio en la lista Clientes cuando el área de tareas está establecida en Administrador empresarial, también verá el cambio en la lista Clientes cuando el área de tareas esté configurada en Procesador de órdenes de venta.
-   Los cambios de una página realizados en un panel tendrán efecto en la página donde se muestre.  
-   Solo puede agregar campos y columnas de una lista predefinida, que está basada en la página. No puede crear campos ni columnas nuevos.

## <a name="see-also"></a>Consulte también
[Visión general de la personalización](ui-personalization-overview.md)  
[Administrar la personalización](ui-personalization-manage.md)  
[Trabajar con [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-work-product.md)  
[Procedimiento: Cambiar el área de tareas](change-role.md)  

