---
title: Analizar real frente a presupuesto
description: "Describe cómo analizar los importes reales frente a los importes presupuestados."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: bi, power BI, analysis, KPI
ms.date: 06/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: da2cdce3ada29fff98ceb875414f750a8af51855
ms.contentlocale: es-mx
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-analyze-actual-amounts-versus-budgeted-amounts"></a><span data-ttu-id="e7fb7-103">Analizar los importes reales frente a los importes presupuestados</span><span class="sxs-lookup"><span data-stu-id="e7fb7-103">How to: Analyze Actual Amounts Versus Budgeted Amounts</span></span>
<span data-ttu-id="e7fb7-104">Como parte de la recopilación, el análisis y el uso compartido de los datos de la empresa, puede ver importes reales comparados con los importes presupuestados para todas las cuentas y durante varios periodos.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-104">As a part of gathering, analyzing, and sharing your company data, you view actual amounts compared to budgeted amounts for all accounts and for several periods.</span></span>

<span data-ttu-id="e7fb7-105">Para analizar los importes presupuestados, primero debe crear presupuestos.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-105">To analyze budgeted amounts, you must first create budgets.</span></span> <span data-ttu-id="e7fb7-106">Para obtener más información, consulte [Crear presupuestos](finance-how-create-budgets.md).</span><span class="sxs-lookup"><span data-stu-id="e7fb7-106">For more information, see [How to: Create Budgets](finance-how-create-budgets.md).</span></span>

## <a name="to-view-a-budget"></a><span data-ttu-id="e7fb7-107">Para ver un presupuesto</span><span class="sxs-lookup"><span data-stu-id="e7fb7-107">To view a budget</span></span>
<span data-ttu-id="e7fb7-108">En un presupuesto con dimensiones, puede filtrar los movimientos y, por lo tanto, ver presupuestos concretos.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-108">In a budget with dimensions, you can filter the entries and see specific budgets.</span></span>

1. <span data-ttu-id="e7fb7-109">Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Presupuestos contables** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **G/L Budgets**, and then choose the related link.</span></span>
2. <span data-ttu-id="e7fb7-110">En la ventana **Presupuestos contables**, abra el presupuesto que desee ver.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-110">In the **G/L Budgets** window, open the budget that you want to view.</span></span>  
3. <span data-ttu-id="e7fb7-111">En la parte superior de la ventana rellene los campos según sea necesario para definir lo que se muestra.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-111">At the top of the window, fill in the fields as necessary to define what is shown.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   <span data-ttu-id="e7fb7-112">Si ha seleccionado **Periodo** en el campo **Muestra como líneas** o **Muestra como columnas**, debe rellenar el campo **Ver por**.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-112">If you have selected **Period** in either the **Show as Lines** or the **Show as Columns** field, then you must fill in the **View by** field.</span></span> <span data-ttu-id="e7fb7-113">Si no ha seleccionado **Periodo** en el campo **Muestra como líneas** o **Muestra como columnas**, escriba el periodo apropiado en el campo **Filtro fecha**.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-113">If you have not selected **Period** in either the **Show as Lines** or **Show as Columns** field, then enter the appropriate period in **Date Filter** field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="e7fb7-114">Sólo se incluyen en el cálculo los movimientos del presupuesto que incluyan los códigos de filtro que haya introducido en la ficha desplegable **Filtros**.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-114">Only entries from the general ledger budget with the filter codes that you enter on the **Filters** FastTab are included in the calculation.</span></span> <span data-ttu-id="e7fb7-115">No se incluirán los movimientos de presupuesto que tengan otros códigos de filtro o que no tengan ninguno.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-115">Budget entries with other filter codes or without any filter codes are not included.</span></span> <span data-ttu-id="e7fb7-116">Mientras el filtro aparezca en la ventana, el presupuesto sólo mostrará los movimientos de presupuesto con dichos códigos de filtro.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-116">As long as the filter remains on the window, the budget only displays the budget entries with these filter codes.</span></span>  

> [!TIP]  
>   <span data-ttu-id="e7fb7-117">Si tiene que modificar el presupuesto, puede editar sus movimientos.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-117">If you want to modify the budget, you can modify the budget entries.</span></span> <span data-ttu-id="e7fb7-118">Elija un importe para ver los movimientos de contabilidad subyacentes.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-118">Choose an amount to view the underlying general ledger budget entries.</span></span>

