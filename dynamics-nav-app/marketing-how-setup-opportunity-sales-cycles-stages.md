---
title: 'Procedimiento: Configurar etapas y ciclos de ventas de oportunidad'
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
ms.openlocfilehash: 756e9b2f33fe66cd4c2b4e26ca4390683bd087af
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-set-up-opportunity-sales-cycles-and-cycle-stages"></a><span data-ttu-id="f5cbe-102">Procedimiento: Configurar etapas y ciclos de ventas de oportunidad</span><span class="sxs-lookup"><span data-stu-id="f5cbe-102">How to: Set Up Opportunity Sales Cycles and Cycle Stages</span></span>
<span data-ttu-id="f5cbe-103">Para poder usar oportunidades de ventas, debe configurar los ciclos de ventas y las etapas del ciclo de ventas.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-103">Before you can start using sales opportunities, you must set up sales cycles and sales cycle stages.</span></span> <span data-ttu-id="f5cbe-104">Un ciclo de ventas se compone de una serie de etapas que van desde el contacto inicial hasta el cierre de una venta.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-104">A sales cycle is made up of a series of stages that go from the initial contact to the closing of a sale.</span></span> <span data-ttu-id="f5cbe-105">Cada etapa puede tener determinados requisitos que se deben cumplir, por ejemplo, requerir una cotización venta, antes de que la oportunidad pueda pasar a la siguiente etapa.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-105">Each stage can have certain requirements that must be met, such as requiring a sales quote, before an opportunity can go to the next stage.</span></span> <span data-ttu-id="f5cbe-106">También puede especificar si se puede omitir una etapa.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-106">You can also specify whether a stage can be skipped.</span></span> <span data-ttu-id="f5cbe-107">Puede configurar tantos ciclos de ventas como necesite y tantas etapas del ciclo de ventas como sean necesarias para el ciclo de ventas.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-107">You can setup as many sales cycles as you need, and you can set up as many sales cycle stages as necessary within a sales cycle.</span></span>

<span data-ttu-id="f5cbe-108">La implementación de ciclos de ventas de oportunidad implica tanto la configuración del código de ciclo de ventas, que define las diferentes etapas del ciclo, como la asignación del ciclo a oportunidades.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-108">Implementing opportunity sales cycles involves setting up the sales cycle code, defining the different stages of the cycle, and then assigning the cycle to opportunities.</span></span>

## <a name="to-set-up-an-opportunity-sales-cycle-code"></a><span data-ttu-id="f5cbe-109">Para configurar un código de ciclo de ventas de oportunidad</span><span class="sxs-lookup"><span data-stu-id="f5cbe-109">To set up an opportunity sales cycle code</span></span>
1. <span data-ttu-id="f5cbe-110">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Ciclos de ventas** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales Cycles**, and then choose the related link.</span></span> <span data-ttu-id="f5cbe-111">Se abre la ventana **Ciclos de ventas** y se muestran todos los ciclos de ventas existentes.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-111">The **Sales Cycles** window opens, and lists all the existing sales cycles.</span></span>
2. <span data-ttu-id="f5cbe-112">Seleccione la acción **Nuevo** y rellene los campos.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-112">Choose the **New** action, and fill in the fields.</span></span>

<span data-ttu-id="f5cbe-113">Repita estos pasos para configurar todos los ciclos de venta que desee.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-113">Repeat these steps to set up as many sales cycles as you want.</span></span> <span data-ttu-id="f5cbe-114">Después de configurar los ciclos de ventas de oportunidad, puede que quiera configurar las distintas etapas de cada ciclo.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-114">After you have set up opportunity sales cycles, you may want to set up the different stages within each cycle.</span></span>

## <a name="to-define-opportunity-sales-cycle-stages"></a><span data-ttu-id="f5cbe-115">Para definir las etapas del ciclo de ventas de oportunidad</span><span class="sxs-lookup"><span data-stu-id="f5cbe-115">To define opportunity sales cycle stages</span></span>
1. <span data-ttu-id="f5cbe-116">En la ventana **Ciclos de ventas**, seleccione el ciclo de ventas de oportunidad para el que quiere configurar etapas y, a continuación, seleccione la acción **Etapas**.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-116">In the **Sales Cycles** window, select the opportunity sales cycle for which you want to set up stages, and then choose the **Stages** action.</span></span> <span data-ttu-id="f5cbe-117">Se abre la ventana **Etapas de ciclo de ventas**.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-117">The **Sales Cycle Stages** window opens.</span></span>
2. <span data-ttu-id="f5cbe-118">Seleccione la acción **Nuevo** para introducir una nueva etapa en el ciclo de ventas.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-118">Choose the **New** action to enter a new stage in the sales cycle.</span></span>

<span data-ttu-id="f5cbe-119">Repita estos pasos para configurar tantas etapas como desee en el ciclo de ventas.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-119">Repeat these steps to set up as many stages as you want within the sales cycle.</span></span>

## <a name="to-assign-stage-cycle-to-an-opportunity"></a><span data-ttu-id="f5cbe-120">Para asignar el ciclo de la etapa a una oportunidad</span><span class="sxs-lookup"><span data-stu-id="f5cbe-120">To assign stage cycle to an opportunity</span></span>
<span data-ttu-id="f5cbe-121">Cuando haya agregado el ciclo de la etapa de oportunidades, puede empezar a agregar oportunidades de ventas y, a continuación, asignar el ciclo de la etapa a oportunidades configurando el campo **Código de ciclo de ventas**.</span><span class="sxs-lookup"><span data-stu-id="f5cbe-121">After you add the opportunities stage cycle, you can start to add sales opportunities, and then assign the stage cycle to opportunities by setting the **Sales Cycle Code** field.</span></span> <span data-ttu-id="f5cbe-122">Para obtener más información, consulte [Procedimiento: Crear oportunidades de ventas](marketing-how-create-opportunities.md).</span><span class="sxs-lookup"><span data-stu-id="f5cbe-122">For more information, see [How to: Create Sales Opportunities](marketing-how-create-opportunities.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="f5cbe-123">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f5cbe-123">See Also</span></span>  
[<span data-ttu-id="f5cbe-124">Procesar oportunidades de ventas</span><span class="sxs-lookup"><span data-stu-id="f5cbe-124">Processing Sales Opportunities</span></span>](marketing-processing-sales-opportunities.md)  
[<span data-ttu-id="f5cbe-125">Gestionar ventas</span><span class="sxs-lookup"><span data-stu-id="f5cbe-125">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="f5cbe-126">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="f5cbe-126">Working with Dynamics NAV</span></span>](ui-work-product.md)

