---
title: "Personalización de su área de trabajo: información general"
description: Aprenda a personalizar la interfaz de usuario para que se adapte a su forma de trabajar.
documentationcenter: 
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 04334d3bb50b37b9643b848ca4f59b015f03ad04
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace---overview"></a>Personalización de su área de trabajo: información general
Puede *personalizar* el área de trabajo para que se adapte a su trabajo y preferencias cambiando el diseño de las páginas de modo que muestren únicamente la información que necesite y donde la necesite. Los cambios de personalización que realice solo afectarán a su visualización y no a la de otros usuarios.

Puede personalizar el área de trabajo mediante [!INCLUDE[nav_windows_md](includes/nav_windows_md.md)] y [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Los cambios de personalización que realice también se verán en [!INCLUDE[nav_phone_md](includes/nav_phone_md.md)] y [!INCLUDE[nav_web_md](includes/nav_phone_md.md)].
  
> [!NOTE]  
> Es posible que el administrador de su empresa ya haya personalizado su interfaz de usuario para un diseño específico del rol para todos los usuarios que tienen el mismo perfil que usted y usen la misma área de tareas. Las personalizaciones que realice en su área de trabajo se guardan en su cuenta de usuario, por lo que se conservarán incluso si un administrador presenta un nuevo conjunto de diseños específicos para cada función en su empresa. Para obtener más información, consulte [Configuración de la interfaz de usuario](admin-configure-user-interface.md).

## <a name="comparing-personalization-in-the-dynamics-nav-windows-and-web-clients"></a>Comparación de la personalización del cliente de Windows y el cliente web de Dynamics NAV
Dependiendo de la página, puede personalizar muchas partes de la interfaz de usuario, como qué campos o columnas se muestran y dónde se sitúan, las acciones que se incluyen en la cinta de opciones, y más. Muchas de estas acciones las puede realizar en el cliente de Windows y el cliente web. En la tabla siguiente se proporciona una visión general de las capacidades de personalización de cada cliente.

|  Personalice  ||  Cliente de Windows  |  Cliente web  |
|---------------|-|------------------|--------------|
|Campos de fichas desplegables||||
||Agregar, mover, eliminar |x|x|
||Mostrar en la cabecera contraída|x||
||Ocultar en la acción **Mostrar más campos**|x||
|Listas o líneas de documento ||||
||Agregar, mover, eliminar columnas  |x|x|
||Agregar, mover, eliminar inmovilización de panel  |x|x|
|Cuadros informativos|||
||Mover, eliminar|x|x|
||Agregar|x||
||Agregar, mover, eliminar campos|x|x|
|Pilas||||
||Mover, eliminar|x|x|
||Agregar |x||
|Gráficos||||
||Mover, eliminar|x|x|
||Agregar|x| |
|Cinta de opciones y acciones||x||
|Panel de navegación||x||

Otra diferencia es que al personalizar mediante el cliente de Windows, puede tener varias versiones personalizadas de la misma página, basadas en diferentes puntos de acceso a la página. Por ejemplo, la página **Órdenes venta** personalizada para que se vea diferente al abrirse desde la página **Ficha cliente** en lugar de cuando se abre desde la página **Área de tareas Procesador de órdenes de venta**. Cuando personaliza una página mediante el cliente web, solo hay una versión personalizada por página, por lo que los cambios se verán sin importar de dónde la abra.

##  <a name="PersonalizationWinWeb"></a>Trabajar con la personalización entre cliente de Windows y el cliente web de Dynamics NAV
Antes de comenzar a personalizar las páginas, es importante comprender cómo funciona la personalización entre el cliente de Windows y el cliente web. Si únicamente utilizará uno de los dos clientes, esta información no le interesará. Sin embargo, será importante si comienza a personalizar las páginas mediante ambos clientes o al cambiar de usar el cliente de Windows a usar el cliente web de forma permanente.  

-   Si usa el cliente de Windows para personalizar una página específica desde el principio, también verá los cambios de personalización en la página en el [!INCLUDE[nav_web_md](includes/nav_web_md.md)].

-   Siempre que continúe utilizando el cliente de Windows para personalizar la página, los cambios de personalización que realice también tendrán efecto en la página del cliente web.

-   Sin embargo, cuando empiece a personalizar la página mediante el uso del cliente web, la personalización de esa página se separará entre los dos clientes, y tendrá una versión personalizada para cada cliente. En el cliente web, se borrarán las personalizaciones anteriores de la página, lo que significa que la página volverá a su diseño original y básicamente comenzará a personalizar la página desde cero. Las personalizaciones anteriores del cliente de Windows no cambian.

- A partir de este momento, personalizará la página en el cliente de Windows y el cliente web de forma separada, lo que significa que la página se verá diferente en cada cliente. Los clientes de teléfono y tableta mostrarán las mismas personalizaciones de la página que el cliente web.  

> [!Tip]  
>Si abre la página **Eliminar personalización usuario**, podrá ver todas las páginas personalizadas por los usuarios. La columna **Personalización heredada** columna le proporciona una indicación de si la personalización se realizó en el cliente de Windows o en el cliente web. Si hay una marca de verificación en la columna, la personalización se realizó en el cliente de Windows (o en el cliente web anterior a [!INCLUDE[navnow_md](includes/navnow_md.md)]).

## <a name="see-also"></a>Consulte también
[Personalización del área de trabajo para el cliente de Windows de Dynamics NAV](ui-personalization-windows-client.md)  
[Personalización del área de trabajo para el cliente web de Dynamics NAV](ui-personalization-user.md)  
[Administrar la personalización](ui-personalization-manage.md)  
[Personalización de Dynamics NAV](ui-customizing-overview.md)  

