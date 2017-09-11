---
title: "Crear numeración"
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
ms.openlocfilehash: e42e5ed139b2487fea13ef0fd57757035764addd
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="create-number-series"></a><span data-ttu-id="c078b-102">Crear numeración</span><span class="sxs-lookup"><span data-stu-id="c078b-102">Create Number Series</span></span>

<span data-ttu-id="c078b-103">Para cada empresa configurada, se necesitan asignar códigos de identificación exclusivos a elementos como cuentas de contabilidad, cuentas de proveedores y clientes, facturas y documentos.</span><span class="sxs-lookup"><span data-stu-id="c078b-103">For each company that you set up, you need to assign unique identification codes to things such as general ledger accounts, customer and vendor accounts, invoices, and documents.</span></span> <span data-ttu-id="c078b-104">La numeración es importante no sólo para la identificación.</span><span class="sxs-lookup"><span data-stu-id="c078b-104">Numbering is important not only for identification.</span></span> <span data-ttu-id="c078b-105">Un sistema de numeración bien diseñado también permite facilitar la gestión y el análisis de la empresa, y puede reducir el número de errores que se producen en la introducción de datos.</span><span class="sxs-lookup"><span data-stu-id="c078b-105">A well-designed numbering system also makes the company more manageable and easy to analyze, and can reduce the number of errors that occur in data entry.</span></span>

<span data-ttu-id="c078b-106">Puede configurar un sistema de numeración completo con un número ilimitado de números de serie.</span><span class="sxs-lookup"><span data-stu-id="c078b-106">You can set up a complete numbering system with an unlimited number of number series.</span></span> <span data-ttu-id="c078b-107">Puede utilizar números de serie para todos los tipos de documentos y diarios, así como para los datos maestros como clientes, productos y proyectos.</span><span class="sxs-lookup"><span data-stu-id="c078b-107">You can use number series for all types of documents and journals, as well as for master data such as customers, items, and jobs.</span></span>

<span data-ttu-id="c078b-108">Es posible combinar el uso de series numéricas con la numeración manual.</span><span class="sxs-lookup"><span data-stu-id="c078b-108">You can combine the use of number series with manual numbering.</span></span>

<span data-ttu-id="c078b-109">Para crear un sistema numérico, establezca uno o varios códigos para cada tipo de datos maestros o documento.</span><span class="sxs-lookup"><span data-stu-id="c078b-109">You create a numbering system by setting up one or more codes for each type of master data or document.</span></span> <span data-ttu-id="c078b-110">Por ejemplo, puede establecer un código para la numeración de clientes, otro para la numeración de facturas de venta y aún otro para la numeración de documentos en los diarios generales.</span><span class="sxs-lookup"><span data-stu-id="c078b-110">For example, you can set up one code for numbering customers, another code for numbering sales invoices, and another code for numbering documents in general journals.</span></span>

<span data-ttu-id="c078b-111">Tras establecer un código, debe establecer al menos una línea de serie numérica.</span><span class="sxs-lookup"><span data-stu-id="c078b-111">After you have set up a code, you set must set up at least one number series line.</span></span> <span data-ttu-id="c078b-112">Ésta contiene información tal como el primer y último número de la serie y la fecha de inicio.</span><span class="sxs-lookup"><span data-stu-id="c078b-112">The number series line contains information such as the first and last number in the series and the starting date.</span></span> <span data-ttu-id="c078b-113">Puede establecer más de una línea de serie numérica por código, con una fecha de inicio diferente para cada una.</span><span class="sxs-lookup"><span data-stu-id="c078b-113">You can set up more than one number series line per number series code, with a different starting date for each line.</span></span> <span data-ttu-id="c078b-114">La serie se usará de manera consecutiva, a partir de la serie de cada fecha de inicio correspondiente.</span><span class="sxs-lookup"><span data-stu-id="c078b-114">The series will be used consecutively, starting each series on the respective starting date.</span></span>

