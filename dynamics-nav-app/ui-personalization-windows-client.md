---
title: "Personalización de páginas para el cliente de Windows de Microsoft Dynamics"
description: Aprenda a personalizar la interfaz de usuario para que se adapte a su forma de trabajar.
author: jswymer
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/26/2017
ms.author: jswymer
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 12aee74950066647f61639ec88c47e9be3c2f172
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="personalizing-your-workspace-in-the-dynamics-windows-client"></a>Personalización del área de trabajo para el cliente de Windows de Microsoft Dynamics
Puede personalizar el área de trabajo para que se adapte a su trabajo y preferencias cambiando las páginas de modo que muestren únicamente la información que necesite y donde la necesite. Los cambios de personalización que realice solo afectarán a su visualización y no a la de otros usuarios. Puede personalizar muchas partes de la interfaz de usuario, incluidas las acciones que se incluirán en la cinta de opciones, el modo en que los campos se colocan en las fichas desplegables o en cuadros informativos, y los elementos de menú que se incluirán en el panel de navegación.

> [!NOTE]  
> También puede personalizar páginas mediante [!INCLUDE[nav_web_md](includes/nav_web_md.md)]. Para aprender como funciona la personalización entre los dos clientes, consulte [Visión general de la personalización](ui-personalization-overview.md).
 
## <a name="how-to-personalize-your-workspace"></a>Cómo personalizar el área de trabajo
La mayor parte de la personalización se realiza mediante la funcionalidad **Personalizar** a la que se puede acceder desde casi todas las páginas mediante los siguientes pasos:

1.  Abra la página que quiera personalizar.
2.  En la parte superior izquierda, elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, seleccione una de las opciones de personalización.

También hay algunos cambios básicos en la interfaz de usuario, como ajustar el tamaño de las ventanas o expandir el ancho de las columnas, acciones que puede realizar directamente en la página, fuera de la opción **Personalizar**.

## <a name="general-information"></a>Información general
Mientras esté personalizando la interfaz de usuario, es conveniente tener en cuenta lo siguiente: 

-   Puede registrar varias personalizaciones de la misma página en función de los distintos puntos de acceso a la página. Por ejemplo, la ventana Pedidos venta se puede personalizar para que se vea diferente al abrirse desde la ventana Ficha cliente que al abrirse desde el área de tareas Procesador de pedidos de ventas. El punto desde el que se tiene acceso a la página que se personalizará se registra en esta personalización de página específica. Por consiguiente, puede haber varios registros de personalización de página en la base de datos, como puede ver en la ventana **Eliminar personalización usuario**.

-   Según su licencia o permisos, la aplicación se puede configurar para mostrar y ocultar elementos de la interfaz de usuario (como campos, fichas desplegables y cuadros informativos). Solo podrá ver y personalizar los campos de los elementos para los que tenga permisos.

## <a name="customize-ribbons"></a>Personalizar cintas de opciones
La cinta de opciones le proporciona acceso a varias acciones. Al personalizar la cinta de opciones, puede optimizarla para los procesos y preferencias del proyecto. Por ejemplo, si utiliza con frecuencia la ventana **Dimensiones**, puede agregar la acción **Dimensiones** al grupo de acciones **Proceso**. También puede quitar las acciones que nunca usa para obtener un resumen mejor.  
  
Puede realizar las siguientes tareas para personalizar cintas de opciones en páginas:  
  
-   Agregar, cambiar de nombre o eliminar pestañas, grupos, acciones y menús.  
-   Reorganizar el orden de las acciones.  
-   Restablecer la configuración predeterminada de la cinta.  
  
### <a name="to-customize-a-ribbon"></a>Para personalizar una cinta de opciones
1. Abra la página que quiera modificar.
2. En la parte superior izquierda, elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Personalizar cinta de opciones**.

