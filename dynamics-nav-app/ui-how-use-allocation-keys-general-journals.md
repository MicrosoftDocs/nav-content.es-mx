---
title: "Procedimiento: utilizar claves de asignación en diarios generales"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ca21d9d129dbc98d75371d1b2b7a0ffad4aa2848
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a><span data-ttu-id="e7c5d-102">Procedimiento: utilizar claves de asignación en diarios generales</span><span class="sxs-lookup"><span data-stu-id="e7c5d-102">How to: Use Allocation Keys in General Journals</span></span>
<span data-ttu-id="e7c5d-103">Puede asignar un movimiento en un diario general a varias cuentas diferentes al registrar el diario.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-103">You can allocate an entry in a general journal to several different accounts when you post the journal.</span></span> <span data-ttu-id="e7c5d-104">La distribución puede realizarse por cantidad, porcentaje o importe.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-104">The allocation can be made by quantity, percentage, or amount.</span></span>

## <a name="to-set-up-allocation-keys"></a><span data-ttu-id="e7c5d-105">Para configurar claves de asignación</span><span class="sxs-lookup"><span data-stu-id="e7c5d-105">To set up allocation keys</span></span> 
1. <span data-ttu-id="e7c5d-106">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general periódico** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-106">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="e7c5d-107">Seleccione el campo **Nombre de sección** para abrir la ventana **Secciones diario general**.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-107">Choose the **Batch Name** field to open the **General Journal Batches** window.</span></span>
3. <span data-ttu-id="e7c5d-108">Puede modificar las asignaciones en una sección existente de la lista o crear une nueva sección con asignaciones.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-108">You can either modify allocations on an existing batch in the list or create a new batch with allocations.</span></span>
  * <span data-ttu-id="e7c5d-109">Para crear un lote nuevo, seleccione la acción **Nuevo** y vaya al paso siguiente.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-109">To create a new batch, choose the **New** action, and go to the next step.</span></span>
  * <span data-ttu-id="e7c5d-110">Para cambiar las asignaciones de un diario existente, seleccione el diario y vaya al paso 7.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-110">To change the allocations of an existing journal, select the journal and go to step 7.</span></span>    
4. <span data-ttu-id="e7c5d-111">En el campo **Nombre**, escriba un nombre para la sección, por ejemplo LIMPIEZA.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-111">In the **Name** field, enter a name for the batch, such as CLEANING.</span></span> <span data-ttu-id="e7c5d-112">En el campo **Descripción**, escriba una descripción, por ejemplo, Limpieza de diario de gastos.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-112">In the **Description** field, enter a description, such as Cleaning Expenses Journal.</span></span>
5. <span data-ttu-id="e7c5d-113">Cuando haya terminado, cierre la ventana.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-113">When you are done, close the window.</span></span> <span data-ttu-id="e7c5d-114">Aparecerá un nuevo diario periódico vacío.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-114">A new, empty recurring journal opens.</span></span> 
6. <span data-ttu-id="e7c5d-115">Complete los campos de la línea.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-115">Fill in the fields in the line.</span></span>
7. <span data-ttu-id="e7c5d-116">Seleccione la acción **Asignaciones**.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-116">Choose the **Allocations** action.</span></span> 
8. <span data-ttu-id="e7c5d-117">Agregue una línea para cada asignación.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-117">Add a line for each allocation.</span></span> <span data-ttu-id="e7c5d-118">Debe rellenar el campo **% Distribución**, **Cantidad a distribuir** o **Importe**.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-118">You must fill in either the **Allocation %**, **Allocation Quantity**, or **Amount** field.</span></span> <span data-ttu-id="e7c5d-119">también debe rellenar el campo **N.º de cuenta**</span><span class="sxs-lookup"><span data-stu-id="e7c5d-119">You must also fill in the **Account No.**</span></span> <span data-ttu-id="e7c5d-120">y, si distribuye la transacción entre dimensiones globales, los campos de dimensión global.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-120">field and, if you are allocating the transaction among global dimensions, the global dimension fields.</span></span>
9. <span data-ttu-id="e7c5d-121">Si escribe un porcentaje en una línea, el importe del campo **Importe** se calcula automáticamente.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-121">If you enter a percentage on a line, the amount in the **Amount** field is calculated automatically.</span></span> <span data-ttu-id="e7c5d-122">Estos importes tienen el signo contrario al importe total del campo **Importe** en el diario periódico.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-122">These amounts have the opposite sign from the total amount in the **Amount** field in the recurring journal.</span></span>
10. <span data-ttu-id="e7c5d-123">Después de introducir las líneas de asignaciones, seleccione **Aceptar** para volver a la ventana **Diario general periódico**.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-123">After entering the allocations lines, choose **OK** to return to the **Recurring General Journal** window.</span></span> <span data-ttu-id="e7c5d-124">El campo **Importe asignado (USD)** se rellena y coincide con el campo **Importe**.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-124">The **Allocated Amt. (USD)** field is filled in and matches the **Amount** field.</span></span>
11. <span data-ttu-id="e7c5d-125">Registre el diario.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-125">Post the journal.</span></span>

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a><span data-ttu-id="e7c5d-126">Para modificar una clave de asignación que ya haya sido configurada</span><span class="sxs-lookup"><span data-stu-id="e7c5d-126">To change an allocation key that has already been set up</span></span>
1. <span data-ttu-id="e7c5d-127">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general periódico** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-127">In the top right corner, choose the **Search for Page or Report** icon, enter **Recurring General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="e7c5d-128">En la ventana **Diarios generales periódicos**, seleccione el diario con la distribución.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-128">In the **Recurring General Journal** window, select the journal with the allocation.</span></span>
3. <span data-ttu-id="e7c5d-129">Seleccione la línea con la asignación y, a continuación, seleccione la acción **Asignaciones**.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-129">Choose the line with the allocation, and then choose **Allocations** action.</span></span>
4. <span data-ttu-id="e7c5d-130">Modifique los campos correspondientes y cierre la ventana.</span><span class="sxs-lookup"><span data-stu-id="e7c5d-130">Change the relevant fields, and close the window.</span></span>

## <a name="see-also"></a><span data-ttu-id="e7c5d-131">Consulte también</span><span class="sxs-lookup"><span data-stu-id="e7c5d-131">See Also</span></span>
[<span data-ttu-id="e7c5d-132">Trabajar con diarios generales</span><span class="sxs-lookup"><span data-stu-id="e7c5d-132">Work With General Journals</span></span>](ui-work-general-journals.md)  
[<span data-ttu-id="e7c5d-133">Registrar documentos y diarios</span><span class="sxs-lookup"><span data-stu-id="e7c5d-133">Post Documents and Journals</span></span>](ui-post-documents-journals.md)




