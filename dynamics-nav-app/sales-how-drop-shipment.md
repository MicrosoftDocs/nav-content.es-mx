---
title: "Procedimiento: Realizar envíos directos"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: a726c8c24d8f843b33b4df4d85ad2b5eab3790e7
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-make-drop-shipments"></a><span data-ttu-id="46d57-102">Procedimiento: Realizar envíos directos</span><span class="sxs-lookup"><span data-stu-id="46d57-102">How to: Make Drop Shipments</span></span>
<span data-ttu-id="46d57-103">Una remisión directa es la remisión de los productos de uno de sus proveedores directamente a uno de sus clientes.</span><span class="sxs-lookup"><span data-stu-id="46d57-103">A drop shipment is the shipment of items from one of your vendors directly to one of your customers.</span></span>

<span data-ttu-id="46d57-104">Cuando marca una orden de venta para envío directo y crea una orden especificando el cliente en el campo **Venta a-N.º cliente**.</span><span class="sxs-lookup"><span data-stu-id="46d57-104">When a sales order is marked for drop shipment, and you create a purchase order specifying the customer in the **Sell-to Customer No.**</span></span> <span data-ttu-id="46d57-105">puede vincular los dos documentos y así asignar instrucciones al proveedor para que envíe el producto directamente al cliente.</span><span class="sxs-lookup"><span data-stu-id="46d57-105">field, then you can link the two documents and thereby instruct the vendor to ship directly to the customer.</span></span>

## <a name="to-create-a-sales-order-for-drop-shipment"></a><span data-ttu-id="46d57-106">Para crear una orden de venta de remisión directa</span><span class="sxs-lookup"><span data-stu-id="46d57-106">To create a sales order for drop shipment</span></span>
<span data-ttu-id="46d57-107">Para preparar una remisión directa, cree una orden de venta como si fuese normal, pero indique en la línea de ventas que dicha venta requiere una remisión directa.</span><span class="sxs-lookup"><span data-stu-id="46d57-107">To prepare a drop shipment, you create a sales order for an item as normal, except you must indicate on the sales line that the sale requires drop shipment.</span></span>