El cuadro de diálogo **Organizar acciones en la cinta de opciones** se divide en dos paneles. El panel **Acciones disponibles** muestra todas las acciones que puede agregar a la página. El panel **Mostrar acciones en este orden** muestra la estructura de todas las acciones que se muestran actualmente en la página.

-   Los productos de nivel de raíz definen las pestañas.

    -   Los productos de segundo nivel definen un grupo en una pestaña.

        -   Los de tercer nivel definen un menú de acciones en un grupo

### <a name="add-a-group"></a>Agregar un grupo
Seleccione la pestaña en la que desea crear el grupo y seleccione **Crear grupo**. No se puede agregar un grupo en un menú.

### <a name="add-a-menu"></a>Agregar un menú
Seleccione el grupo en la que desea crear el menú y seleccione **Crear menú**. Puede agregar únicamente un menú en cada grupo o menú. 

#### <a name="add-an-action"></a>Agregar una acción
Selecciónela del panel **Acciones disponibles**, elija **Agregar** para agregarla al panel **Mostrar acciones en este orden** y utilice los botones **Mover arriba** y **Mover abajo** para colocarla en la posición deseada.

No puede agregar una acción a una pestaña; únicamente a un grupo o a un menú.

###  <a name="limitations-and-recommendations"></a>Limitaciones y recomendaciones 
Tenga en cuenta de las limitaciones siguientes al personaliza la cinta:  
  
-   Las pestañas o los grupos del sistema, tal como **Inicio** o **Nuevo**, no se pueden mover ni se puede cambiar su nombre. La posición de algunos grupos, como **Nuevo documento**, es fija.  
-   Las acciones o los grupos que tienen información dinámica no se pueden agregar o quitar. 
-   Solo puede crear menús dentro de los grupos, no dentro de las pestañas.  
-   Puede anidar un menú en otro, pero no se recomienda.  
-   Si experimenta un comportamiento inesperado con los grupos y las acciones después de haber personalizado la cinta, haga lo siguiente:  
    
    1.  Vacíe, pero no elimine, el grupo en el que se produce el problema.  
    2.  Cierre el cuadro de diálogo mediante el botón **Aceptar**.  
    3.  Abra el diálogo de nuevo y vuelva a agregar las acciones al grupo.  

> [!IMPORTANT]  
>  Cualquier personalización que modifique la cinta de opciones podría afectar a la ayuda que proporciona [!INCLUDE[navnow_md](includes/navnow_md.md)], ya que los pasos de navegación en la ayuda pueden hacer referencia a otra organización de las cintas de opciones.

## <a name="customize-fasttabs"></a>Personalizar fichas desplegables
Las fichas desplegables ayudan a organizar la información sobre las páginas en grupos simples y manejables. Puede personalizar fichas desplegables en páginas de modo que faciliten su flujo de trabajo. Por ejemplo, puede que desee mostrar menos fichas desplegables u ocultar campos concretos en fichas desplegables. También puede promover que los campos más importantes se incluyan en los encabezados de ficha desplegable al contraer las fichas desplegables.  

### <a name="to-customize-a-fasttab"></a>Para personalizar una ficha desplegable  
  
1.  Abra la página que quiera modificar.
2.  Elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Personalizar esta página**.  
3.  En el cuadro de diálogo **Personalizar <Page Name>**, seleccione **Fichas desplegables**.  
  
### <a name="add-move-or-remove-fasttabs"></a>Agregar, mover o eliminar fichas desplegables
El cuadro **Mostrar fichas desplegables en este orden** contiene fichas desplegables que se encuentran actualmente en la página y el orden en el que se muestran. Utilice **Agregar**, **Eliminar** y los botones **Mover arriba** y **Mover abajo** para realizar cambios.

### <a name="show-and-hide-fields-on-fasttabs"></a>Mostrar y ocultar campos de las fichas desplegables
En el cuadro **Mostrar fichas desplegables en este orden**, seleccione la ficha desplegable que desee cambiar y haga clic en **Personalizar ficha desplegable**. Utilice los botones para personalizar los campos que desee mostrar y el orden que deben seguir.

