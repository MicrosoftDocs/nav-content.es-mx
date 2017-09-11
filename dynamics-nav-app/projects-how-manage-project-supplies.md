---
title: "Administración de suministros de proyecto"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00b9ed8480f6b5ab9265beb0fe2dc0060b1c3192
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-job-supplies"></a><span data-ttu-id="47fa0-102">Administración de suministros de proyecto</span><span class="sxs-lookup"><span data-stu-id="47fa0-102">How to: Manage Job Supplies</span></span>
<span data-ttu-id="47fa0-103">La administración de los suministros de los productos, servicios y gastos de un proyecto es un aspecto clave y fundamental de la ejecución de todos los proyectos.</span><span class="sxs-lookup"><span data-stu-id="47fa0-103">Managing project supplies of items, services, and expenses is an integral and critical aspect of the execution of all jobs.</span></span> <span data-ttu-id="47fa0-104">Puede utilizar las cantidades de inventario o realizar compras de proyecto mediante pedidos de compra o facturas de compra.</span><span class="sxs-lookup"><span data-stu-id="47fa0-104">You can use inventory quantities or make job-specific purchases using purchase orders or purchase invoices.</span></span> <span data-ttu-id="47fa0-105">Por ejemplo, un proyecto de servicio en un equipo precisa un disco nuevo.</span><span class="sxs-lookup"><span data-stu-id="47fa0-105">For example, a service job on a computer requires a new disk.</span></span> <span data-ttu-id="47fa0-106">Debe crear una factura de compra para comprar un disco nuevo y registrar el proyecto en el que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="47fa0-106">You create a purchase invoice to buy a new disk and record the job that it will be used on.</span></span>

