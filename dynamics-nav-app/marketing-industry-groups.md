---
title: Configurar grupos de industria para empresas de contacto
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 466f8513b3abc8c10dc579bff5fde9ea11c21d27
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-industry-groups-for-contact-companies"></a>Configurar grupos de industria para empresas de contacto
Puede usar grupos de industria para indicar el tipo de industria al que pertenecen sus contactos, por ejemplo, el sector de fabricación o el sector automotriz.

El uso de grupos de industria en contactos es un proceso que consta de dos pasos. Primero, debe definir el código del grupo de industria. Solo debe realzar este paso una vez para cada grupo de industria. Una vez tenga código de grupo de industria, puede comenzar a asignar el código a empresas de contacto.

**Nota:** Si pretende sincronizar sus contactos con proveedores, clientes o bancos en otras partes de la aplicación, puede ser interesante configurar una relación de negocio para ellos.

## <a name="define-an-industry-group-code"></a>Definir un código de grupo de industria
El código de grupo de industria define el tipo o la categoría del grupo, como ADVERT para publicidad o PRESS para televisión y radio. Puede tener varios códigos de grupo de industria. Para definir los grupos de industria, pude usar la ventana **Grupos industria**.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Grupos de industria** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la acción **Nuevo** e introduzca un código y una descripción. El código admite un máximo de 11 caracteres y puede ser cualquier combinación de números y letras.

## <a name="assign-industry-groups-to-a-contact"></a>Para asignar grupos de industria a un contacto
No puede asignar grupos de industria a una persona de contacto, solo a empresas.

1. Abra el contacto.
2. Elija la acción **Empresa** y, a continuación, elija la acción **Grupos de industria**. Se abrirá la ventana **Grupos industria contacto**.
3. En el campo **Código de grupos de industria**, seleccione el grupo de industria que desea asignar.

Repita estos pasos para asignar todos los grupos de industria que desee. También puede asignar grupos de industria desde la lista de contactos con el mismo procedimiento.

Aparece automáticamente el número de grupos de industrias asignados al contacto del campo **N.º grupos industrias** en la sección **Segmentación** de la ventana **Contacto**.

Después de asignar grupos de industria a sus contactos, puede utilizar esa información para seleccionar contactos para sus segmentos. Para obtener más información, vea [Procedimiento: Agregar contactos a segmentos](marketing-add-contact-segment.md).

##<a name="see-also"></a>Consulte también
[Crear empresas de contacto](marketing-create-contact-companies.md)