Establezca la **Importancia** de la siguiente forma:
-   Si desea ver el campo de la cabecera de la ficha desplegable cuando esta se contraiga, establezca la acción **Aumentado**.
- Si desea que el campo se oculte a menos que el usuario elija la acción **Mostrar más campos** en la ficha desplegable, establezca la acción **Adicional**.
-   **Estándar** es la configuración predeterminada o normal.

### <a name="set-up-field-for-quick-entry"></a>Configure el campo para la entrada rápida 
Seleccione la casilla de verificación **Entrada rápida** para agregar el campo a la lista de campos de entrada rápida. Cuando trabaja en la página y pulsa la tecla Introducir clave en un campo, el puntero salta al siguiente campo que se configura para que sea un campo de entrada rápida. 

## <a name="customize-factboxes"></a>Personalizar cuadros informativos
Utilice los cuadros informativos para ver información relativa al registro que se ha seleccionado en la lista o se ha abierto en una página de tareas. Puede seleccionar qué cuadros informativos mostrar en su panel. También puede personalizar los cuadros informativos para mostrar sólo los campos que necesite.  
  
### <a name="to-show-or-hide-the-factbox-pane"></a>Para mostrar u ocultar el panel de cuadro informativo
Los cuadros informativos están situados en los paneles de cuadro informativo, que puede mostrar u ocultar según la página. Esto le permite ocultar fácilmente varios cuadros informativos sin tener que eliminarlos uno a uno. 

1.  Abra la página que quiera modificar. 
2.  Elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Cuadros informativos**. Una marca de verificación indica que se muestra el panel de cuadro informativo.  

### <a name="to-customize-the-factbox-pane"></a>Para personalizar el panel de cuadro informativo  
1.  Abra la página que quiera modificar. 
2.  Elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Elegir cuadros informativos**.  
    
### <a name="add-a-factbox"></a>Agregue un cuadro informativo  
  
Seleccione el cuadro informativo que desea agregar al panel en el cuadro **Cuadros informativos disponibles** y elija el botón **Agregar**.  
  
### <a name="remove-a-factbox"></a>Elimine un cuadro informativo  
  
En el cuadro **Mostrar cuadros informativos en este orden**, seleccione los cuadros informativos y elija el botón **Eliminar**.   
  
### <a name="change-the-order-of-the-factboxes"></a>Cambie el orden de los cuadros informativos  
  
En el cuadro **Mostrar cuadros informativos en este orden** seleccione el cuadro informativo que desee mover y elija **Mover arriba** o **Mover abajo** hasta que el cuadro informativo se coloque en el lugar deseado.  
  
### <a name="change-the-fields-in-a-factbox"></a>Modifique los campos de un cuadro informativo  
  
1.  En el cuadro **Mostrar cuadros informativos en este orden**, seleccione el cuadro informativo y elija el botón **Personalizar elemento**.  
  
2.   El cuadro **Campos disponibles** muestra todos los campos que puede elegir. El cuadro **Campos mostrados** muestra todos los campos que se muestran actualmente en el cuadro informativo. Utilice los botones para agregar, eliminar y mover los campos.   


## <a name="customize-columns-in-a-list-or-on-document-lines"></a>Personalice columnas de una lista o líneas de documento
Para obtener un mejor resumen de la información que necesita, puede personalizar las páginas de lista y de ficha. Para ello, agregue o elimine columnas de las cuadrículas, reorganice columnas y agregue una inmovilización de panel.  
  
### <a name="to-add-remove-and-arrange-columns"></a>Para agregar, eliminar y organizar columnas  
  
1.  Puede agregar, eliminar o reorganizar columnas de dos formas:

    -   Elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Elegir columnas**.
    -   Haga clic con el botón secundario del mouse en un encabezado de columna y, a continuación, seleccione **Elegir columnas**.