## <a name="to-view-actual-and-budgeted-amounts-for-all-accounts"></a><span data-ttu-id="e7fb7-119">Para ver los importes reales y presupuestados de todas las cuentas</span><span class="sxs-lookup"><span data-stu-id="e7fb7-119">To view actual and budgeted amounts for all accounts</span></span>  
<span data-ttu-id="e7fb7-120">Puede ver presupuestos y compararlos con las cifras reales de varias áreas de [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e7fb7-120">You can view general ledger budgets and compare them with actual figures in several areas of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

1. <span data-ttu-id="e7fb7-121">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plan de cuentas** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-121">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7fb7-122">En la ventana **Plan de cuentas**, seleccione la acción **Saldo/Ppto. cuenta**.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-122">In the **Chart of Accounts** window, choose the **G/L Balance/Budget** action.</span></span>
3. <span data-ttu-id="e7fb7-123">En la parte superior de la ventana rellene los campos según sea necesario para definir lo que se muestra.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-123">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>  
4. <span data-ttu-id="e7fb7-124">Para ver una especificación que compone un importe que aparece en pantalla, elija el campo.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-124">To see a specification that makes up the amount shown, choose the field.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="e7fb7-125">Los filtros que establezca en la cabecera de ventana se aplicarán a los movimientos de contabilidad y a los movimientos de presupuesto.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-125">The filters you set in the window header will be applied to general ledger entries and also budget entries.</span></span>

<span data-ttu-id="e7fb7-126">Las columnas de la izquierda contienen el Catálogo de cuentas.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-126">The leftmost columns contain the chart of accounts.</span></span> <span data-ttu-id="e7fb7-127">De las cinco columnas de la derecha, las primeras cuatro muestran los importes del Debe y el Haber reales y presupuestados de cada cuenta.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-127">Of the five columns on the rightmost side, the first four columns show actual and budgeted debit and credit amounts for each account.</span></span> <span data-ttu-id="e7fb7-128">La quinta columna muestra las relaciones proporcionales entre los importes reales y presupuestados de la cuenta.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-128">The fifth column shows the proportional relationship between the actual and the budgeted amounts on the general ledger account.</span></span>  

> [!TIP]  
>   <span data-ttu-id="e7fb7-129">Utilice el campo **Ver por** en la ventana **Saldo/Ppto. cuenta** seleccionar la longitud del periodo.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-129">Use the **View by** field in the **G/L Balance/Budget** window to select the period length.</span></span> <span data-ttu-id="e7fb7-130">Utilice el campo **Ver como** para seleccionar el modo de cálculo de los importes **Saldo periodo** o **Saldo a la fecha**.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-130">Use the **View as** field to select the way the amounts will be calculated, **Net Change** or **Balance at Date**.</span></span> <span data-ttu-id="e7fb7-131">Elija la acción **Periodo anterior** o **Periodo siguiente** para cambiar el periodo.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-131">Choose the **Previous Period** or **Next Period** action to change the period.</span></span>  

## <a name="to-view-actual-and-budgeted-amounts-for-several-periods"></a><span data-ttu-id="e7fb7-132">Para ver los importes reales y presupuestados de varios periodos</span><span class="sxs-lookup"><span data-stu-id="e7fb7-132">To view actual and budgeted amounts for several periods</span></span>  
<span data-ttu-id="e7fb7-133">En lugar de ver los importes reales y presupuestados de todas las cuentas en un único periodo, puede ver varios periodos de una cuenta.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-133">Instead of viewing the actual and budgeted amounts for all accounts within a single period, you can view a number of periods for a single account.</span></span>  

1. <span data-ttu-id="e7fb7-134">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Plan de cuentas** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-134">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="e7fb7-135">En la ventana **Plan de cuentas**, seleccione la cuenta contable relevante y, después, seleccione la acción **Saldo cuenta/Presupuesto**.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-135">In the **Chart of Accounts** window, select the relevant general ledger account, and then choose the **G/L Account Balance/Budget** action.</span></span>  
3. <span data-ttu-id="e7fb7-136">En la parte superior de la ventana rellene los campos según sea necesario para definir lo que se muestra.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-136">At the top of the window, fill in the fields as necessary to define what is shown.</span></span>   
4. <span data-ttu-id="e7fb7-137">Para ver una especificación de un importe que aparece en pantalla, elija el campo.</span><span class="sxs-lookup"><span data-stu-id="e7fb7-137">To see a specification of an amount shown, choose the field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e7fb7-138">Consulte también</span><span class="sxs-lookup"><span data-stu-id="e7fb7-138">See Also</span></span>
<span data-ttu-id="e7fb7-139">[Inteligencia empresarial](bi.md)
[Trabajar con esquemas de cuentas](bi-how-work-account-schedule.md)</span><span class="sxs-lookup"><span data-stu-id="e7fb7-139">[Business Intelligence](bi.md)
[How to: Work with Account Schedules](bi-how-work-account-schedule.md)</span></span>  
[<span data-ttu-id="e7fb7-140">Finanzas</span><span class="sxs-lookup"><span data-stu-id="e7fb7-140">Finance</span></span>](finance.md)  
[<span data-ttu-id="e7fb7-141">Configurar las finanzas</span><span class="sxs-lookup"><span data-stu-id="e7fb7-141">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="e7fb7-142">Libro mayor y plan de cuentas</span><span class="sxs-lookup"><span data-stu-id="e7fb7-142">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
<span data-ttu-id="e7fb7-143">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e7fb7-143">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

