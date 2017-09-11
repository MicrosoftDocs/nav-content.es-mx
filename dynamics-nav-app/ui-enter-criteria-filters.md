---
title: Introducir criterios en los filtros
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: df386e1195db385ee053b69fec0f5082d8df4116
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="entering-criteria-in-filters"></a><span data-ttu-id="fcf9a-102">Introducir criterios en los filtros</span><span class="sxs-lookup"><span data-stu-id="fcf9a-102">Entering Criteria in Filters</span></span>
<span data-ttu-id="fcf9a-103">Cuando quiera buscar datos, como nombres de cliente, direcciones o grupos de productos, puede introducir los criterios.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-103">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="fcf9a-104">En los criterios de búsqueda puede usar todos los números y las letras que normalmente se emplean en un campo específico.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-104">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="fcf9a-105">También puede usar símbolos especiales o expresiones matemáticas para filtrar aún más los resultados.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-105">In addition, you can use special symbols to further filter the results.</span></span>

## <a name="searching-using-the-quick-filter"></a><span data-ttu-id="fcf9a-106">Búsqueda mediante el filtro rápido</span><span class="sxs-lookup"><span data-stu-id="fcf9a-106">Searching using the Quick Filter</span></span>
<span data-ttu-id="fcf9a-107">Puede agregar filtros a todas las páginas con el filtro rápido.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-107">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="fcf9a-108">El filtro rápido se activa al elegir el icono de la lupa que se encuentra en la esquina superior derecha de una página.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-108">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="fcf9a-109">Este tipo de filtro se utiliza para una rápida introducción de criterios.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-109">This filtering type is used for a fast entry of criteria.</span></span>

<span data-ttu-id="fcf9a-110">**Importante**: El filtro rápido proporciona un acceso sencillo a los datos de filtro mediante la especificación de texto simple, pero también proporciona muchas opciones de criterios de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-110">**Important**: The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="fcf9a-111">El filtro rápido actúa de distinta forma dependiendo de si introduce texto sin formato o texto con símbolos.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-111">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  
- <span data-ttu-id="fcf9a-112">Si se introduce texto sin formato en los criterios de búsqueda, estos se interpretan como una búsqueda que tendrá en cuenta mayúsculas y minúsculas y que contendrá un determinado texto.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-112">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
- <span data-ttu-id="fcf9a-113">Si se introduce texto con símbolos en los criterios de búsqueda, estos se interpretan exactamente como se haya introducido este texto y teniendo en cuenta mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-113">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="fcf9a-114">Criterios del filtro rápido</span><span class="sxs-lookup"><span data-stu-id="fcf9a-114">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="fcf9a-115">Criterios de búsqueda</span><span class="sxs-lookup"><span data-stu-id="fcf9a-115">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="fcf9a-116">Interpretado como…</span><span class="sxs-lookup"><span data-stu-id="fcf9a-116">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="fcf9a-117">Devoluciones...</span><span class="sxs-lookup"><span data-stu-id="fcf9a-117">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="fcf9a-118">>man</span><span class="sxs-lookup"><span data-stu-id="fcf9a-118">>man</span></span></TD>
    <TD><span data-ttu-id="fcf9a-119">@*man*</span><span class="sxs-lookup"><span data-stu-id="fcf9a-119">@*man*</span></span></TD>
    <TD><span data-ttu-id="fcf9a-120">Todos los registros que contienen el texto man y respetando mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-120">All records that contain the text man and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="fcf9a-121">>se</span><span class="sxs-lookup"><span data-stu-id="fcf9a-121">>se</span></span></TD>
    <TD><span data-ttu-id="fcf9a-122">@*se*</span><span class="sxs-lookup"><span data-stu-id="fcf9a-122">@*se*</span></span></TD>
    <TD><span data-ttu-id="fcf9a-123">Todos los registros que contienen el texto se y respetando mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-123">All records that contain the text se and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="fcf9a-124">>Man*</span><span class="sxs-lookup"><span data-stu-id="fcf9a-124">>Man*</span></span></TD>
    <TD><span data-ttu-id="fcf9a-125">Empieza por Man y distingue mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-125">Starts with Man and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="fcf9a-126">Todos los registros que empiecen por el texto Man.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-126">All records that start with the text Man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="fcf9a-127">'man'</span><span class="sxs-lookup"><span data-stu-id="fcf9a-127">'man'</span></span></TD>
    <TD><span data-ttu-id="fcf9a-128">Un texto exacto respetando mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-128">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="fcf9a-129">Todos los registros que coincidan exactamente con man.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-129">All records that match man exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="fcf9a-130">@*man</span><span class="sxs-lookup"><span data-stu-id="fcf9a-130">@*man</span></span></TD>
    <TD><span data-ttu-id="fcf9a-131">Termina en y distingue mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-131">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="fcf9a-132">Todos los registros que terminen en man.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-132">All records that end with man.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="fcf9a-133">@man*</span><span class="sxs-lookup"><span data-stu-id="fcf9a-133">@man*</span></span></TD>
    <TD><span data-ttu-id="fcf9a-134">Empieza por y distingue mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-134">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="fcf9a-135">Todos los registros que empiecen por man.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-135">All records that start with man.</span></span></TD>
  </TR>
</TABLE>

<span data-ttu-id="fcf9a-136">**Nota**: No puede usar un carácter comodín al filtrar en los campos de enumeración, como el campo **Estado** en las órdenes de venta.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-136">**Note**: You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="fcf9a-137">Para especificar un filtro para este tipo de campo, puede especificar el valor numérico como parámetro de filtrado.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-137">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="fcf9a-138">Por ejemplo, en el campo **Estado** de una orden de venta que tenga los valores **Abierto**, **Lanzado**, **Aprobación pendiente** y **Anticipo pendiente**, utilice los valores **0**, **1**, **2** y **3** para filtrar para estas opciones.</span><span class="sxs-lookup"><span data-stu-id="fcf9a-138">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fcf9a-139">Consulte también</span><span class="sxs-lookup"><span data-stu-id="fcf9a-139">See Also</span></span>
[<span data-ttu-id="fcf9a-140">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="fcf9a-140">Work with Dynamics NAV</span></span>](ui-work-product.md)

