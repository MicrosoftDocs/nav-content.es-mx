---
title: "Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 7d6ce2a9133b02a1a38cd853c34b1f3440e7a50e
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a><span data-ttu-id="eab4f-102">Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas</span><span class="sxs-lookup"><span data-stu-id="eab4f-102">How to: Enable Application of Ledger Entries in Different Currencies</span></span>
<span data-ttu-id="eab4f-103">Si se realiza una compra a un proveedor en una divisa y se emite el pago en otra divisa, es posible liquidar la compra con el pago.</span><span class="sxs-lookup"><span data-stu-id="eab4f-103">If you purchase from a vendor in one currency and submit payment in another currency, you can apply the payment to the purchase.</span></span>

<span data-ttu-id="eab4f-104">De igual modo, si vende a un cliente en una divisa y cobra en otra, puede liquidar el pago con la factura de venta.</span><span class="sxs-lookup"><span data-stu-id="eab4f-104">Likewise, if you sell to a customer in one currency and receive payment in another currency, you can apply the payment to the sales invoice.</span></span>

<span data-ttu-id="eab4f-105">El procedimiento siguiente describe cómo configurarlo para movimientos de proveedor en la ventana **Configuración de compras y pagos**.</span><span class="sxs-lookup"><span data-stu-id="eab4f-105">The following procedure describes how to set this up for vendor ledger entries in the **Purchases & Payables Setup** window.</span></span> <span data-ttu-id="eab4f-106">La configuración es similar para los movimientos de cliente en la ventana **Configuración de ventas y cobros**.</span><span class="sxs-lookup"><span data-stu-id="eab4f-106">The setup is similar for customer ledger entries in the **Sales & Receivables Setup** window.</span></span>

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a><span data-ttu-id="eab4f-107">Para permitir la liquidación de movimientos de proveedor en divisas distintas</span><span class="sxs-lookup"><span data-stu-id="eab4f-107">To enable application of vendor ledger entries in different currencies</span></span>
1. <span data-ttu-id="eab4f-108">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de compras y pagos** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="eab4f-108">In the top right corner, choose the **Search for Page or Report** icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="eab4f-109">En el campo **Liquidación entre divisas**, seleccione una de las siguientes opciones.</span><span class="sxs-lookup"><span data-stu-id="eab4f-109">In the **Appln. between Currencies** field, select one of the following options.</span></span>

|<span data-ttu-id="eab4f-110">Opción</span><span class="sxs-lookup"><span data-stu-id="eab4f-110">Option</span></span> |<span data-ttu-id="eab4f-111">Descripción</span><span class="sxs-lookup"><span data-stu-id="eab4f-111">Description</span></span> |
|-------|------------|
|<span data-ttu-id="eab4f-112">Ninguno</span><span class="sxs-lookup"><span data-stu-id="eab4f-112">None</span></span>|<span data-ttu-id="eab4f-113">No se permite la liquidación entre divisas.</span><span class="sxs-lookup"><span data-stu-id="eab4f-113">Application between currencies is not allowed.</span></span>|
|<span data-ttu-id="eab4f-114">UME</span><span class="sxs-lookup"><span data-stu-id="eab4f-114">EMU</span></span>|<span data-ttu-id="eab4f-115">Se permite la liquidación entre divisas de la UME.</span><span class="sxs-lookup"><span data-stu-id="eab4f-115">Application between EMU currencies is allowed.</span></span>|
|<span data-ttu-id="eab4f-116">Todo</span><span class="sxs-lookup"><span data-stu-id="eab4f-116">All</span></span>|<span data-ttu-id="eab4f-117">Se permite la liquidación entre todas las divisas.</span><span class="sxs-lookup"><span data-stu-id="eab4f-117">Application between all currencies is allowed.</span></span>

## <a name="see-also"></a><span data-ttu-id="eab4f-118">Consulte también</span><span class="sxs-lookup"><span data-stu-id="eab4f-118">See Also</span></span>  
[<span data-ttu-id="eab4f-119">Gestionar pagos</span><span class="sxs-lookup"><span data-stu-id="eab4f-119">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="eab4f-120">Gestionar cobros</span><span class="sxs-lookup"><span data-stu-id="eab4f-120">Manage Receivables</span></span>](receivables-manage-receivables.md)

