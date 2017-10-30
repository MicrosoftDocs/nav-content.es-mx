---
title: "Configuración de la interfaz de usuario (IU) para los usuarios"
description: "Como administrador, configure la interfaz de usuario predeterminada de la empresa personalizando los diseños de página para los perfiles de usuario de la empresa."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize pages, configure user interface, customize UI
ms.date: 07/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7ba3d45a856eb38fe99fc5012b4e2f2d8609f9ce
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="configuring-the-user-interface-ui-for-users"></a>Configuración de la interfaz de usuario (IU) para los usuarios
Como administrador, podrá configurar la interfaz de usuario predeterminada de la empresa personalizando los diseños de página para los perfiles de usuario de la empresa. Para realizar este trabajo, debe ser administrador con el conjunto de permisos SUPER. Además, los perfiles deben configurarse y asignarles los usuarios apropiados. Para obtener más información, vea [Administrar usuarios, perfiles y áreas de tareas](admin-users-profiles-roles.md).  
  
Para configurar la interfaz de usuario para varios usuarios, personalice las páginas de un determinado perfil al que están asignados los usuarios. Puede hacerlo mediante [!INCLUDE[nav_windows](includes/nav_windows_md.md)], y personalizar de la misma forma que los usuarios individuales personalizan sus propias áreas de trabajo, es decir, con la función **Personalizar**. La diferencia es que debe abrir [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en el modo de configuración. Entre las personalizaciones habituales están las acciones que se incluirán en la cinta de opciones, el modo en que los campos se colocan en las fichas desplegables o en cuadros informativos, y los elementos de menú que se incluirán en el panel de navegación. 

> [!TIP]  
>  Una manera rápida para implementar la configuración de la IU para un perfil es si ya tiene un perfil configurado en otra base de datos de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Puede exportar ese perfil e importarlo a la base de datos actual. Para obtener más información, vea [Exportación e importación de perfiles](admin-profiles.md#ExportImportProfile).  
  
## <a name="general-information"></a>Información general
Tenga en cuenta la información siguiente antes de empezar a configurar la interfaz de usuario:
-   Antes de empezar a configurar la interfaz de usuario, según su licencia o permisos, la aplicación se puede configurar para mostrar y ocultar elementos de la interfaz de usuario (como campos, fichas desplegables y cuadros informativos). Para obtener más información sobre cómo hacerlo, consulte [Eliminando elementos de la interfaz de usuario según los permisos](https://msdn.microsoft.com/en-us/dynamics-nav/removing-elements-from-the-user-interface-according-to-permissions).

    Para ver el efecto de la opción Eliminación de los elementos de la IU, puede iniciar sesión como un usuario de prueba el conjunto de permisos del perfil que va a configurar. El motivo es que, como administrador, tiene el conjunto de permisos SUPER y, por lo tanto, no puede ver y probarla interfaz de usuario resultante durante su propio inicio de sesión.    
-   Al realizar cambios en la configuración de la IU para una página que ha personalizado un usuario, se mantiene la personalización de la IU del usuario y no la sobrescribe la nueva configuración de página. Del mismo modo, cuando se cancela la configuración de la IU de una página que ha personalizado un usuario, no se cancela la personalización de la IU del usuario.
-   La única situación en la que la configuración de la IU sobrescribe la personalización de la IU se produce cuando la configuración quita un elemento de la IU. Por ejemplo, si el administrador elimina un campo que el usuario haya movido o cuyo nombre haya cambiado, el campo se sigue eliminando de la interfaz del usuario.
-   Puede registrar configuraciones de IU de la misma página en función de los distintos puntos de acceso a la página. Por ejemplo, la ventana **Pedidos venta** se puede personalizar para que se vea diferente al abrirse desde la ventana **Ficha cliente** que al abrirse desde al área de tareas **Procesador de pedidos de ventas**. El punto desde el que se tiene acceso a la página que se personalizará se registra en esta personalización de página específica. Por consiguiente, puede haber varios registros de personalización de página en la base de datos, como se puede ver en la ventana **Eliminar configuración perfil**.  
-   A diferencia de cuando los usuarios cambian el tamaño de las ventanas o el ancho de las columnas en su propio equipo, cualquier cambio de vista básico que realice durante la configuración de la IU de un perfil no se guarda en dicho perfil y no estará disponible para los usuarios asignados al perfil. Los cambios básicos de visualización son específicos de cada equipo.   

## <a name="configure-a-profile-with-the-includenavwindowsincludesnavwindowsmdmd-in-configuration-mode"></a>Configure un perfil con el [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en modo configuración
1.  Abra un símbolo del sistema y escriba el siguiente comando para cambiar a la carpeta de instalación de [!INCLUDE[nav_windows](includes/nav_windows_md.md)]. Por ejemplo:  
  
    ```  
    cd C:\Program Files\(x86)\Microsoft Dynamics NAV\110\RoleTailored Client  
    ```  
  
2.  Escriba el comando siguiente para iniciar el [!INCLUDE[nav_windows](includes/nav_windows_md.md)] en modo de configuración en un perfil determinado:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"profileid"  
    ```  
  
     Reemplace **profileid** con el nombre del perfil que desee configurar.  
  
     Por ejemplo, para configurar el perfil del Administrador de contabilidad, utilice este comando:  
  
    ```  
    Microsoft.Dynamics.Nav.Client.exe -configure -profile:"Accounting Manager"  
    ``` 

3. Ahora está listo para comenzar a configurar la interfaz de usuario de la misma manera que los usuarios individuales personalizan sus propias áreas de trabajo. Para obtener más información, vea [Personalización del área de trabajo en [!INCLUDE[nav_windows](includes/nav_windows_md.md)]](ui-personalization-windows-client.md). 

## <a name="cancel-ui-configuration"></a>Cancelar la configuración de la IU
Puede cancelar las personalizaciones de la IU realizadas como configuración de un perfil de tres maneras:  
  
-   Cancele todas las personalizaciones que haya hecho para un perfil con el botón **Borrar páginas configuradas** de la ventana **Ficha de perfil**.  
  
-   Cancele la personalización de la IU realizada para páginas específicas de un perfil eliminando filas en la ventana **Eliminar configuración perfil**.  
  
-   Cancele la personalización de la IU realizada para un área de una página específica de un perfil con el botón **Restablecer valores predeterminados** de la ventana **Personalizar**.  
  
### <a name="general-information"></a>Información general  
-   Los usuarios pueden realizar personalizaciones de IU con su propio inicio de sesión de usuario para personalizar su propia interfaz. Cuando se cancela la configuración de la IU de una página que ha personalizado un usuario, no se cancela la personalización de la IU del usuario. Del mismo modo, al crear la nueva configuración de la IU para una página que ha personalizado un usuario, se mantiene la personalización de la IU del usuario y no la sobrescribe la nueva configuración de página.  

    La única situación en la que la configuración de la IU sobrescribe la personalización de la IU se produce cuando la configuración quita un elemento de la IU. Por ejemplo, si el administrador elimina un campo que el usuario haya movido o cuyo nombre haya cambiado, el campo se sigue eliminando de la IU del usuario.  
  
-   En la ventana **Eliminar personalización usuario** y con el botón **Restablecer valores predeterminados** en la ventana **Personalizar**, los usuarios pueden cancelar la personalización particular de la IU que han realizado en las páginas bajo su propia conexión de usuario. En este caso, el diseño de dichas páginas se restablece a cualquier personalización de IU que el administrador haya configurado para el perfil. Si no se ha configurado el perfil, el diseño de las páginas del usuario se restablece a la configuración de perfil predeterminada. Para obtener más información sobre cómo los usuarios cancelan una personalización, vea [Cancelar personalización](ui-personalization-windows-client.md#CancelPersonalization).
  
### <a name="to-cancel-all-ui-customization-that-you-have-made-for-a-profile"></a>Para cancelar toda la personalización de IU que ha realizado en un perfil  
  
1.  En el cuadro **Buscar**, escriba **Perfiles** y, a continuación, elija el vínculo relacionado.  
  
2.  Seleccione el perfil para el que desea cancelar todas las personalizaciones de la IU y, a continuación, en la pestaña **Inicio**, en el grupo **Administrar**, elija **Editar**.  
  
3.  En la ventana **Ficha de perfil**, en la pestaña **Acciones**, en el grupo **Funciones**, seleccione **Borrar páginas configuradas**.  
  
> [!NOTE]  
>  Toda personalización de la IU para el perfil, tanto la instalada con la aplicación como la efectuada por el administrador, queda cancelada. En la base de datos no permanece ningún diseño de página específico del perfil.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-specific-page-for-a-profile"></a>Para cancelar la personalización de IU que ha realizado en una determinada página o perfil  
  
1.  En el cuadro **Buscar**, escriba **Eliminar configuración perfil** y, a continuación, elija el vínculo relacionado.  
  
2.  Seleccione el perfil o el conjunto de páginas para el que desea cancelar la personalización de la IU y, a continuación, en la pestaña **Inicio**, en el grupo **Administrar**, elija **Eliminar**.  
  
    > [!IMPORTANT]  
    >  Si ha configurado distintas personalizaciones de la IU de la misma página basándose en distintas rutas de navegación a la página, la personalización de cada página aparecerá en la lista de la ventana **Eliminar configuración perfil** con la misma información. No existe información para identificar qué fila está relacionada con cada ruta de exploración. Por lo tanto, debe eliminar las filas una a una y realizar una comprobación visual en la página, o puede eliminar todas las filas con personalizaciones de IU para el perfil o la página.
    >    
    >  Toda personalización de la IU para la página del perfil realizada en la instalación o desde la última vez que se utilizó la ventana de **Eliminar configuración perfil**, queda cancelada. El diseño de la página se restablece al diseño estándar del objeto de página.  
  
### <a name="to-cancel-ui-customization-that-you-have-made-for-a-specific-ui-area-for-a-specific-page-for-a-profile"></a>Para cancelar la personalización de IU que ha realizado para una determinada área de IU en una página específica de un perfil  
  
Puede deshacer los cambios realizados en áreas de IU individuales, como una cinta de opciones, mediante el botón **Restablecer valores predeterminados** en la ventana **Personalizar**. También puede deshacer todos los cambios en la IU realizados para un perfil mediante la ventana de **Eliminar configuración perfil**.  
  
Se cancela la personalización de la IU del perfil del área de IU concreta en la página específica. El diseño del área de IU de la página se restablece a la configuración predeterminada, tal como lo ha creado el administrador o tal como se ha instalado con la aplicación.  
  
## <a name="see-also"></a>Consulte también  
[Personalización de [!INCLUDE[navnow_md](includes/navnow_md.md)]](ui-customizing-overview.md)   
