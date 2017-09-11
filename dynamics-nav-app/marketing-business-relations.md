---
title: Configurar relaciones de negocio en empresas de contacto
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 6616473a00e85e52648713d7e067f4b3b72caecf
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---
# <a name="set-up-business-relations-on-contact-companies"></a><span data-ttu-id="e3591-102">Configurar relaciones de negocio en empresas de contacto</span><span class="sxs-lookup"><span data-stu-id="e3591-102">Set Up Business Relations on Contact Companies</span></span>
<span data-ttu-id="e3591-103">Puede usar relaciones de negocio se usan para indicar las relaciones de ese tipo con los contactos, por ejemplo, referencia, banco, consultora, proveedor de servicios, etc.</span><span class="sxs-lookup"><span data-stu-id="e3591-103">You can use business relations to indicate the business relationship you have with your contacts, for example, a prospect, bank, consultant, service supplier, and so on.</span></span>

<span data-ttu-id="e3591-104">El uso relaciones de negocio en contactos es un proceso que consta de dos pasos.</span><span class="sxs-lookup"><span data-stu-id="e3591-104">Using business relations on contacts is a two-step process.</span></span> <span data-ttu-id="e3591-105">Primero, debe definir el código de relación de negocio.</span><span class="sxs-lookup"><span data-stu-id="e3591-105">First, you define the business relation code.</span></span> <span data-ttu-id="e3591-106">Solo debe realizar este paso una vez para cada relación de negocio.</span><span class="sxs-lookup"><span data-stu-id="e3591-106">You only have to perform this step one time for each business relation.</span></span> <span data-ttu-id="e3591-107">Una vez tenga un código de relación de negocio, puede comenzar a asignar el código a empresas de contacto.</span><span class="sxs-lookup"><span data-stu-id="e3591-107">Once you have a business relation code, you can start to assign the code to contact companies.</span></span>

<span data-ttu-id="e3591-108">**Nota**: Si pretende sincronizar sus contactos con proveedores, clientes o bancos en otras partes de la aplicación, puede ser interesante configurar una relación de negocio para ellos.</span><span class="sxs-lookup"><span data-stu-id="e3591-108">**Note**: If you plan to synchronize your contacts with vendors, customers, or bank accounts in other parts of the application, you may want to set up a business relation for them.</span></span>

## <a name="define-a-business-relation-code"></a><span data-ttu-id="e3591-109">Definir un código de relación de negocio</span><span class="sxs-lookup"><span data-stu-id="e3591-109">Define a Business Relation Code</span></span>
<span data-ttu-id="e3591-110">El código de relación de negocio define una categoría o un tipo de relación de negocio, como BANCO o ABO.</span><span class="sxs-lookup"><span data-stu-id="e3591-110">The business relation code defines a category or type of the business relationship, such as BANK or LAW.</span></span> <span data-ttu-id="e3591-111">Puede tener varios códigos de relación de negocio.</span><span class="sxs-lookup"><span data-stu-id="e3591-111">You can have several business relation codes.</span></span> <span data-ttu-id="e3591-112">Para definir relaciones de negocio, use la ventana **Relaciones de negocio**.</span><span class="sxs-lookup"><span data-stu-id="e3591-112">To define the business relation, you use the **Business Relations** window.</span></span>

1. <span data-ttu-id="e3591-113">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Relaciones de negocio** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="e3591-113">In the top right corner, choose the **Search for Page or Report** icon, enter **Business Relations**, and then choose the related link.</span></span>
2. <span data-ttu-id="e3591-114">Seleccione la acción **Nuevo** e introduzca un código y una descripción.</span><span class="sxs-lookup"><span data-stu-id="e3591-114">Choose the **New** action, and fill in a code and description.</span></span> <span data-ttu-id="e3591-115">El código admite un máximo de 11 caracteres y puede ser cualquier combinación de números y letras.</span><span class="sxs-lookup"><span data-stu-id="e3591-115">The code can be a maximum of 11 characters, and can be any combination of numbers and letters.</span></span>

## <a name="assign-business-relations-to-a-contact"></a><span data-ttu-id="e3591-116">Asignar relaciones de negocio a un contacto</span><span class="sxs-lookup"><span data-stu-id="e3591-116">Assign Business Relations to a Contact</span></span>
<span data-ttu-id="e3591-117">No puede asignar relaciones de contacto a una persona de contacto, solo a empresas.</span><span class="sxs-lookup"><span data-stu-id="e3591-117">You cannot assign business relations to a contact person - only companies.</span></span>

1. <span data-ttu-id="e3591-118">Abra el contacto.</span><span class="sxs-lookup"><span data-stu-id="e3591-118">Open the contact.</span></span>
2. <span data-ttu-id="e3591-119">Seleccione la acción **Empresa** y, a continuación, seleccione la acción **Relaciones de negocio**.</span><span class="sxs-lookup"><span data-stu-id="e3591-119">Choose the **Company** action, and then the **Business Relations** action.</span></span>

    <span data-ttu-id="e3591-120">Se abre la ventana **Relaciones de negocio de contacto**.</span><span class="sxs-lookup"><span data-stu-id="e3591-120">The **Contact Business Relations** window opens.</span></span>
3. <span data-ttu-id="e3591-121">En el campo **Cód. relación negocio**, seleccione la relación de negocio que desea asignar.</span><span class="sxs-lookup"><span data-stu-id="e3591-121">In the **Business Relation Code** field, select the business relation you want to assign.</span></span>

<span data-ttu-id="e3591-122">Repita estos pasos para asignar todos las relaciones de negocio que desee.</span><span class="sxs-lookup"><span data-stu-id="e3591-122">Repeat these steps to assign as many business relations as you want.</span></span> <span data-ttu-id="e3591-123">También puede asignar relaciones de negocio desde la lista de contactos con el mismo procedimiento.</span><span class="sxs-lookup"><span data-stu-id="e3591-123">You can also assign business relations from the contact list by following the same procedure.</span></span>

<span data-ttu-id="e3591-124">Aparece automáticamente el número de relaciones de negocio asignadas al contacto del campo **N.º de relaciones de negocio** en la sección **Segmentación** de la ventana **Contacto**.</span><span class="sxs-lookup"><span data-stu-id="e3591-124">The number of business relations you have assigned to the contact is displayed in the **No. of Business Relations** field in the **Segmentation** section in the **Contact** window.</span></span>

<span data-ttu-id="e3591-125">Después de asignar relaciones de negocio a sus contactos, puede utilizar esa información para seleccionar contactos para sus segmentos.</span><span class="sxs-lookup"><span data-stu-id="e3591-125">After you have assigned business relations to your contacts, you can use this information to select contacts for your segments.</span></span> <span data-ttu-id="e3591-126">Para obtener más información, vea [Procedimiento: Agregar contactos a segmentos](marketing-add-contact-segment.md).</span><span class="sxs-lookup"><span data-stu-id="e3591-126">For more information, see [How to: Add Contacts to Segments](marketing-add-contact-segment.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="e3591-127">Consulte también</span><span class="sxs-lookup"><span data-stu-id="e3591-127">See Also</span></span>
[<span data-ttu-id="e3591-128">Crear empresas de contacto</span><span class="sxs-lookup"><span data-stu-id="e3591-128">Create Contact Companies</span></span>](marketing-create-contact-companies.md)