<span data-ttu-id="c078b-115">Si desea usar más de un código de serie numérica para un tipo de datos maestros, por ejemplo, usar una serie numérica diferente para categorías de productos, puede establecer relaciones de series numéricas.</span><span class="sxs-lookup"><span data-stu-id="c078b-115">If you want to use more than one number series code for one type of master data - for example, if you want to use different number series for different categories of items - you can use number series relationships.</span></span>

<span data-ttu-id="c078b-116">Además de los números que se asignan manualmente o mediante el sistema de numeración, a todas las transacciones (movimientos) se les asignan números consecutivos.</span><span class="sxs-lookup"><span data-stu-id="c078b-116">In addition to the numbers that you assign manually or by use of the numbering system, all transactions (ledger entries) are automatically assigned consecutive numbers.</span></span> <span data-ttu-id="c078b-117">Estos números se pueden ver en el campo **N.º mov.**</span><span class="sxs-lookup"><span data-stu-id="c078b-117">These numbers can be seen in the **Entry No.**</span></span> <span data-ttu-id="c078b-118">de todas las ventanas de movimiento.</span><span class="sxs-lookup"><span data-stu-id="c078b-118">field in all the ledger entry windows.</span></span> <span data-ttu-id="c078b-119">Estos números no se pueden modificar ni eliminar.</span><span class="sxs-lookup"><span data-stu-id="c078b-119">You cannot modify or delete these numbers.</span></span>

## <a name="to-create-relationships-between-number-series"></a><span data-ttu-id="c078b-120">Para crear relaciones entre números de serie</span><span class="sxs-lookup"><span data-stu-id="c078b-120">To create relationships between number series</span></span>
<span data-ttu-id="c078b-121">Si ha configurado más de un código de número de serie para el mismo tipo de información básica o transacciones, puede crear relaciones entre los códigos.</span><span class="sxs-lookup"><span data-stu-id="c078b-121">If you have set up more than one number series code for the same kind of basic information or transactions, you can create relationships between the codes.</span></span> <span data-ttu-id="c078b-122">Esta característica puede servirle de ayuda para decidir entre un código u otro cuando utilice un número.</span><span class="sxs-lookup"><span data-stu-id="c078b-122">This feature can assist you in deciding among the codes when you use a number.</span></span>

1. <span data-ttu-id="c078b-123">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Nos. serie** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="c078b-123">In the top right corner, choose the **Search for Page or Report** icon, enter **No. Series**, and then choose the related link.</span></span>
2. <span data-ttu-id="c078b-124">Seleccione la línea con las series numéricas que desea insertar para crear relaciones y, a continuación, elija **Relaciones**.</span><span class="sxs-lookup"><span data-stu-id="c078b-124">Select the line with the number series you want to create relationships for and then choose **Relationships**.</span></span>
3. <span data-ttu-id="c078b-125">En el campo **Código serie**, escriba el código del número de serie con el que desee relacionar la serie seleccionada en el paso 2.</span><span class="sxs-lookup"><span data-stu-id="c078b-125">In the **Series Code** field, enter the code for the number series that you want to relate to the series you selected in step 2.</span></span>
4. <span data-ttu-id="c078b-126">Agregue una línea para cada código que desee relacionar con el número de serie seleccionado.</span><span class="sxs-lookup"><span data-stu-id="c078b-126">Add a line for each code that you want to relate to the selected number series.</span></span>
5. <span data-ttu-id="c078b-127">Cierre la ventana.</span><span class="sxs-lookup"><span data-stu-id="c078b-127">Close the window.</span></span>

<span data-ttu-id="c078b-128">En lo sucesivo, cuando configure algo que requiera un número, podrá utilizar las relaciones que haya creado para seleccionar uno de los números de serie relacionados.</span><span class="sxs-lookup"><span data-stu-id="c078b-128">Now when you set up something that requires a number, you can use the relationships you created to select among the related number series.</span></span>

## <a name="see-also"></a><span data-ttu-id="c078b-129">Consulte también</span><span class="sxs-lookup"><span data-stu-id="c078b-129">See Also</span></span>
[<span data-ttu-id="c078b-130">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="c078b-130">Work with Dynamics NAV</span></span>](ui-work-product.md)