2.  En el cuadro de diálogo **Seleccionar las columnas que desea mostrar en la lista** el panel**Columnas disponibles** contiene las columnas ocultas. El panel **Mostrar columnas en este orden** contiene las columnas mostradas. Use los botones **Agregar** y **Eliminar** para mover columnas de un campo a otro. Use los botones **Mover arriba** y **Mover abajo** para cambiar la posición de las columnas. 

>[!TIP]
>Seleccione la casilla de verificación **Entrada rápida** para agregar el campo a la lista de campos de entrada rápida. Cuando trabaja en la página y pulsa la tecla Introducir clave en un campo, el puntero salta al siguiente campo que se configura para que sea un campo de entrada rápida. 

### <a name="to-set-the-freeze-pane"></a>Para establecer inmovilización de panel
Una lista puede tener muchas columnas, que pueden forzarle a desplazarse horizontalmente para verlas todas. Es posible que haya algunas columnas que siempre quiera mostrar incluso mientras se desplaza. Para hacerlo, puede agregar una inmovilización de panel vertical para restringir el desplazamiento de algunas columnas. Esto le permite asegurarse de que solo se muevan columnas menos importantes cuando se desplace.

Para configurar la inmovilización del panel, seleccione la columna después de la que desea que se inicie y elija **Agregar inmovilización de panel**.

## <a name="customizing-the-navigation-pane"></a>Personalizar el panel de navegación
El panel de navegación muestra un menú de vínculos a diferentes páginas de lista. Los vínculos se agrupan en los botones del nivel de raíz. 

### <a name="to-customize-the-navigation-pane"></a>Para personalizar el panel de navegación  
  
Elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Personalizar panel de navegación**.  
  
### <a name="rename-or-rearrange-buttons-in-the-navigation-pane"></a>Cambie el nombre o reorganice los botones en el panel de navegación  
En el cuadro de diálogo **Personalizar panel de exploración**, en el panel izquierdo, seleccione el botón que desea mover, cambiar de nombre o eliminar y, a continuación, seleccione la opción que le corresponda en el centro de la ventana.

No puede mover, eliminar ni cambiar el nombre del botón **Inicio**. El botón **Departamentos** puede ser eliminado del panel de exploración, pero no es posible cambiar su nombre ni moverlo. 
  
### <a name="add-a-new-menu-button"></a>Agregue un nuevo botón de menú 
Puede crear un nuevo botón del nivel de raíz y agregar un menú de vínculos a varias páginas abiertas en ese botón.

1. En el cuadro de diálogo **Personalizar panel de exploración**, seleccione **Nuevo** e introduzca un nombre en el campo **Nombre**.
2.  Elija el botón **Aceptar**.

Puede agregar vínculos al botón.  
  
### <a name="add-a-link-to-a-button"></a>Agregar un vínculo a un botón   
Si tiene permiso para ver una lista, como la lista de pedido de venta, puede agregarle un vínculo desde un botón en el panel de exploración.  
  
1.  En el cuadro de diálogo **Personalizar panel de exploración**, en el campo **Botones del panel de exploración**, seleccione el menú al que desee agregar el vínculo.  
  
2.  Elija el botón **Agregar**.  
  
3.  Busque el vínculo que desea agregar y seleccione **Aceptar**.  
> [!TIP]
> Si encuentra un vínculo en las páginas **Departamentos**, también puede agregarlo al panel de exploración. Para obtener más información, consulte la sección Agregar un vínculo de Departamentos al Área de tareas.  
  
### <a name="move-or-copy-a-link-from-one-button-to-another"></a>Mover o copiar un vínculo de un botón a otro  
  
1.  En el cuadro de diálogo **Personalizar panel de exploración**, en el campo **Botones del panel de exploración**, seleccione el menú donde actualmente aparece el vínculo.  
  
