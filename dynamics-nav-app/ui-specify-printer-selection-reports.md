---
title: "Especificar selección de impresora para informes"
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
ms.openlocfilehash: 56a5c1428651162293e56d71e2369fe55d291594
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---
    
# <a name="specify-printer-selection-for-reports"></a><span data-ttu-id="65a1f-102">Especificar selección de impresora para informes</span><span class="sxs-lookup"><span data-stu-id="65a1f-102">Specify Printer Selection for Reports</span></span>
<span data-ttu-id="65a1f-103">Puede configurar los informes para que se deban imprimir en una impresora específica.</span><span class="sxs-lookup"><span data-stu-id="65a1f-103">You can set up reports so that they must be printed on a specific printer.</span></span> <span data-ttu-id="65a1f-104">A continuación, se indican algunos usos de la selección de la impresora:</span><span class="sxs-lookup"><span data-stu-id="65a1f-104">The following are some uses of printer selection:</span></span> 

- <span data-ttu-id="65a1f-105">Puede imprimir informes en papel con membrete especial de la empresa.</span><span class="sxs-lookup"><span data-stu-id="65a1f-105">You can print reports on special company letterhead.</span></span>
- <span data-ttu-id="65a1f-106">Puede imprimir informes en distintos tamaños en papel.</span><span class="sxs-lookup"><span data-stu-id="65a1f-106">You can print reports on different paper sizes.</span></span>
- <span data-ttu-id="65a1f-107">Puede imprimir informes en la impresora predeterminada de un empleado especificado.</span><span class="sxs-lookup"><span data-stu-id="65a1f-107">You can print reports on the default printer of a specified employee.</span></span>

<span data-ttu-id="65a1f-108">Puede usar la ventana **Selección de impresoras** para establecer valores diferentes para obtener una salida distinta.</span><span class="sxs-lookup"><span data-stu-id="65a1f-108">You use the **Printer Selections** window to set different values to obtain different output.</span></span> <span data-ttu-id="65a1f-109">Si establece una selección de impresora específica, tendrá preferencia sobre una selección de impresora más general.</span><span class="sxs-lookup"><span data-stu-id="65a1f-109">If you set a specific printer selection, then it takes precedence over a more general printer selection.</span></span> <span data-ttu-id="65a1f-110">Por ejemplo, puede definir una selección de impresora que tenga valores en los campos **Id. usuario**, **Id. informe** y **Nombre impresora**.</span><span class="sxs-lookup"><span data-stu-id="65a1f-110">For example, you can set a printer selection that has values in the **User ID**, **Report ID**, and **Printer Name** fields.</span></span> <span data-ttu-id="65a1f-111">Esta selección de impresora tiene preferencia sobre una selección de impresora que tenga entradas en blanco en los campos **Id. usuario** o **Id. informe**.</span><span class="sxs-lookup"><span data-stu-id="65a1f-111">This printer selection takes precedence over a printer selection that has blank entries in the **User ID** or **Report ID** fields.</span></span> 

<span data-ttu-id="65a1f-112">La tabla siguiente describe la combinación de valores que especificar al configurar selecciones de impresora para un informe.</span><span class="sxs-lookup"><span data-stu-id="65a1f-112">The following table describes the combination of values to specify when you set up printer selections for a report.</span></span>

|<span data-ttu-id="65a1f-113">Para</span><span class="sxs-lookup"><span data-stu-id="65a1f-113">To</span></span>                                                 |<span data-ttu-id="65a1f-114">Establecer los valores siguientes</span><span class="sxs-lookup"><span data-stu-id="65a1f-114">Set the following values</span></span>                                             |
|---------------------------------------------------|---------------------------------------------------------------------|
|<span data-ttu-id="65a1f-115">Imprimir un informe en una impresora específica para todos los usuarios</span><span class="sxs-lookup"><span data-stu-id="65a1f-115">Print a report to a specific printer for all users</span></span> |<span data-ttu-id="65a1f-116">Especifique los valores de los campos **Id. informe** y **Nombre impresora** y deje en blanco el campo **Id. usuario**.</span><span class="sxs-lookup"><span data-stu-id="65a1f-116">Specify values in the **Report ID** and **Printer Name** fields and leave the **User ID** field blank.</span></span>|
|<span data-ttu-id="65a1f-117">Imprimir todos los informes en una impresora específica para un usuario específico</span><span class="sxs-lookup"><span data-stu-id="65a1f-117">Print all reports to a specific printer for a specific user</span></span>|<span data-ttu-id="65a1f-118">Especifique los valores de los campos **Id. usuario** y **Nombre impresora** y deje en blanco el campo **Id. informe**.</span><span class="sxs-lookup"><span data-stu-id="65a1f-118">Specify values in the **User ID** and **Printer Name** fields and leave the **Report ID** field blank.</span></span>|
|<span data-ttu-id="65a1f-119">Establecer la impresora predeterminada para todos los informes</span><span class="sxs-lookup"><span data-stu-id="65a1f-119">Set the default printer for all reports</span></span>|<span data-ttu-id="65a1f-120">Especifique un valor en el campo **Nombre impresora** y deje en blanco los campos **Id. usuario** e **Id. informe**.</span><span class="sxs-lookup"><span data-stu-id="65a1f-120">Specify a value in the **Printer Name** field and leave the **User ID** and **Report ID** fields blank.</span></span>|
|<span data-ttu-id="65a1f-121">Imprimir un informe específico en la impresora predeterminada del usuario</span><span class="sxs-lookup"><span data-stu-id="65a1f-121">Print a specific report to the user’s default printer</span></span>|<span data-ttu-id="65a1f-122">Especifique un valor en el campo **Id. informe** y deje en blanco los campos **Id. usuario** y **Nombre impresora**.</span><span class="sxs-lookup"><span data-stu-id="65a1f-122">Specify a value in the **Report ID** field and leave the **Printer Name** and **User ID** fields blank.</span></span>|
|<span data-ttu-id="65a1f-123">Imprimir un informe específico en una impresora concreta para un usuario específico</span><span class="sxs-lookup"><span data-stu-id="65a1f-123">Print a specific report to a specific printer for a specific user</span></span>|<span data-ttu-id="65a1f-124">Especifique los valores de los tres campos.</span><span class="sxs-lookup"><span data-stu-id="65a1f-124">Specify values in all three fields.</span></span>|

## <a name="see-also"></a><span data-ttu-id="65a1f-125">Consulte también</span><span class="sxs-lookup"><span data-stu-id="65a1f-125">See Also</span></span>
[<span data-ttu-id="65a1f-126">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="65a1f-126">Work with Dynamics NAV</span></span>](ui-work-product.md)

