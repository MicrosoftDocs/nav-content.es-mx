---
title: Transferir productos entre almacenes
description: "Describe cómo mover el inventario de un lugar o almacén a otro con el diario de reclasificación o con pedidos de transferencia."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: move, warehouse
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: HT
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 06f7b6d5efdd895383be8bbed82a3e9f5f8e071e
ms.contentlocale: es-mx
ms.lasthandoff: 12/01/2017

---
# <a name="how-to-transfer-inventory-between-locations"></a><span data-ttu-id="44734-103">Procedimiento: Transferir el inventario entre almacenes</span><span class="sxs-lookup"><span data-stu-id="44734-103">How to: Transfer Inventory Between Locations</span></span>
<span data-ttu-id="44734-104">Puede transferir inventarios de productos entre almacenes creando pedidos de transferencia.</span><span class="sxs-lookup"><span data-stu-id="44734-104">You can transfer inventory items between locations by creating transfer orders.</span></span> <span data-ttu-id="44734-105">También puede usar el diario de reclasificación de productos.</span><span class="sxs-lookup"><span data-stu-id="44734-105">Alternatively, you can use the item reclassification journal.</span></span>

<span data-ttu-id="44734-106">Con los pedidos de transferencia, se envía la transferencia de salida desde un almacén y se recibe la transferencia de entrada en el otro almacén.</span><span class="sxs-lookup"><span data-stu-id="44734-106">With transfer orders, you ship the outbound transfer from one location and receive the inbound transfer at the other location.</span></span> <span data-ttu-id="44734-107">Esto permite administrar las actividades de almacén correspondientes y proporciona más certidumbre de que las cantidades del inventario se actualizan correctamente.</span><span class="sxs-lookup"><span data-stu-id="44734-107">This allows you to manage the involved warehouse activities and provides more certainty that inventory quantities are updated correctly.</span></span>

<span data-ttu-id="44734-108">Cono el diario de reclasificación, simplemente se rellenan los campos **Código de almacén** y **Nuevo código de almacén**.</span><span class="sxs-lookup"><span data-stu-id="44734-108">With the reclassification journal, you simply fill in the **Location Code** and the **New Location Code** fields.</span></span> <span data-ttu-id="44734-109">Al registrar el diario, los movimientos de productos se ajustan en los almacenes en cuestión.</span><span class="sxs-lookup"><span data-stu-id="44734-109">When you post the journal, the item ledger entries are adjusted at the locations in question.</span></span> <span data-ttu-id="44734-110">Con este método, las actividades de almacén no se administran.</span><span class="sxs-lookup"><span data-stu-id="44734-110">With this method, warehouse activities are not managed.</span></span>

> [!NOTE]  
>   <span data-ttu-id="44734-111">Si tiene productos registrados en el inventario sin un código de almacén, por ejemplo cuando solo tenía un almacén, no podrá transferir estos productos con pedidos de transferencia.</span><span class="sxs-lookup"><span data-stu-id="44734-111">If you have items recorded in your inventory without a location code, for example from a time when you only had one warehouse, then you cannot transfer those items using transfer orders.</span></span> <span data-ttu-id="44734-112">En su lugar, deberá utilizar el diario de reclasificación para reclasificar los productos desde un código de almacén en blanco a un código de almacén real.</span><span class="sxs-lookup"><span data-stu-id="44734-112">Instead, you must use the reclassification journal to reclassify the items from a blank location code to an actual location code.</span></span>  <span data-ttu-id="44734-113">Para obtener más información, vea el paso 3 en la sección "Para transferir productos con el diario de reclasificación".</span><span class="sxs-lookup"><span data-stu-id="44734-113">For more information, see step 3 in the "To transfer items with the item reclassification journal" section.</span></span>

<span data-ttu-id="44734-114">Para transferir productos, se deben configurar las ubicaciones y las rutas de transferencia.</span><span class="sxs-lookup"><span data-stu-id="44734-114">To transfer items, locations and transfer routes must be set up.</span></span> <span data-ttu-id="44734-115">Para obtener más información, vea [Procedimiento: Configurar almacenes](inventory-how-setup-locations.md).</span><span class="sxs-lookup"><span data-stu-id="44734-115">For more information, see [How to: Set Up Locations](inventory-how-setup-locations.md).</span></span>

