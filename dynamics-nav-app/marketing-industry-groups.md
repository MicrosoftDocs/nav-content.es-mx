---
title: Configurar grupos de industria para empresas de contacto
description: "Describe cómo definir un grupo de industria y asignarlo a una empresa de contacto, por ejemplo, en la industria minorista o la industria del automóvil."
documentationcenter: 
author: jswymer
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: relationship, prospect
ms.date: 06/06/2017
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 62d946155cb65a3e976771bc5029878893bd4797
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-industry-groups-for-contact-companies"></a>Configurar grupos de industria para empresas de contacto
Puede usar grupos de industria para indicar el tipo de industria al que pertenecen sus contactos, por ejemplo, el sector de fabricación o el sector automotriz.

El uso de grupos de industria en contactos es un proceso que consta de dos pasos. Primero, debe definir el código del grupo de industria. Solo debe realzar este paso una vez para cada grupo de industria. Una vez tenga código de grupo de industria, puede comenzar a asignar el código a empresas de contacto.

> [!NOTE]  
>   Si desea sincronizar sus contactos con proveedores, clientes o bancos en otras partes de la aplicación, se recomienda configurar una relación de negocio para ellos.

## <a name="to-define-an-industry-group-code"></a>Para definir un código de grupo de industria
El código de grupo de industria define el tipo o la categoría del grupo, como ADVERT para publicidad o PRESS para televisión y radio. Puede tener varios códigos de grupo de industria. Para definir los grupos de industria, pude usar la ventana **Grupos industria**.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Grupos industria** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo** e introduzca un código y una descripción. El código admite un máximo de 11 caracteres y puede ser cualquier combinación de números y letras.

## <a name="AssignIndustryGroupContact"></a> Para asignar grupos de industria a un contacto
No puede asignar grupos de industria a una persona de contacto, solo a empresas.

1. Abra el contacto.
2. Elija la acción **Empresa** y, a continuación, elija la acción **Grupos de industria**. Se abrirá la ventana **Grupos industria contacto**.
3. En el campo **Código de grupos de industria**, seleccione el grupo de industria que desea asignar.

Repita estos pasos para asignar todos los grupos de industria que desee. También puede asignar grupos de industria desde la lista de contactos con el mismo procedimiento.

Aparece automáticamente el número de grupos de industrias asignados al contacto del campo **N.º grupos industrias** en la sección **Segmentación** en la ventana **Contacto**.

Después de asignar grupos de industria a sus contactos, puede utilizar esa información para seleccionar contactos para sus segmentos. Para obtener más información, vea [Procedimiento: Agregar contactos a segmentos](marketing-add-contact-segment.md).

## <a name="see-also"></a>Consulte también
[Crear empresas de contacto](marketing-create-contact-companies.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

