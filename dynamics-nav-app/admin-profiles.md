---
title: "Administrar perfiles y áreas de tareas"
description: "Obtenga más información sobre cómo administrar usuarios y áreas de tareas en Dynamics NAV."
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: profiles, roles, role centers, user roles
ms.date: 09/01/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: a657c409c9cd361a505f1fd61dbb5254b25c5144
ms.contentlocale: es-mx
ms.lasthandoff: 10/26/2017

---
# <a name="managing-profiles-and-role-centers"></a>Administrar perfiles y áreas de tareas
Los perfiles son colecciones de usuarios de [!INCLUDE[navnow_md](includes/navnow_md.md)] que comparten la misma área de tareas. Un área de tareas es un tipo de página en la que puede situar distintos apartados. Cada apartado es un contenedor en el que puede albergar otras páginas o apartados del sistema predefinidos, como un apartado de Outlook o apartados para agregar tareas, notificaciones o notas.  

## <a name="about-profiles-and-role-centers"></a>Acerca de perfiles y áreas de tareas
Los perfiles se usan para vincular usuarios a áreas de tareas definidas previamente. Un área de tareas es la página de inicio de todos los usuarios de un perfil, que se ha configurado para reflejar las tareas y las prioridades de los usuarios de ese perfil. Por ejemplo, el área de tareas procesadora de pedidos se ha configurado para reflejar las tareas y las prioridades de un procesador de pedidos. Un área de tareas proporciona acceso fácil a la información que los usuarios necesitan para realizar su trabajo diario. Por ejemplo, el área de tareas determina las pilas, o mosaicos, que se muestran cuando los usuarios inician sesión por primera vez y los vínculos de la página de navegación.

El perfil que se usa aparece en el encabezado del área de contenido principal del Área de tareas. Un administrador puede personalizar esta área de tareas para cubrir las necesidades de un rol específico en una empresa concreta. El área de tareas procesadora de pedidos se podrá personalizar más en un único equipo para cubrir las necesidades de una persona que esté realizando el trabajo de procesador de pedidos. Esta persona puede personalizar el área de tareas al guardar consultas, agregar filtros y agregar o eliminar campos.

Los perfiles y las áreas de tareas se asocian a los roles y las responsabilidades de la organización. [!INCLUDE[navnow_md](includes/navnow_md.md)] proporciona un conjunto de perfiles predeterminados donde cada uno de ellos corresponde a un área de tareas y se vincula a ella. Los administradores pueden modificar los perfiles existentes o crear perfiles nuevos.  

> [!NOTE]  
>  Los perfiles no se vinculan explícitamente a los roles y a los permisos que constituyen el sistema de seguridad, pero los usuarios de perfiles deben tener permisos que se alineen con sus roles en el sistema de seguridad. Para obtener más información, consulte [Seguridad en el entorno adaptado a roles en MSDN Library](http://go.microsoft.com/fwlink?LinkId=147633).

## <a name="to-create-a-profile"></a>Para crear un perfil
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Perfiles** y, a continuación, seleccione el vínculo relacionado.  

2.  Seleccione la acción **Nuevo** para abrir la ventana **Nueva ficha de perfil**.  

3.  En el campo **Id. perfil**, escriba un nombre que describa el rol previsto del usuario.  

4.  En el campo **Descripción**, escriba una descripción del identificador de perfil, como por ejemplo, **Procesador de pedidos**.  

5.  Establezca el campo **Id. área de tareas** en el área de tareas que desea asignar al perfil.  

6.  Active la casilla **Área de tareas predeterminada** para convertir esta área de tareas en la predeterminada del perfil.  

7.  Elija el botón **Aceptar**. .  

El procedimiento para modificar un perfil existente es el mismo, excepto que se selecciona un perfil existente en la página de perfiles en lugar de elegir la acción **Nuevo**.  


##<a name="copying-a-profile"></a>Copiar un perfil
Copiar un perfil puede ahorrarle tiempo si desea utilizar una configuración similar en un perfil y solo desea modificar algunos ajustes.

1.  Abra el perfil que desea copiar y elija la acción **Copiar perfil**.

2.  En el campo **Nuevo id. de perfil**, introduzca el nombre del perfil que desea copiar.

3.  Establezca el campo **Nuevo ámbito de perfil** en una de las siguientes opciones:

    - **Sistema** para hacer que el nuevo perfil esté disponible para todas las bases de datos de inquilinos que usan la aplicación.
    - **Suscriptor** para hacer que el nuevo perfil esté disponible para la base de datos actual del suscriptor.
4. Cuando haya finalizado, elija el botón **Aceptar**.

## <a name="ExportImportProfile"></a>Exportación e importación de perfiles

Puede exportar e importar perfiles como archivos XML a o desde la base de datos de [!INCLUDE[d365fin](includes/d365fin_md.md)]. La exportación e importación de un perfil puede ahorrarle tiempo al configurar la interfaz de usuario porque reutiliza una configuración de perfil existente en lugar de tener que configurar un perfil desde cero. Si tiene un perfil configurado en una base de datos de [!INCLUDE[d365fin](includes/d365fin_md.md)] y desea reutilizar todas o algunas de las mismas configuraciones de perfil en otra base de datos, puede exportar el perfil a un archivo XML. A continuación, puede importar el archivo XML de perfil a otra base de datos.

-   Para exportar un perfil, abra la búsqueda y abra la página **Exportar perfiles**, seleccione el perfil de la lista y elija la acción **Exportar**. Guarde el archivo XML en una ubicación del equipo o red.

-   Para importar un perfil, abra la búsqueda y abra la página **Importar perfiles**, seleccione el perfil del archivo XML y elija el botón **Aceptar**.

    > [!NOTE]  
    >  No puede importar un perfil que ya exista en la base de datos, aunque nombre o el contenido del archivo XML sean distintos. Debe eliminar el perfil existente para poder importar el perfil nuevo.



## <a name="see-also"></a>Consulte también  
[Administrar usuarios y permisos](ui-how-users-permissions.md)  
[Personalización de la interfaz de usuario](ui-customizing-overview.md)   
<!--[Security Overview](../Security%20Overview.md)-->

