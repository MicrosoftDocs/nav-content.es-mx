---
title: "Creación de un diseño de informe personalizado"
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
ms.openlocfilehash: 90136439e09deb00a9aed9344fc5f89812caef3a
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-a-custom-report-layout"></a>Creación de un diseño de informe personalizado
De forma predeterminada, un informe tendrá un diseño de informe integrado, bien de RDLC o de Word, o ambos. No puede modificar diseños integrados. No obstante, puede crear sus propios diseños personalizados que le permitan modificar el aspecto del informe cuando se vea, se imprima o se guarde. Puede crear varios diseños de informe personalizados para el mismo informe y, a continuación, cambiar al diseño utilizado por un informe según sea necesario.

Para crear un diseño personalizado, puede hacer una copia de un diseño personalizado existente o agregar un nuevo diseño personalizado, que en la mayoría de los casos se basa en un diseño integrado. Cuando se agrega un nuevo diseño personalizado, puede elegir agregar un tipo de diseño de informe de RDLC, uno de Word, o ambos. El nuevo diseño personalizado se basará automáticamente en el diseño integrado del informe si hay uno disponible. Si no hay ningún diseño integrado para el tipo, se crea un nuevo diseño en blanco que tendrá que modificar y diseñar desde cero. Para obtener más información acerca de los diseños de informe de RDLC y de Word, diseños personalizados e integrados y otros temas, consulte [Gestionar diseños de informe](ui-manage-report-layouts.md).  

## <a name="to-create-a-custom-layout"></a>Para crear un diseño personalizado
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Selección de diseño de informes** y, a continuación, seleccione el enlace relacionado.  
La ventana **Selección de diseño de informes** muestra todos los informes disponibles en la empresa especificada en el campo Empresa en la parte superior de la ventana.
2. Establezca el campo **Empresa** en la empresa en la que desea crear el diseño del informe.
3. Seleccione la fila para el informe para el cual desee crear el diseño y, a continuación, elija **Diseños personalizados**.  
La ventana **Diseños de informe personalizados** aparece con todos los diseños personalizados disponibles para el informe seleccionado.
4. Si desea crear una copia de un diseño personalizado existente, seleccione el diseño personalizado existente en la lista y, a continuación, elija **Copiar**.  
La copia del diseño personalizado aparece en la ventana **Diseños de informe personalizados** e incluye las palabras Copia de en el campo Descripción.
5. Si desea añadir un nuevo diseño personalizado que se base en un diseño integrado, haga lo siguiente:  
    1. Elija **Nuevo**. Aparece la ventana **Insertar diseñado integrado para un informe**. Los campos de **Id.** y **Nombre** se rellenan automáticamente.
    2. Para agregar un tipo de diseño de informe de Word personalizado, seleccione la casilla **Insertar diseño de Word**.
    3. Para agregar un tipo de diseño de informe de RDLC personalizado, seleccione la casilla **Insertar diseño de RDLC**.
    4. Elija el botón **Aceptar**.  
    Los nuevos diseños personalizados aparecen en la ventana **Diseños de informe personalizados**. Si un diseño nuevo se basa en un diseño integrado, tendrá las palabras **Copia de un diseño integrado** en el campo **Descripción**. Si no había diseño integrado para el informe, el nuevo diseño tendrá las palabras **Nuevo diseño** en el campo **Descripción** para indicar que el diseño personalizado está en blanco.
6. De forma predeterminada, el campo **Nombre de la empresa** está en blanco, lo que significa que el diseño personalizado estará disponible para el informe en todas las empresas. Para que el diseño personalizado esté disponible en una empresa específica solo, elija **Editar** y, a continuación, establezca el campo **Nombre de la empresa** en la empresa que quiera.

## <a name="see-also"></a>Consulte también
[Gestionar diseños de informe](ui-manage-report-layouts.md)  
[Cambiar el diseño que se usa actualmente en un informe](ui-how-change-layout-currently-used-report.md)
