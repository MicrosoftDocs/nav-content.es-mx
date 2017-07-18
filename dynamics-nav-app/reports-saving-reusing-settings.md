---
title: "Configuración guardada en los informes"
author: jswymer
ms.custom: na
ms.date: 09/26/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 0f11d862315c8ecd160cd18afb0a72a2d684b9b2
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="saved-settings-on-reports"></a>Configuración guardada en los informes
Según el informe que se ejecute, es posible que se le presente una página que permite definir determinadas opciones y filtros para cambiar los datos que se incluyen en el informe generado. Esta página se conoce como la página de solicitud de informe. Un informe puede incluir una o varias *opciones de configuración guardadas* que puede aplicar al informe de la página de solicitud. La *configuración guardada* son básicamente opciones y filtros predeterminados. El uso de la configuración guardada es una forma rápida y confiable de generar de forma coherente informes que contienen los datos correctos.

Puede ver la configuración guardada que están a su disposición para un informe en la sección **Configuración guardada** de la página de solicitud de informe.

## <a name="to-apply-saved-settings-to-a-report"></a>Para aplicar la configuración guardada a un informe
1.  Abra el informe.

    Aparece la página de solicitud de informe.    
2.  En la sección **Configuración guardada** de la página, configure el campo **Nombre** como la configuración guardada que desea usar.

    La sección **Valores guardados** solo aparece si el informe se ha ejecutado antes o si hay configuraciones existentes guardadas. La configuración guardada que se denomina **Filtros y opciones usados por última vez** está siempre disponible. Esta configuración son los valores de opción y filtro que se utilizaron la última vez que ejecutó el informe.

## <a name="administer-saved-report-settings-for-users"></a>Administrar la configuración de informe guardada para los usuarios
Si tiene los permisos adecuados, puede ver, crear y modificar la configuración guardada de todos los informes para todos los usuarios de la empresa. Puede asignar la configuración guardada de un informe a usuarios individuales o a todos los usuarios de la empresa.

La configuración guardada se administra en la página 1506 **Configuración del informe**. Para abrir esta página, en la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración del informe** y, a continuación, seleccione el vínculo relacionado. 

En la página **Configuración del informe**, puede crear nuevos valores de cero o hacer una copia y modificar la configuración existente. Para modificar las opciones y los filtros de una configuración, elija la acción **Editar**.

**Notas**:
-    La característica de configuración guardada en informes es relevante únicamente cuando la propiedad SaveValues de la página de solicitud se define en Sí. La propiedad SaveValues se define en el entorno de desarrollo.
-    Si crea un elemento de configuración guardada para todos los usuarios y tiene el mismo nombre que la configuración guardada existente de un usuario determinado, ese usuario no podrá utilizar la configuración guardada que se asigne a todos.  En el campo Configuración guardada de la página de solicitud de informe, el usuario verá dos opciones de configuración guardada con el mismo nombre. Sin embargo, independientemente de la opción que elija, se usará la configuración guardada específica del usuario.

## <a name="see-also"></a>Consulte también
[Programar un informe para que se ejecute](ui-schedule-report.md)

