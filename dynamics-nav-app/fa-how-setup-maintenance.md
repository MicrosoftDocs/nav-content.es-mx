---
title: 'Procedimiento: Configurar el mantenimiento de los activos fijos'
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
ms.openlocfilehash: ace0fb13d2be71c7204f16f34f6b65b54ff98230
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-maintenance"></a><span data-ttu-id="d8d19-102">Procedimiento: Configurar el mantenimiento de los activos fijos</span><span class="sxs-lookup"><span data-stu-id="d8d19-102">How to: Set Up Fixed Asset Maintenance</span></span>
<span data-ttu-id="d8d19-103">Para gestionar el mantenimiento de los activos fijos, primero debe configurar la información de mantenimiento en una cuenta de registro para los costos de mantenimiento y los códigos de mantenimiento para los tipos de trabajo, por ejemplo, Servicio de rutina o Reparación.</span><span class="sxs-lookup"><span data-stu-id="d8d19-103">To manage fixed asset maintenance, you must first set up some general maintenance information, a posting account for maintenance costs, and maintenance codes for types of work, such as Routine Service or Repair.</span></span>

## <a name="to-set-up-general-maintenance-information"></a><span data-ttu-id="d8d19-104">Para configurar la información general de mantenimiento</span><span class="sxs-lookup"><span data-stu-id="d8d19-104">To set up general maintenance information</span></span>
<span data-ttu-id="d8d19-105">Si configura los campos para el mantenimiento, puede registrar los gastos de mantenimiento en un diario de activos fijos.</span><span class="sxs-lookup"><span data-stu-id="d8d19-105">If you set up the fields for maintenance, you can post maintenance expenses from the fixed asset journal.</span></span>
1. <span data-ttu-id="d8d19-106">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="d8d19-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Fixed Assets**, and then choose the related link.</span></span>
2. <span data-ttu-id="d8d19-107">Seleccione el activo fijo del que definirá la cobertura de seguro y, a continuación, elija la acción **Editar**.</span><span class="sxs-lookup"><span data-stu-id="d8d19-107">Select the fixed asset that you to define insurance coverage for, and then choose the **Edit** action.</span></span>
3. <span data-ttu-id="d8d19-108">En la ficha desplegable **Mantenimiento**, rellene los campos como sea necesario.</span><span class="sxs-lookup"><span data-stu-id="d8d19-108">On the **Maintenance** FastTab, fill in the fields as necessary.</span></span> <span data-ttu-id="d8d19-109">Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.</span><span class="sxs-lookup"><span data-stu-id="d8d19-109">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-maintenance-codes"></a><span data-ttu-id="d8d19-110">Para configurar los códigos de mantenimiento</span><span class="sxs-lookup"><span data-stu-id="d8d19-110">To set up maintenance codes</span></span>  
<span data-ttu-id="d8d19-111">Al registrar costos de mantenimiento desde un diario general, puede rellenar el campo **Cód. mantenimiento** para registrar el tipo de mantenimiento efectuado, como un servicio rutinario o una reparación.</span><span class="sxs-lookup"><span data-stu-id="d8d19-111">When you post maintenance costs from a general journal, you fill in the **Maintenance Code** field to record what kind of maintenance has been performed, such as routine service or repair.</span></span>
1. <span data-ttu-id="d8d19-112">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Mantenimiento** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="d8d19-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Maintenance**, and then choose the related link.</span></span>
2. <span data-ttu-id="d8d19-113">En la ventana **Mantenimiento**, configure los códigos para cada tipo de trabajo de mantenimiento.</span><span class="sxs-lookup"><span data-stu-id="d8d19-113">In the **Maintenance** window, set up codes for different types of maintenance work.</span></span>

## <a name="to-set-up-maintenance-expense-accounts"></a><span data-ttu-id="d8d19-114">Para configurar las cuentas de gastos de mantenimiento</span><span class="sxs-lookup"><span data-stu-id="d8d19-114">To set up maintenance expense accounts</span></span>  
<span data-ttu-id="d8d19-115">Para registrar los costos de mantenimiento, primero debe introducir un número de cuenta en la ventana **A/F Grupos contables**.</span><span class="sxs-lookup"><span data-stu-id="d8d19-115">To post maintenance costs, you must first enter an account number in the **FA Posting Groups** window.</span></span>
1. <span data-ttu-id="d8d19-116">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **A/F Grupos contables** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="d8d19-116">In the top right corner, choose the **Search for Page or Report** icon, enter **FA Posting Groups**, and then choose the related link.</span></span>
2. <span data-ttu-id="d8d19-117">Rellene el campo **Cta. gastos mantenimiento** de cada grupo contable.</span><span class="sxs-lookup"><span data-stu-id="d8d19-117">Fill in the **Maintenance Expense Account** field for each posting group.</span></span>

<span data-ttu-id="d8d19-118">**Nota**: Para indicar que los costos de mantenimiento están distribuidos entre departamentos o proyectos, debe configurar claves de distribución.</span><span class="sxs-lookup"><span data-stu-id="d8d19-118">**Note**: To define that maintenance costs are allocated to departments or projects, set up an allocation keys.</span></span> <span data-ttu-id="d8d19-119">Para obtener más información, consulte [Procedimiento: Configurar funciones generales a los activos fijos](fa-how-setup-general.md).</span><span class="sxs-lookup"><span data-stu-id="d8d19-119">For more information, see [How to: Set Up General Fixed Assets Features](fa-how-setup-general.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="d8d19-120">Consulte también</span><span class="sxs-lookup"><span data-stu-id="d8d19-120">See Also</span></span>
[<span data-ttu-id="d8d19-121">Configuración de activos fijos</span><span class="sxs-lookup"><span data-stu-id="d8d19-121">Set Up Fixed Assets</span></span>](fa-setup.md)  
[<span data-ttu-id="d8d19-122">Gestión de activos fijos</span><span class="sxs-lookup"><span data-stu-id="d8d19-122">Manage Fixed Assets</span></span>](fa-manage.md)  
[<span data-ttu-id="d8d19-123">Finanzas</span><span class="sxs-lookup"><span data-stu-id="d8d19-123">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="d8d19-124">Este es Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="d8d19-124">Welcome to Dynamics NAV</span></span>](across-get-started.md)