2.  En el panel **Listas**, seleccione el vínculo que desea mover y haga clic en **Mover a** o **Copiar a**  
  
3.  Seleccione el botón de navegación al que desea agregar el vínculo y, a continuación, haga clic en **Aceptar**.  
  
### <a name="rearrange-the-order-of-a-links-under-a-button"></a>Reorganice el orden de los vínculos en un botón  
  
1.  En el panel **Listas**, seleccione el vínculo que desea mover.  
  
2.  Utilice los botones **Mover arriba** y **Mover abajo** para colocar el vínculo.

## <a name="adding-department-links-to-the-role-center"></a>Agregar un vínculo de Departamentos al Área de tareas
En ocasiones, puede encontrar un vínculo en una página **Departamentos** que desea agregar al Área de tareas para acceder fácilmente. El lugar donde puede colocar el vínculo en el área de tareas depende de la categoría del vínculo en la página **Departamentos**.

En la tabla siguiente se describen los tipos de vínculos de cada categoría de las páginas **Departamentos** y en qué lugar del Área de tareas pueden agregarse.  
  
|**Categoría**|**Contiene**|**Agregar vínculo a**|  
|------------------|------------------|---------------------|  
|Listas|Páginas de lista|Botón **Inicio** en el panel de navegación|  
|Tareas|Páginas de tareas, procesos, hojas de trabajo, diarios|Pestaña **Acciones** en la cinta de opciones|  
|Informes y análisis|Informes, procesos, ventanas matriz|Pestaña **Informes** en la cinta de opciones|  
|Documentos|Documentos como facturas y recordatorios|**Informes** en la cinta de opciones|  
|Archivo/Historial|Documentos históricos finalizados, registros|Botón **Inicio** en el panel de navegación|  
|Administración|Ventanas de configuración|Pestaña **Acciones** en la cinta de opciones|  
  
### <a name="to-copy-department-links-to-your-role-center"></a>Para copiar vínculos de departamento al Área de tareas  
  
1.  Abra la página **Departamentos**.  
  
2.  Haga clic con el botón secundario en el vínculo y elija una de las siguientes opciones (solo estará disponible una).  
  
    |**Seleccione**|**Para agregar el vínculo a**|  
    |----------------|----------------------------|  
    |**Agregar al panel de exploración**|El botón **Inicio** del panel de navegación en el área de tareas.|  
    |**Agregar a acciones en la cinta de opciones Área de tareas**|El menú **Acciones** en la cinta de su Área de tareas|  
    |**Agregar a informes en la cinta de opciones Área de tareas**|El menú **Informes** en la cinta de su Área de tareas|  
  
3.  Confirme el mensaje que aparece.  
  
 El nuevo vínculo aparece ahora en el menú al cual lo agregó. Sin embargo, es posible que desee moverlo a otro lugar del menú. Si, por ejemplo, agregó un vínculo al panel de exploración, éste aparecerá en el menú **Inicio**, pero no podrá moverlo a otro menú del panel. Para obtener más información, vea la sección Personalización del panel de navegación. 

## <a name="adding-charts-to-role-centers-and-list-pages"></a>Agregar gráficos en áreas de tareas y páginas de lista
Cuando tiene información compleja, es posible que desee ver una representación visual de los datos que le ayude a ver tendencias y a tomar decisiones. Por ejemplo, puede que desee supervisar los saldos por cuenta bancaria de su empresa en un gráfico. Use el panel gráfico para mostrar visualmente datos en una lista en los siguientes tipos de páginas:  
  
-   En su área de tareas, donde puede seleccionar gráficos genéricos predefinidos.  
  
-   En una página de lista, donde puede elegir ver una lista como un gráfico.  
  
### <a name="to-add-a-generic-chart-to-your-role-center"></a>Para agregar un gráfico genérico al área de tareas  
  
