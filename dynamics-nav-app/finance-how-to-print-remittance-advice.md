---
title: Imprimir un aviso de pago
description: "Puede ayudar a sus proveedores a realizar conciliaciones si imprime un aviso de pago antes de publicar un diario de pagos y después de registrar un pago."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: 71c84b4a7bad83e6008c0fa34f908e133b014a59
ms.contentlocale: es-mx
ms.lasthandoff: 10/26/2017

---

#<a name="how-to-print-remittance-advice"></a><span data-ttu-id="022bd-103">Imprimir un aviso de pago</span><span class="sxs-lookup"><span data-stu-id="022bd-103">How to: Print Remittance Advice</span></span>
<span data-ttu-id="022bd-104">Puede imprimir el aviso de pago antes de registrar el diario de pagos y después de registrar un pago.</span><span class="sxs-lookup"><span data-stu-id="022bd-104">You can print remittance advice before posting a payment journal and after posting a payment.</span></span> <span data-ttu-id="022bd-105">Este aviso muestra números de factura del proveedor que ayudan a los proveedores a realizar la conciliación.</span><span class="sxs-lookup"><span data-stu-id="022bd-105">This advice displays vendor invoice numbers, which helps vendors to perform reconciliations.</span></span>

##<a name="to-print-remittance-advice"></a><span data-ttu-id="022bd-106">Para imprimir un aviso de pago</span><span class="sxs-lookup"><span data-stu-id="022bd-106">To print remittance advice</span></span>
1. <span data-ttu-id="022bd-107">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios de pagos** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="022bd-107">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Payment Journals**, and then choose the related link.</span></span>  
2. <span data-ttu-id="022bd-108">En la ventana **Diario de pagos**, seleccione el pago para el que se debe imprimir el aviso de pago.</span><span class="sxs-lookup"><span data-stu-id="022bd-108">In the **Payment Journal** window, select the payment for which remittance advice must be printed.</span></span>  
3. <span data-ttu-id="022bd-109">Seleccione la acción **Imprimir un aviso de pago**.</span><span class="sxs-lookup"><span data-stu-id="022bd-109">Choose the **Print Remittance Advice** action.</span></span>  
4. <span data-ttu-id="022bd-110">En el proceso **Aviso de pago - Diario**, en la ficha desplegable **Lín. diario general**, seleccione los filtros apropiados.</span><span class="sxs-lookup"><span data-stu-id="022bd-110">In the **Remittance Advice - Journal** batch job, on the **Fen. Journal Line** FastTab, choose the appropriate filters.</span></span>  
  
    >[!Note]
    > <span data-ttu-id="022bd-111">Puede filtrar mediante el número de documento externo del proveedor para hacer coincidir los pagos con las facturas.</span><span class="sxs-lookup"><span data-stu-id="022bd-111">You can filter using the vendor's external document number to match payments with invoices.</span></span>

5. <span data-ttu-id="022bd-112">En la ficha desplegable **Proveedor**, seleccione los filtros apropiados.</span><span class="sxs-lookup"><span data-stu-id="022bd-112">On the **Vendor** FastTab, choose the appropriate filters.</span></span>  
6. <span data-ttu-id="022bd-113">Elija **Imprimir** para imprimir el informe o **Vista preliminar** para verlo ahora.</span><span class="sxs-lookup"><span data-stu-id="022bd-113">Choose **Print** to print the report, or choose **Preview** to view it now.</span></span>  

## <a name="using-remittance-advice-reports"></a><span data-ttu-id="022bd-114">Mediante informes de aviso de pago</span><span class="sxs-lookup"><span data-stu-id="022bd-114">Using Remittance Advice Reports</span></span>
<span data-ttu-id="022bd-115">En la tabla siguiente se describen los informes que se pueden utilizar con el aviso de pago:</span><span class="sxs-lookup"><span data-stu-id="022bd-115">The following table describes the reports that you can use with remittance advice:</span></span>

