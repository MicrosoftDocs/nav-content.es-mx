---
title: Configurar relaciones de negocio en empresas de contacto
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 20abe2f08fc726a008719f94389579d02ecbd275
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a>Configurar relaciones de negocio en empresas de contacto
Puede usar relaciones de negocio se usan para indicar las relaciones de ese tipo con los contactos, por ejemplo, referencia, banco, consultora, proveedor de servicios, etc.

El uso relaciones de negocio en contactos es un proceso que consta de dos pasos. Primero, debe definir el código de relación de negocio. Solo debe realizar este paso una vez para cada relación de negocio. Una vez tenga un código de relación de negocio, puede comenzar a asignar el código a empresas de contacto.

**Nota**: Si pretende sincronizar sus contactos con proveedores, clientes o bancos en otras partes de la aplicación, puede ser interesante configurar una relación de negocio para ellos.

## <a name="define-a-business-relation-code"></a>Definir un código de relación de negocio
El código de relación de negocio define una categoría o un tipo de relación de negocio, como BANCO o ABO. Puede tener varios códigos de relación de negocio. Para definir relaciones de negocio, use la ventana **Relaciones de negocio**.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Relaciones de negocio** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la acción **Nuevo** e introduzca un código y una descripción. El código admite un máximo de 11 caracteres y puede ser cualquier combinación de números y letras.

## <a name="assign-business-relations-to-a-contact"></a>Asignar relaciones de negocio a un contacto
No puede asignar relaciones de contacto a una persona de contacto, solo a empresas.

1. Abra el contacto.
2. Seleccione la acción **Empresa** y, a continuación, seleccione la acción **Relaciones de negocio**.

    Se abre la ventana **Relaciones de negocio de contacto**.
3. En el campo **Cód. relación negocio**, seleccione la relación de negocio que desea asignar.

Repita estos pasos para asignar todos las relaciones de negocio que desee. También puede asignar relaciones de negocio desde la lista de contactos con el mismo procedimiento.

Aparece automáticamente el número de relaciones de negocio asignadas al contacto del campo **N.º de relaciones de negocio** en la sección **Segmentación** de la ventana **Contacto**.

Después de asignar relaciones de negocio a sus contactos, puede utilizar esa información para seleccionar contactos para sus segmentos. Para obtener más información, vea [Procedimiento: Agregar contactos a segmentos](marketing-add-contact-segment.md).

##<a name="see-also"></a>Consulte también
[Crear empresas de contacto](marketing-create-contact-companies.md)