1.  En su área de tareas, elija el menú **Liquidación** ![icono del botón de menú Liquidación en la barra de menús](media/applicationmenuicon.png "ApplicationMenuIcon"), seleccione **Personalizar** y, a continuación, **Personalizar esta página**.  
  
2.  En el campo **Partes disponibles** de la ventana **Personalizar Área de tareas**, seleccione **Elemento gráfico** y haga clic en **Agregar**.  
  
3.  Utilice los botones **Mover arriba**, **Mover abajo**, **Mover izquierda** y **Mover derecha** para colocar el elemento gráfico en su Área de tareas.  
  
4.  Seleccione el elemento gráfico y elija **Personalizar elemento**.  
  
5.  En la ventana **Personalizar elemento**, seleccione el gráfico predefinido que desee mostrar y, a continuación, haga clic en **Aceptar**.  
  
### <a name="to-view-a-list-as-a-chart"></a>Para ver una lista como un gráfico  
  
1.  En la página de lista, seleccione la acción **Mostrar como gráfico**.  
  
2.  Seleccione una medida y una dimensión para crear un gráfico personalizado. Para ver información adicional, seleccione una dimensión secundaria. Por ejemplo, para crear un simple gráfico de barras, seleccione una dimensión en el eje X y, a continuación, la dimensión **Cuenta de dimensiones** en el eje Y.  
  
> [!NOTE]  
>  Por defecto, el panel de gráficos está oculto, ya que puede reducir el rendimiento. Debe mostrar únicamente el gráfico cuando deba disponer de la información.  
    
## <a name="handling-external-files-and-automation-objects"></a>Gestión de archivos externos y objetos de automatización
Cuando [!INCLUDE[navnow_md](includes/navnow_md.md)] recibe un archivo externo, se presentará un cuadro de diálogo. Además de seleccionar qué hacer con el archivo, puede decidir cómo tratar el tipo de archivo la siguiente vez que se reciba.  
  
Cuando se requiere que [!INCLUDE[navnow_md](includes/navnow_md.md)] ejecute un objeto de automatización, se presentará un cuadro de diálogo. Puede decidir si el tipo de objeto siempre se debe ejecutar o si nunca se puede ejecutar.  
  
### <a name="to-specify-how-to-handle-external-files"></a>Para especificar cómo se controlan los archivos externos  
  
1.  Cuando se presente el cuadro de diálogo, desactive la casilla **Preguntar siempre antes de abrir este tipo de archivo** si desea que [!INCLUDE[navnow_md](includes/navnow_md.md)] recuerde la opción seleccionada en el paso 2. La próxima vez que se deba administrar el tipo de archivo, no aparecerá el cuadro de diálogo y el archivo se tratará según lo especificado en el paso 2.  
  
     También puede seleccionar la casilla **Preguntar siempre antes de abrir este tipo de archivo** para que se abra siempre el cuadro de diálogo cuando se reciba este tipo de archivo.  
  
2.  Seleccione **Abrir**, **Guardar** o **Cancelar**. El archivo se trata en función de su selección.  
  
### <a name="to-specify-how-to-handle-automation-objects"></a>Para especificar cómo se controlan los objetos de automatización  
  
Cuando se presente con el diálogo, seleccione la casilla **Permitir siempre** si desea que [!INCLUDE[navnow_md](includes/navnow_md.md)] ejecute siempre dicho tipo de objeto de automatización. La próxima vez que se requiera la ejecución del objeto de automatización, no aparecerá el cuadro de diálogo y dicho objeto se ejecutará directamente.  
  
También puede seleccionar la casilla de **No permitir nunca**. La próxima vez que se requiera la ejecución del objeto de automatización, no aparecerá el cuadro de diálogo y no se ejecutará dicho objeto.  

## <a name="CancelPersonalization"></a>Cancelación de la personalización
La cancelación de la personalización se puede dividir en dos categorías:

-   Cancelar los cambios que ha realizado mediante la función **Personalizar** .
-   Cancelación de cambios básicos de la interfaz de usuario. 

### <a name="cancel-customization"></a>Cancelar la personalización
Si desea cancelar todas las personalizaciones de la IU realizadas para una página bajo sus datos de inicio de sesión o desde la última vez que canceló personalizaciones de la IU, hágalo a través de la ventana **Eliminar personalización usuario**. El diseño de la página para la que se elimina la personalización se restablece a la configuración predeterminada para su perfil.  
  
Si solo desea cancelar personalizaciones de la IU realizadas en un área específica de la interfaz de usuario en una página, como la cinta de opciones, puede utilizar el botón **Restablecer valores predeterminados** de la ventana **Personalizar**. El diseño del área de IU específica en dicha página se restablece a la configuración predeterminada para su perfil.  
  
#### <a name="to-cancel-all-ui-customization-that-you-have-made-to-a-page"></a>Para cancelar toda la personalización de IU que ha realizado en una página  
  
1.  En el cuadro **Buscar**, introduzca **Eliminar personalización usuario** y, a continuación, elija el vínculo relacionado.  
  
2.  Seleccione la página para la que desea cancelar la personalización de la IU y, a continuación, en la pestaña **Inicio**, en el grupo **Ver**, elija **Eliminar**.  
  
> [!NOTE]  
>  Toda personalización de la IU de la página realizada hasta ahora bajo los datos de inicio de sesión actuales o desde que se utilizó por última vez la ventana **Eliminar personalización usuario**, queda cancelada. El diseño de la página se restablece a la configuración predeterminada para su perfil, tal como lo ha configurado el administrador o tal como se ha instalado con Microsoft Dynamics NAV.  
  
#### <a name="to-cancel-ui-customization-that-you-have-made-to-a-ui-area-on-a-page"></a>Para cancelar la personalización de IU que ha realizado en un área de IU en una página  
  
1.  Desde la página donde se ha personalizado un área de la IU, como la cinta de opciones, elija el icono del menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Personalizar <UI area>**.  
  
2.  En la parte inferior de la ventana **Personalizar**, seleccione el botón de **Restablecer valores predeterminados**.  
  
> [!NOTE]  
>  Toda personalización del área de IU realizada hasta ahora para la página bajo los datos de inicio de sesión actuales o desde que se utilizó por última vez el botón **Restablecer valores predeterminados**, queda cancelada. El diseño del área de la IU en la página se restablece a la configuración predeterminada para su perfil, tal como lo ha configurado el administrador o tal como se ha instalado con Microsoft Dynamics NAV.

### <a name="cancel-basic-ui-changes"></a>Cancelar cambios básicos de la interfaz de usuario
Puede cancelar los cambios básicos de la interfaz de usuarios si abre la ventana **Restablecer la configuración especificada por el usuario** de su área de tareas.  
  
Los cambios de IU básicos incluyen opciones como:
 -  Cambiar el tamaño y la posición de las ventanas.
 -  Cambiar el ancho de las columnas
 -  Cambiar la altura de los encabezados de columna.
 -  Organizar en columnas una lista.
 -  Mostrar listas como gráficos.
 -  Especificar cómo gestionar archivos externos y objetos de automatización  
 
#### <a name="to-cancel-basic-ui-changes"></a>Para cancelar cambios básicos de la interfaz de usuario
  
1.  Vaya a su área de tareas.  
  
     En el menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Restablecer la configuración especificada por el usuario**.  
  
2.  Elija el botón **Restablecer la configuración de la IU**. También puede seleccionar el botón **Restablecer todo** para cancelar las decisiones para gestionar los archivos y los objetos de automatización.  
  
 Todos los cambios básicos de la IU realizados bajo los datos de inicio de sesión actuales en [!INCLUDE[navnow_md](includes/navnow_md.md)], o desde la última vez que se seleccionó el botón de **Restablecer la configuración de la IU**, quedan cancelados. La interfaz de usuario se restablece a la configuración predeterminada para su perfil.  
  
