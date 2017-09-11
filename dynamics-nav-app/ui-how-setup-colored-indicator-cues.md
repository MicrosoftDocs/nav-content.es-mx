---
title: 'Procedimiento: Configurar un indicador de color en pilas'
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
ms.openlocfilehash: 38cd904d0cf22374eac430d035e6ea6d205bcab8
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---
    
# <a name="how-to-set-up-a-colored-indicator-on-cues"></a><span data-ttu-id="09f97-102">Procedimiento: Configurar un indicador de color en pilas</span><span class="sxs-lookup"><span data-stu-id="09f97-102">How to: Set Up a Colored Indicator on Cues</span></span>
<span data-ttu-id="09f97-103">Puede configurar pilas para que aparezcan en la página **Inicio** a fin de que incluyan un indicador que cambia de color según los valores de datos de las pilas.</span><span class="sxs-lookup"><span data-stu-id="09f97-103">You can set up Cues that appear on the **Home** page to include an indicator that changes color based on the data values in the Cues.</span></span> 

<span data-ttu-id="09f97-104">El indicador se muestra como una barra de color a lo largo del borde superior del mosaico de la pila.</span><span class="sxs-lookup"><span data-stu-id="09f97-104">The indicator appears as a colored bar along the top border of the Cue tile.</span></span> <span data-ttu-id="09f97-105">Proporciona una guía visual del estado de la actividad de la pila, que puede indicar condiciones favorables o desfavorables para que el usuario actúe en consecuencia.</span><span class="sxs-lookup"><span data-stu-id="09f97-105">It provides a visual signal of the status of the Cue's activity, which can indicate favorable or unfavorable conditions to prompt the user to take action.</span></span> <span data-ttu-id="09f97-106">Por ejemplo, si una pila muestra las facturas de venta en curso, puede configurar que el indicador aparezca de color verde (favorable) si el número total de facturas de venta en curso es inferior a 10 y que aparezca de color rojo (desfavorable) si el total es mayor que 20.</span><span class="sxs-lookup"><span data-stu-id="09f97-106">For example, if a Cue displays ongoing sales invoices, you can set up the indicator to appear green (favorable) when total number of ongoing sales invoices is below 10, and appears red (unfavorable) when the total is greater than 20.</span></span>

<span data-ttu-id="09f97-107">En la ventana **Configuración de pila** se configuran indicadores para todas las pilas que están disponibles en la base de datos de la empresa.</span><span class="sxs-lookup"><span data-stu-id="09f97-107">From the **Cue Setup** window, you set up indicators for all the Cues that are available in the company database.</span></span>

<span data-ttu-id="09f97-108">Para configurar el indicador, especifique hasta dos valores de umbral que definan tres rangos de valores de datos (bajo, medio y alto) a los que se pueda aplicar otro color (o estilo).</span><span class="sxs-lookup"><span data-stu-id="09f97-108">To set up the indicator, you specify up to two threshold values that define three ranges of data values (low, middle, and high) to which you can apply a different color (or style).</span></span>

## <a name="to-set-up-colored-indicators-on-cues"></a><span data-ttu-id="09f97-109">Para configurar indicadores de color en las pilas</span><span class="sxs-lookup"><span data-stu-id="09f97-109">To set up colored indicators on Cues</span></span>
1. <span data-ttu-id="09f97-110">En **Actividades** en la página **Inicio**, elija **Configurar pilas**.</span><span class="sxs-lookup"><span data-stu-id="09f97-110">Under **Activities** on your **Home** page, choose **Set Up Cues**.</span></span>  
<span data-ttu-id="09f97-111">Aparece la ventana **Configuración de pila**.</span><span class="sxs-lookup"><span data-stu-id="09f97-111">The **Cue Setup** window appears.</span></span> <span data-ttu-id="09f97-112">La ventana muestra los indicadores que están actualmente configurados en pilas.</span><span class="sxs-lookup"><span data-stu-id="09f97-112">The window lists the indicators that are currently setup up on Cues.</span></span>
2. <span data-ttu-id="09f97-113">Para modificar un marcador, edite los campos y modifique, por ejemplo, los valores para los distintos umbrales.</span><span class="sxs-lookup"><span data-stu-id="09f97-113">To modify an indicator, edit the fields and modify, for example, the values for the different thresholds.</span></span>  

<span data-ttu-id="09f97-114">La tabla siguiente muestra los colores que corresponden a las opciones de los campos **Estilo de rango bajo**, **Estilo de rango medio** y **Estilo de rango alto**.</span><span class="sxs-lookup"><span data-stu-id="09f97-114">The following table lists the colors that correspond to the options of the **Low Range Style**, **Middle Range Style**, and **High Range Style** fields.</span></span>

|<span data-ttu-id="09f97-115">Opción</span><span class="sxs-lookup"><span data-stu-id="09f97-115">Option</span></span>|<span data-ttu-id="09f97-116">Color</span><span class="sxs-lookup"><span data-stu-id="09f97-116">Color</span></span>|
|------|-----|
|<span data-ttu-id="09f97-117">**Ninguno**</span><span class="sxs-lookup"><span data-stu-id="09f97-117">**None**</span></span>|<span data-ttu-id="09f97-118">Sin color (mismo color que el mosaico de la pila)</span><span class="sxs-lookup"><span data-stu-id="09f97-118">No color (same color as the Cue tile</span></span>|
|<span data-ttu-id="09f97-119">**Favorable**</span><span class="sxs-lookup"><span data-stu-id="09f97-119">**Favorable**</span></span>|<span data-ttu-id="09f97-120">Verde</span><span class="sxs-lookup"><span data-stu-id="09f97-120">Green</span></span>|
|<span data-ttu-id="09f97-121">**Desfavorable**</span><span class="sxs-lookup"><span data-stu-id="09f97-121">**Unfavorable**</span></span>|<span data-ttu-id="09f97-122">Rojo</span><span class="sxs-lookup"><span data-stu-id="09f97-122">Red</span></span>|
|<span data-ttu-id="09f97-123">**Ambiguo**</span><span class="sxs-lookup"><span data-stu-id="09f97-123">**Ambiguous**</span></span>|<span data-ttu-id="09f97-124">Amarillo</span><span class="sxs-lookup"><span data-stu-id="09f97-124">Yellow</span></span>|
|<span data-ttu-id="09f97-125">**Subordinado**</span><span class="sxs-lookup"><span data-stu-id="09f97-125">**Subordinate**</span></span>|<span data-ttu-id="09f97-126">Gris</span><span class="sxs-lookup"><span data-stu-id="09f97-126">Gray</span></span>|

## <a name="see-also"></a><span data-ttu-id="09f97-127">Consulte también</span><span class="sxs-lookup"><span data-stu-id="09f97-127">See Also</span></span>
[<span data-ttu-id="09f97-128">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="09f97-128">Work with Dynamics NAV</span></span>](ui-work-product.md)