|<span data-ttu-id="022bd-116">Informe</span><span class="sxs-lookup"><span data-stu-id="022bd-116">Report</span></span>|<span data-ttu-id="022bd-117">Descripción</span><span class="sxs-lookup"><span data-stu-id="022bd-117">Description</span></span>|
|----|----|
|<span data-ttu-id="022bd-118">Aviso de pago - Informe del diario</span><span class="sxs-lookup"><span data-stu-id="022bd-118">Remittance Advice - Journal Report</span></span>|<span data-ttu-id="022bd-119">Este informe indica qué documentos se incluyen en el pago.</span><span class="sxs-lookup"><span data-stu-id="022bd-119">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="022bd-120">Para las líneas del diario general, puede especificar el libro de diario y la sección de diario desde los que se imprimirán los avisos de remesa, la fecha de la primera actividad para imprimir y filtrar por número de documento.</span><span class="sxs-lookup"><span data-stu-id="022bd-120">For general journal lines, you can specify the journal template and journal batch from which the remittance advices will be printed, the date of the first activity to print, and filter on a document number.</span></span> <span data-ttu-id="022bd-121">Para los proveedores, puede introducir los números de los proveedores que se incluirán en el informe.</span><span class="sxs-lookup"><span data-stu-id="022bd-121">For vendors, you can enter the vendor numbers to include in the report.</span></span> |
|<span data-ttu-id="022bd-122">Aviso pago - Informe de entradas</span><span class="sxs-lookup"><span data-stu-id="022bd-122">Remittance Advice - Entries Report</span></span>| <span data-ttu-id="022bd-123">Este informe indica qué documentos se incluyen en el pago.</span><span class="sxs-lookup"><span data-stu-id="022bd-123">This report indicates which documents are included in the payment.</span></span> <span data-ttu-id="022bd-124">Defina el contenido del informe estableciendo filtros.</span><span class="sxs-lookup"><span data-stu-id="022bd-124">You define the report contents by setting filters.</span></span> <span data-ttu-id="022bd-125">Puede definir campos adicionales en la ficha mediante el campo **Campo**.</span><span class="sxs-lookup"><span data-stu-id="022bd-125">You can set additional fields on the tab by choosing the **Field** field.</span></span> <span data-ttu-id="022bd-126">Para los movimientos de proveedor, puede especificar los proveedores que se incluirán en el informe, la fecha de la primera actividad a imprimir, la divisa y el número del movimiento.</span><span class="sxs-lookup"><span data-stu-id="022bd-126">For vendor ledger entries, you can specify the vendors to include in the report, the date of the first activity to print, the currency, and the entry number to include.</span></span> |

> [!Note]
> <span data-ttu-id="022bd-127">El Aviso de pago - Informe del diario no admite escenarios de aplicación de divisa cruzada ni tolerancias de pago.</span><span class="sxs-lookup"><span data-stu-id="022bd-127">The Remittance Advice - Journal Report does not support cross currency application scenarios or payment tolerances.</span></span> <span data-ttu-id="022bd-128">Para obtener más información vea, [Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas](finance-how-enable-application-ledger-entries-different-currencies.md).</span><span class="sxs-lookup"><span data-stu-id="022bd-128">For more information, see [How to: Enable Application of Ledger Entries in Different Currencies](finance-how-enable-application-ledger-entries-different-currencies.md).</span></span>

> [!Tip]
> <span data-ttu-id="022bd-129">Para obtener más información sobre cómo usar los informes, consulte [Visualización de los informes de prueba antes de realizar el registro](ui-how-view-test-reports-posting.md), [Trabajar con informes](ui-work-report.md) y [Buscar, filtrar y ordenar datos](ui-enter-criteria-filters.md).</span><span class="sxs-lookup"><span data-stu-id="022bd-129">For more information about how to work with reports, see [Viewing Test Reports before Posting](ui-how-view-test-reports-posting.md), [Work with Reports](ui-work-report.md), and [Searching, Filtering, and Sorting Data](ui-enter-criteria-filters.md).</span></span>

##<a name="see-also"></a><span data-ttu-id="022bd-130">Consulte también</span><span class="sxs-lookup"><span data-stu-id="022bd-130">See Also</span></span>  
[<span data-ttu-id="022bd-131">Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="022bd-131">Welcome to Dynamics NAV</span></span>](across-get-started.md)
