---
title: Gestionar inventario
author: SorenGP
ms.custom: na
ms.date: 11/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 4e1d7f9a8e2c22ab19a8b7a5fbf57bd0509a9b4a
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="manage-inventory"></a><span data-ttu-id="f6442-102">Gestionar inventario</span><span class="sxs-lookup"><span data-stu-id="f6442-102">Manage Inventory</span></span>
<span data-ttu-id="f6442-103">Por cada producto físico que se comercialice de debe crear una ficha de producto del tipo Inventario.</span><span class="sxs-lookup"><span data-stu-id="f6442-103">For each physical product that you trade in you must create an item card of type Inventory.</span></span> <span data-ttu-id="f6442-104">Los productos que ofrece a los clientes pero que no mantiene en el inventario, puede registrarlos como productos no inventariables, y puede convertirlos a productos de inventario cuando sea necesario.</span><span class="sxs-lookup"><span data-stu-id="f6442-104">Items that you offer to customers but do not keep in inventory you can register as nonstock items, which you can convert to inventory items when necessary.</span></span> <span data-ttu-id="f6442-105">Puede aumentar o reducir la cantidad de un producto en el inventario registrándolo directamente desde los movimientos de producto, por ejemplo, después de un recuento físico o si no registra compras.</span><span class="sxs-lookup"><span data-stu-id="f6442-105">You can increase or decrease the quantity of an item in inventory by posting directly to the item ledger entries, for example, after a physical count or if you do not record purchases.</span></span>

<span data-ttu-id="f6442-106">Los aumentos y las disminuciones de inventario también se registran cuando registra documentos de compra y de ventas respectivamente.</span><span class="sxs-lookup"><span data-stu-id="f6442-106">Inventory increases and decreases are naturally also recorded when you post purchase and sales documents respectively.</span></span> <span data-ttu-id="f6442-107">Para obtener más información, vea [Procedimiento: Registrar](purchasing-how-record-purchases.md), [Procedimiento: Vender productos](sales-how-sell-products.md) y [Procedimiento: Facturar ventas](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="f6442-107">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md), [How to: Sell Products](sales-how-sell-products.md), and [How to: Invoice Sales](sales-how-invoice-sales.md).</span></span>

<span data-ttu-id="f6442-108">Para aumentar la información general de los productos y ayudarle a encontrarlos, puede clasificar los productos y darles atributos para que los pueda ordenar y buscar.</span><span class="sxs-lookup"><span data-stu-id="f6442-108">To increase your overview of items and to help you find them, you can categorize items and give them attributes to search and sort by.</span></span>   

<span data-ttu-id="f6442-109">**Nota**: En Dynamics NAV, se usa el término "producto" para denominar los artículos.</span><span class="sxs-lookup"><span data-stu-id="f6442-109">**Note**: In Dynamics NAV, a product is referred to using the term “item”.</span></span>

|<span data-ttu-id="f6442-110">Para</span><span class="sxs-lookup"><span data-stu-id="f6442-110">To</span></span> |<span data-ttu-id="f6442-111">Vea</span><span class="sxs-lookup"><span data-stu-id="f6442-111">See</span></span> |
|---|----|
|<span data-ttu-id="f6442-112">Crear fichas de producto para los productos de inventario que comercialice.</span><span class="sxs-lookup"><span data-stu-id="f6442-112">Create item cards for inventory item that you trade in.</span></span>|[<span data-ttu-id="f6442-113">Registro de productos nuevos</span><span class="sxs-lookup"><span data-stu-id="f6442-113">How to: Register New Products</span></span>](inventory-how-register-new-products.md)|
|<span data-ttu-id="f6442-114">Mantener una visión general de los productos y ayudarle a buscarlos y clasificarlos al organizarlos en categorías.</span><span class="sxs-lookup"><span data-stu-id="f6442-114">Maintain an overview of items and help you find and sort items by organizing them in categories.</span></span>|[<span data-ttu-id="f6442-115">Clasificar productos</span><span class="sxs-lookup"><span data-stu-id="f6442-115">How to: Categorize Items</span></span>](inventory-how-categorize-items.md)|  
|<span data-ttu-id="f6442-116">Asignar atributos de producto de distintos tipos de valor a sus productos le ayudará a ordenarlos y encontrarlos.</span><span class="sxs-lookup"><span data-stu-id="f6442-116">Assign item attributes of different value types to your items to help you sort and find items.</span></span>|[<span data-ttu-id="f6442-117">Trabajar con atributos de producto</span><span class="sxs-lookup"><span data-stu-id="f6442-117">How to: Work with Item Attributes</span></span>](inventory-how-work-item-attributes.md)|
|<span data-ttu-id="f6442-118">Crear fichas especiales para los productos que desea ofrecer a los clientes, pero que no desea mantener en el inventario.</span><span class="sxs-lookup"><span data-stu-id="f6442-118">Create special item cards for items that you offer to customers but do not maintain inventory for.</span></span>|[<span data-ttu-id="f6442-119">Procedimiento: Trabajar con productos sin stock</span><span class="sxs-lookup"><span data-stu-id="f6442-119">How to: Work with Nonstock Items</span></span>](inventory-how-work-nonstock-items.md)|
|<span data-ttu-id="f6442-120">Apreciar o amortizar el valor de uno o más productos del inventario registrando el valor calculado actual.</span><span class="sxs-lookup"><span data-stu-id="f6442-120">Appreciate or depreciate the value of one or more items in inventory by posting their current, calculated value.</span></span>|[<span data-ttu-id="f6442-121">Revaluación de inventario</span><span class="sxs-lookup"><span data-stu-id="f6442-121">How to: Revalue Inventory</span></span>](inventory-how-revalue-inventory.md)|
|<span data-ttu-id="f6442-122">Ajuste los costos de productos, automática o manualmente, para desviar los cambios de costo de los movimientos de entrada a sus movimientos de salida relacionados.</span><span class="sxs-lookup"><span data-stu-id="f6442-122">Adjust item costs, either automatically or manually, to forward cost changes from inbound entries to their related outbound entries.</span></span>|[<span data-ttu-id="f6442-123">Procedimiento: Ajustar precios de productos</span><span class="sxs-lookup"><span data-stu-id="f6442-123">How to: Adjust Item Costs</span></span>](inventory-how-adjust-item-costs.md)|
|<span data-ttu-id="f6442-124">Refleje los cambios en los valores de inventario en sus libros de la empresa registrando costos de inventario, ya sea automática o manualmente, en las cuentas de inventario relacionadas del libro mayor.</span><span class="sxs-lookup"><span data-stu-id="f6442-124">Reflect inventory value changes in your company books by posting inventory costs, either automatically or manually, to the related inventory accounts in the general ledger.</span></span>|[<span data-ttu-id="f6442-125">Cómo registrar costes de inventario en la contabilidad general</span><span class="sxs-lookup"><span data-stu-id="f6442-125">How to: Post Inventory Costs to the General Ledger</span></span>](inventory-how-post-inventory-cost-gl.md)|

## <a name="see-also"></a><span data-ttu-id="f6442-126">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f6442-126">See Also</span></span>  
[<span data-ttu-id="f6442-127">Gestionar compras</span><span class="sxs-lookup"><span data-stu-id="f6442-127">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="f6442-128">Gestionar ventas</span><span class="sxs-lookup"><span data-stu-id="f6442-128">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="f6442-129">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="f6442-129">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="f6442-130">Con varias áreas de negocio</span><span class="sxs-lookup"><span data-stu-id="f6442-130">Across Business Areas</span></span>](ui-across-business-areas.md)

