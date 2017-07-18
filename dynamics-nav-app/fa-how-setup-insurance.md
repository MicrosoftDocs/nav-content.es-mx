---
title: 'Procedimiento: Configurar el seguro de los activos fijos'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 44bb5f20702a01d9fbbc025889ec2bc3191813be
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-insurance"></a>Procedimiento: Configurar el seguro de los activos fijos
Para gestionar la cobertura del seguro de los activos fijos, debe configurar la información general de los seguros y una ficha de seguro por cada póliza.

## <a name="to-set-up-general-insurance-information"></a>Para configurar la información general de seguros  
Para poder utilizar las características de seguro en Dynamics NAV, debe configurar antes alguna información general de seguro.  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración A/F** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.  

## <a name="to-set-up-insurance-types"></a>Para configurar tipos de seguros  
Puede agrupar las pólizas de seguros en categorías, como seguro contra robo o contra incendios. Los tipos de seguros se utilizan en la ficha de seguro.
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Tipos seguros** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario.

## <a name="to-set-up-insurance-cards"></a>Para configurar fichas de seguros  
Puede acumular información acerca de cada póliza de seguros en la ficha de seguro.  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Seguro** y, a continuación, seleccione el vínculo relacionado.  
2. En la ventana **Seguro**, seleccione la acción **Nuevo** para crear una ficha de seguro nueva.  
3. Rellene los campos según sea necesario.

## <a name="to-set-up-insurance-journal-templates"></a>Para configurar libros diarios de seguros  
Dynamics NAV crea automáticamente una plantilla de diario de seguros la primera vez que abre la ventana **Diario seguros**, pero puede configurar plantillas de diario adicionales. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md).  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Plantillas diario de seguros** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario.

## <a name="to-set-up-insurance-journal-batches"></a>Para configurar secciones del diario de seguros  
En un libro diario de seguros puede configurar secciones. Los valores de la sección del diario se utilizan como valores predeterminados si no se rellenan los campos de las líneas de diario. Para obtener más información, consulte [Trabajar con diarios generales](ui-work-general-journals.md)  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Plantillas diario de seguros** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione una plantilla de diario de seguros y, a continuación, selecciona la acción **Secciones**.
3. En la ventana **Secciones diario seguros**, rellene los campos según sea necesario.

**NOTA**: Los números tienen una función especial en los nombres de diario. Si un nombre de libro diario o un nombre de sección del diario contiene un número, el número aumenta automáticamente en uno cada vez que se registra el diario. Por ejemplo, si se escribe HH1 en el campo **Nombre**, el nombre del diario cambiará a HH2 después de registrar el diario llamado HH1.

## <a name="see-also"></a>Consulte también
[Configuración de activos fijos](fa-setup.md)  
[Gestión de activos fijos](fa-manage.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)