1. <span data-ttu-id="46d57-108">Cree una orden de venta para un artículo.</span><span class="sxs-lookup"><span data-stu-id="46d57-108">Create a sales order for an item.</span></span> <span data-ttu-id="46d57-109">Para obtener más información, vea [Procedimiento: Vender productos](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="46d57-109">For more information, see [How to: Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="46d57-110">En la línea de la orden de venta del artículo con envío directo, seleccione la casilla **Envío directo**.</span><span class="sxs-lookup"><span data-stu-id="46d57-110">On the sales order line for the drop-shipment item, select the **Drop Shipment** check box.</span></span>

## <a name="to-create-the-purchase-order-for-drop-shipment"></a><span data-ttu-id="46d57-111">Para crear órdenes de compra de remisión directa</span><span class="sxs-lookup"><span data-stu-id="46d57-111">To create the purchase order for drop shipment</span></span>
<span data-ttu-id="46d57-112">Para preparar una remisión directa de un producto que se va a vender, cree una orden de compra como si fuese normal, pero indique en dicha orden que el producto debe enviarse directamente al cliente no a usted.</span><span class="sxs-lookup"><span data-stu-id="46d57-112">To prepare a drop shipment for the item to be sold, you create a purchase order as normal, except you must indicate on the purchase order that it must be shipped to your customer, not to yourself.</span></span>

1. <span data-ttu-id="46d57-113">Cree una orden de compra.</span><span class="sxs-lookup"><span data-stu-id="46d57-113">Create a purchase order.</span></span> <span data-ttu-id="46d57-114">No rellene ningún campo en las líneas.</span><span class="sxs-lookup"><span data-stu-id="46d57-114">Do not fill any fields on the lines.</span></span> <span data-ttu-id="46d57-115">Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="46d57-115">For more information, see [How to: Record Purchases](purchasing-how-record-purchases.md).</span></span>
2. <span data-ttu-id="46d57-116">En el campo **Venta a-N.º cliente**,</span><span class="sxs-lookup"><span data-stu-id="46d57-116">In the **Sell-to Customer No.**</span></span> <span data-ttu-id="46d57-117">seleccione el cliente al que le está vendiendo.</span><span class="sxs-lookup"><span data-stu-id="46d57-117">field, select the customer that you are selling to.</span></span>
3. <span data-ttu-id="46d57-118">Elija la acción **Envíos directos** y, a continuación, **Tomar orden venta**.</span><span class="sxs-lookup"><span data-stu-id="46d57-118">Choose the **Drop Shipments** action, and then choose the **Get Sales Order** action.</span></span>
4. <span data-ttu-id="46d57-119">En la ventana **Lista ventas**, seleccione la orden de venta que ha preparado en la sección "Para crear una orden de venta de envío directo".</span><span class="sxs-lookup"><span data-stu-id="46d57-119">In the **Sales List** window, select the sales order that you prepared in the "To create a sales order for drop shipment" section.</span></span>
5. <span data-ttu-id="46d57-120">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="46d57-120">Choose the **OK** button.</span></span>

<span data-ttu-id="46d57-121">La información de la línea de la orden de venta se inserta en las líneas de la orden de compra.</span><span class="sxs-lookup"><span data-stu-id="46d57-121">The line information from the sales order is inserted on the purchase order line(s).</span></span>

<span data-ttu-id="46d57-122">Ahora puede asignar instrucciones al proveedor para que envíe los productos al cliente, por ejemplo, enviando la orden de compra por correo electrónico en formato PDF.</span><span class="sxs-lookup"><span data-stu-id="46d57-122">You can now instruct the vendor to ship the items to your customer, for example, by mailing the purchase order as a PDF.</span></span>     

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a><span data-ttu-id="46d57-123">Para ver la orden de compra vinculada a la orden de venta</span><span class="sxs-lookup"><span data-stu-id="46d57-123">To view the linked purchase order from the sales order</span></span>
1. <span data-ttu-id="46d57-124">Seleccione la línea de la orden de compra de envío directo, elija las acciones **Orden**, **Envío directo** y, a continuación, **Orden de compra**.</span><span class="sxs-lookup"><span data-stu-id="46d57-124">Select the drop-shipment sales order line, choose the **Order** action, choose the **Drop Shipment** action, and then choose the **Purchase Order** action.</span></span>

<span data-ttu-id="46d57-125">Se abre la orden de compra vinculada.</span><span class="sxs-lookup"><span data-stu-id="46d57-125">The linked purchase order opens.</span></span>

## <a name="to-post-a-drop-shipment"></a><span data-ttu-id="46d57-126">Para registrar una remisión directa</span><span class="sxs-lookup"><span data-stu-id="46d57-126">To post a drop shipment</span></span>
<span data-ttu-id="46d57-127">Cuando el proveedor ha enviado los artículos, puede establecer las órdenes de venta como enviadas.</span><span class="sxs-lookup"><span data-stu-id="46d57-127">When the vendor has shipped the items, you can post the sales order as shipped.</span></span> <span data-ttu-id="46d57-128">También puede registrar la orden de compra, pero solo con la opción **Recibir** hasta que se haya facturado la orden de venta.</span><span class="sxs-lookup"><span data-stu-id="46d57-128">You can also post the purchase order, but only with the **Receive** option until the sales order has been invoiced.</span></span>
1. <span data-ttu-id="46d57-129">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Órdenes de venta** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="46d57-129">In the top right corner, choose the **Search for Page or Report** icon, enter **Sales orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="46d57-130">Abra la orden de venta que ha creado en la sección "Para crear una orden de venta de remisión directa".</span><span class="sxs-lookup"><span data-stu-id="46d57-130">Open the sales order that you created in the "To create a sales order for a drop shipment" section.</span></span>
3. <span data-ttu-id="46d57-131">En el campo **Cantidad a enviar**, especifiqué qué cantidad de la orden debe enviarse, todo o solo una parte.</span><span class="sxs-lookup"><span data-stu-id="46d57-131">In the **Qty. to Ship** field, specify how many of the order quantity to ship, the full or a partial order quantity.</span></span>
3. <span data-ttu-id="46d57-132">Seleccione la acción **Registrar** o **Registrar y enviar**.</span><span class="sxs-lookup"><span data-stu-id="46d57-132">Choose the **Post** or **Post and Send** action.</span></span>
4. <span data-ttu-id="46d57-133">Elija la opción **Enviar** para facturar más adelante o la opción **Enviar y facturar** para facturar ahora.</span><span class="sxs-lookup"><span data-stu-id="46d57-133">Choose either the **Ship** option to invoice later, or the **Ship and Invoice** option to invoice immediately.</span></span>

## <a name="see-also"></a><span data-ttu-id="46d57-134">Consulte también</span><span class="sxs-lookup"><span data-stu-id="46d57-134">See Also</span></span>
<span data-ttu-id="46d57-135">[Vender productos](sales-how-sell-products.md)  </span><span class="sxs-lookup"><span data-stu-id="46d57-135">[How to: Sell Products](sales-how-sell-products.md)  </span></span>  
[<span data-ttu-id="46d57-136">Registro de compras</span><span class="sxs-lookup"><span data-stu-id="46d57-136">How to: Record Purchases</span></span>](purchasing-how-record-purchases.md)  
[<span data-ttu-id="46d57-137">Gestionar ventas</span><span class="sxs-lookup"><span data-stu-id="46d57-137">Manage Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="46d57-138">[Gestionar inventario](inventory-manage-inventory.md)    </span><span class="sxs-lookup"><span data-stu-id="46d57-138">[Manage Inventory](inventory-manage-inventory.md)    </span></span>  
[<span data-ttu-id="46d57-139">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="46d57-139">Work with Dynamics NAV</span></span>](ui-work-product.md)