#### <a name="to-cancel-your-decision-for-running-or-saving-external-files"></a>Para cancelar la decisión de ejecutar o guardar archivos externos  
  
1.  Vaya a su área de tareas.  
  
     En el menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Restablecer la configuración especificada por el usuario**.  
  
2.  Elija el botón **Restablecer la decisión de control**. También puede seleccionar el botón **Restablecer todo** para cancelar las decisiones y los cambios de vista para gestionar los objetos de automatización.  
  
 Todas las decisiones de la gestión predeterminada de los tipos de archivo realizadas bajo los datos de inicio de sesión del usuario actual o desde que se seleccionó por última vez el botón **Acceso a archivo cliente**, quedan canceladas y restablecidas en la configuración predeterminada para su perfil. La próxima vez que [!INCLUDE[navnow_md](includes/navnow_md.md)] reciba un archivo externo de cualquier tipo, se le presentará un cuadro de diálogo con las opciones **Guardar**, **Ejecutar** y **Cancelar**  
  
### <a name="to-cancel-your-decision-for-handling-automation-objects"></a>Para cancelar la decisión de controlar los objetos de automatización  
  
1.  Vaya a su área de tareas.  
  
     En el menú **Liquidación** ![botón menú liquidación en la barra de menú](media/applicationmenuicon.png "IconoMenúLiquidación"), seleccione **Personalizar** y, a continuación, **Restablecer la configuración especificada por el usuario**.  
  
2.  Elija el botón **Restablecer las decisiones de automatización**. También puede seleccionar el botón **Restablecer todo** para cancelar las decisiones y los cambios de vista para ejecutar o guardar archivos externos.  
  
 Todas las decisiones sobre cómo ejecutar los objetos de automatización realizadas bajo los datos de inicio de sesión actuales o desde la última vez que se seleccionó el botón **Restablecer las decisiones de automatización**, quedan canceladas. El comportamiento de control de archivos se ha restablecido a la configuración predeterminada para su perfil. La próxima vez que [!INCLUDE[navnow_md](includes/navnow_md.md)] deba ejecutar un objeto de automatización de cualquier tipo, se le presentará un cuadro de diálogo con las opciones **Permitir siempre** y **No permitir nunca**.    

<!--Use the following table to get more information about customizing the different elements of the UI.

| To | See |
| --- | --- |
| Change which actions to show on the ribbon and how the actions are grouped. |[How to: Customize FastTabs](purchasing-how-record-purchases.md) |
|Change which FastTabs to show and which fields to include on the FastTabs.|[How to: Request Quotes](purchasing-how-request-quotes.md)|
|Add, remove, or arrange columns in a list or document-lines that represent fields in the underlying tables. |[ How to: Add or Remove Columns in a List or on Document Lines](purchasing-how-purchase-products-sale.md) |
| Rename or rearrange buttons, create a new menu button, add a link to a menu, or rearrange the order of a menu. |[ How to: Customize the Navigation Pane](purchasing-how-correct-cancel-unpaid-purchase-invoices.md) |
| Add a link from a department page to your Role Center. |[How to: Process Purchase Returns or Cancellations](purchasing-how-register-new-vendors.md) |
|Add a chart to your Role Center or to a list page.|[How to: Combine Receipts on a Single Invoice](purchasing-how-to-combine-receipts.md)|
| Unod personalization that you have made to your user interface, either for a specific area on a page, such as a ribbon, or for the whole page.|[How to: Cancel Personalization](ui-customization-cancel.md)|
-->


## <a name="see-also"></a>Consulte también
[Personalización del área de trabajo para el cliente web de Dynamics](ui-personalization-user.md)  
[Visión general de la personalización](ui-personalization-overview.md)  