<span data-ttu-id="47fa0-107">Si el proceso de compra no requiere que la transacción física de registre por separado, se puede procesar una compra en la ventana **Diario general proyecto**.</span><span class="sxs-lookup"><span data-stu-id="47fa0-107">If the purchase process does not require that the physical transaction be recorded separately, then a purchase may be processed in the **Job G/L Journal** window.</span></span> <span data-ttu-id="47fa0-108">Para obtener más información, consulte [Registro del uso para proyectos](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="47fa0-108">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

## <a name="to-purchase-items-or-services-for-a-job"></a><span data-ttu-id="47fa0-109">Para comprar productos o servicios para un proyecto</span><span class="sxs-lookup"><span data-stu-id="47fa0-109">To purchase items or services for a job</span></span>
<span data-ttu-id="47fa0-110">El siguiente procedimiento muestra cómo utilizar una factura de compra para comprar productos de un proyecto.</span><span class="sxs-lookup"><span data-stu-id="47fa0-110">The following procedure shows how to use a purchase invoice to purchase products for a job.</span></span> <span data-ttu-id="47fa0-111">Los mismos pasos se aplican al utilizar un pedido de compra.</span><span class="sxs-lookup"><span data-stu-id="47fa0-111">The same steps apply when using a purchase order.</span></span>  

1. <span data-ttu-id="47fa0-112">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Facturas de compra** y, a continuación, elija el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="47fa0-112">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchase Invoices**, and then choose the related link.</span></span>  
2. <span data-ttu-id="47fa0-113">Elija la acción **Nuevo** y, a continuación, rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="47fa0-113">Choose the **New** action and fill in the fields as necessary.</span></span> <span data-ttu-id="47fa0-114">Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="47fa0-114">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
3. <span data-ttu-id="47fa0-115">En los campos **N.º de proyecto**</span><span class="sxs-lookup"><span data-stu-id="47fa0-115">In the **Job No.**</span></span> <span data-ttu-id="47fa0-116">y **N.º tarea de proyecto**,</span><span class="sxs-lookup"><span data-stu-id="47fa0-116">and **Job Task No.**</span></span> <span data-ttu-id="47fa0-117">seleccione la información del proyecto para el que desea comprar productos o servicios.</span><span class="sxs-lookup"><span data-stu-id="47fa0-117">fields, select the information of the job that you want to purchase items or services for.</span></span>  

    <span data-ttu-id="47fa0-118">El valor que seleccione en el campo **Tipo línea proyecto** define si una línea de planificación se crea cuando registra el uso del producto.</span><span class="sxs-lookup"><span data-stu-id="47fa0-118">The value that you select in the **Job Line Type** field defines whether a planning line is created when you post the usage of the item.</span></span> <span data-ttu-id="47fa0-119">Si el campo contiene **Facturable**, se crean las líneas de planificación de proyecto preparadas para facturarlas al cliente.</span><span class="sxs-lookup"><span data-stu-id="47fa0-119">If the field contains **Billable**, then job planning lines that are ready to be invoiced to the customer are created.</span></span> <span data-ttu-id="47fa0-120">Para obtener más información, vea [Facturación de proyectos](projects-how-invoice-jobs.md).</span><span class="sxs-lookup"><span data-stu-id="47fa0-120">For more information, see [How to: Invoice Jobs](projects-how-invoice-jobs.md).</span></span>

4. <span data-ttu-id="47fa0-121">Seleccione la acción **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="47fa0-121">Choose the **Post** action.</span></span>

## <a name="to-view-the-value-of-purchases-for-a-job"></a><span data-ttu-id="47fa0-122">Para ver el valor de compras de un proyecto</span><span class="sxs-lookup"><span data-stu-id="47fa0-122">To view the value of purchases for a job</span></span>  

1. <span data-ttu-id="47fa0-123">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proyectos** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="47fa0-123">In the top right corner, choose the **Search for Page or Report** icon, enter **Jobs**, and then choose the related link.</span></span>
2. <span data-ttu-id="47fa0-124">Abra una ficha de un proyecto relevante.</span><span class="sxs-lookup"><span data-stu-id="47fa0-124">Open a relevant job card.</span></span>

    <span data-ttu-id="47fa0-125">En la ficha desplegable **Tareas**, el campo **Pedidos pendientes** muestra el importe total de los pedidos en divisa local, los productos y servicios de inventario en los documentos de compras de la línea de tarea de proyecto.</span><span class="sxs-lookup"><span data-stu-id="47fa0-125">On the **Tasks** FastTab, the **Outstanding Orders** field shows the total outstanding amount, in local currency, of inventory items and services on purchase documents for the job task line.</span></span>  

    <span data-ttu-id="47fa0-126">El campo **Importe recibido no facturado** muestra el valor de los productos entregados en un documento de compra pero que no están facturados.</span><span class="sxs-lookup"><span data-stu-id="47fa0-126">The **Amt. Rec. Not Invoiced** field shows the value of items delivered on purchase documents, but not yet invoiced.</span></span>  

3. <span data-ttu-id="47fa0-127">Seleccione cualquier de los campos para abrir la ventana **Líns. compra** donde puede revisar la información sobre las líneas de documento de compra, incluyendo qué productos o servicios se han recibido.</span><span class="sxs-lookup"><span data-stu-id="47fa0-127">Choose either of the fields to open the **Purchase Lines** window where you can review information about the related purchase document lines, including which items or services have been received.</span></span>

## <a name="to-post-a-job-related-expense"></a><span data-ttu-id="47fa0-128">Para registrar un gasto relacionado con el proyecto</span><span class="sxs-lookup"><span data-stu-id="47fa0-128">To post a job-related expense</span></span>  
<span data-ttu-id="47fa0-129">Si tiene costes de proyecto extraordinarios o únicos, puede utilizar la ventana **Diario general proyecto** para enviarlos directamente a la cuenta de proyecto relevante.</span><span class="sxs-lookup"><span data-stu-id="47fa0-129">If you incur extraordinary or one-time job expenses, you can use the **Job G/L Journal** window to post them directly to the relevant job account.</span></span>

1. <span data-ttu-id="47fa0-130">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios generales proyecto** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="47fa0-130">In the top right corner, choose the **Search for Page or Report** icon, enter **Job G/L Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="47fa0-131">Cree una línea nueva y especifique los datos del gasto, incluyendo la información en los campos **N.º proyecto**</span><span class="sxs-lookup"><span data-stu-id="47fa0-131">Create a new line and enter information about the expense, including information in the **Job No.**</span></span> <span data-ttu-id="47fa0-132">y **N.º tarea de proyecto**.</span><span class="sxs-lookup"><span data-stu-id="47fa0-132">and **Job Task No** fields.</span></span>  
3. <span data-ttu-id="47fa0-133">Cuando el diario esté completo, seleccione la acción **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="47fa0-133">When the journal is complete, choose the **Post** action.</span></span>


## <a name="see-also"></a><span data-ttu-id="47fa0-134">Consulte también</span><span class="sxs-lookup"><span data-stu-id="47fa0-134">See Also</span></span>
[<span data-ttu-id="47fa0-135">Administrar proyectos</span><span class="sxs-lookup"><span data-stu-id="47fa0-135">Manage Projects</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="47fa0-136">Finanzas</span><span class="sxs-lookup"><span data-stu-id="47fa0-136">Finance</span></span>](finance-setup.md)  
<span data-ttu-id="47fa0-137">[Gestionar compras](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="47fa0-137">[Manage Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="47fa0-138">[Gestionar ventas](sales-manage-sales.md)    </span><span class="sxs-lookup"><span data-stu-id="47fa0-138">[Manage Sales](sales-manage-sales.md)    </span></span>  
[<span data-ttu-id="47fa0-139">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="47fa0-139">Work With Dynamics NAV</span></span>](ui-work-product.md)  