## <a name="to-transfer-items-with-a-transfer-order"></a><span data-ttu-id="44734-116">Para transferir productos con un pedido de transferencia</span><span class="sxs-lookup"><span data-stu-id="44734-116">To transfer items with a transfer order</span></span>
1. <span data-ttu-id="44734-117">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de transferencia** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="44734-117">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="44734-118">En la ventana **Pedido de transferencia**, rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="44734-118">In the **Transfer Order** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
>   <span data-ttu-id="44734-119">Si ha rellenado los campos **Cód. en tránsito**, **Cód. transportista** y **Cód. servicio transportista** en la ventana **Ruta transf. espec.** cuando configuró la ruta de transferencia, los campos correspondientes del pedido de transferencia se rellenan automáticamente.</span><span class="sxs-lookup"><span data-stu-id="44734-119">If you have filled in the **In-Transit Code**, **Shipping Agent Code**, and **Shipping Agent Service** fields in the **Trans. Route Spec.** window when you set up the transfer route, then the corresponding fields on the transfer order are filled in automatically.</span></span>

    <span data-ttu-id="44734-120">Cuando se especifica un valor en el campo **Servicio transportista**, se calcula la fecha de recepción en el almacén de destino de la transferencia, sumando el tiempo de envío del transportista a la fecha de envío.</span><span class="sxs-lookup"><span data-stu-id="44734-120">When you fill in the **Shipping Agent Service** field, the receipt date at the transfer-to location is calculated by adding the shipping time of the shipping agent service to the shipment date.</span></span>

    <span data-ttu-id="44734-121">Como trabajador de almacén en el almacén de procedencia de la transferencia, continúe con el envío de los productos.</span><span class="sxs-lookup"><span data-stu-id="44734-121">As a warehouse worker at the transfer-from location, proceed to ship the items.</span></span>
3. <span data-ttu-id="44734-122">Seleccione la acción **Registrar**, seleccione la opción **Envío** y seleccione el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="44734-122">Choose the **Post** action, choose the **Ship** option, and then choose the **OK** button.</span></span>

    <span data-ttu-id="44734-123">Los productos ahora se encuentran en tránsito entre las ubicaciones especificadas, según la ruta de transferencia especificada.</span><span class="sxs-lookup"><span data-stu-id="44734-123">The items are now in transit between the specified locations, according to the specifies transfer route.</span></span>

    <span data-ttu-id="44734-124">Como trabajador de almacén en el almacén de procedencia de la transferencia, continúe con la recepción de los productos.</span><span class="sxs-lookup"><span data-stu-id="44734-124">As a warehouse worker at the transfer-from location, proceed to receive the items.</span></span>
4. <span data-ttu-id="44734-125">Seleccione la acción **Registrar**, seleccione la opción **Recepción** y seleccione el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="44734-125">Choose the **Post** action, choose the **Receive** option, and then choose the **OK** button.</span></span>

## <a name="to-transfer-items-with-the-item-reclassification-journal"></a><span data-ttu-id="44734-126">Para transferir productos con el diario de reclasificación de productos</span><span class="sxs-lookup"><span data-stu-id="44734-126">To transfer items with the item reclassification journal</span></span>
1. <span data-ttu-id="44734-127">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios reclas. producto** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="44734-127">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Item Reclass. Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="44734-128">En la ventana **Diarios reclasif. producto**, rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="44734-128">In the **Item Reclass. Journal** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="44734-129">En el campo **Cód. almacén**, escriba la ubicación donde se almacenan los productos actualmente.</span><span class="sxs-lookup"><span data-stu-id="44734-129">In the **Location Code** field, enter the location where the items are currently stored.</span></span>

    > [!NOTE]  
>   <span data-ttu-id="44734-130">Para transferir productos que no tienen código de almacén, deje en blanco el campo **Cód. almacén**.</span><span class="sxs-lookup"><span data-stu-id="44734-130">To transfer items that have no location code, leave the **Location Code** field blank.</span></span>
4. <span data-ttu-id="44734-131">En el campo **Cód. almacén destino**, especifique la ubicación a la que desee transferir los productos.</span><span class="sxs-lookup"><span data-stu-id="44734-131">In the **New Location Code** field, enter the location that you want to transfer the items to.</span></span>
5. <span data-ttu-id="44734-132">Seleccione la acción **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="44734-132">Choose the **Post** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="44734-133">Consulte también</span><span class="sxs-lookup"><span data-stu-id="44734-133">See Also</span></span>
[<span data-ttu-id="44734-134">Gestionar inventario</span><span class="sxs-lookup"><span data-stu-id="44734-134">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="44734-135">Configuración de almacenes</span><span class="sxs-lookup"><span data-stu-id="44734-135">How to: Set Up Locations</span></span>](inventory-how-setup-locations.md)  

<span data-ttu-id="44734-136">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="44734-136">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="44734-137">[Personalización de [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span><span class="sxs-lookup"><span data-stu-id="44734-137">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-customizing-overview.md)</span></span>  
[<span data-ttu-id="44734-138">Funciones empresariales generales</span><span class="sxs-lookup"><span data-stu-id="44734-138">General Business Functionality</span></span>](ui-across-business-areas.md)

##

