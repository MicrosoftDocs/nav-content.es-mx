---
title: Registrar ventas
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
ms.openlocfilehash: e87dd5faf7713aecfbe7209d00bb8076fcae9d25
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="posting-sales"></a><span data-ttu-id="cd7c6-102">Registrar ventas</span><span class="sxs-lookup"><span data-stu-id="cd7c6-102">Posting Sales</span></span>
<span data-ttu-id="cd7c6-103">En **Grupo contable** en un documento de ventas, puede elegir entre las funciones de registro siguientes:</span><span class="sxs-lookup"><span data-stu-id="cd7c6-103">In the **Posting group** on a sales document, you can choose between the following posting functions:</span></span>

- <span data-ttu-id="cd7c6-104">**Registrar**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-104">**Post**</span></span>
- <span data-ttu-id="cd7c6-105">**Informe de prueba**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-105">**Test Report**</span></span>
- <span data-ttu-id="cd7c6-106">**Registrar y enviar**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-106">**Post and Send**</span></span>
- <span data-ttu-id="cd7c6-107">**Registrar e imprimir**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-107">**Post and Print**</span></span>
- <span data-ttu-id="cd7c6-108">**Registrar y enviar por correo electrónico**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-108">**Post and Email**</span></span>
- <span data-ttu-id="cd7c6-109">**Registrar por lotes**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-109">**Post Batch**</span></span>
- <span data-ttu-id="cd7c6-110">**Vista previa de registro**</span><span class="sxs-lookup"><span data-stu-id="cd7c6-110">**Preview Posting**</span></span>

<span data-ttu-id="cd7c6-111">Una vez completadas todas las líneas e introducida toda la información en la orden de venta, puede registrarla.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-111">When you have completed all the lines and entered all the information on the sales order, you can post it.</span></span> <span data-ttu-id="cd7c6-112">Esto crea una remisión y una factura.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-112">This creates a shipment and an invoice.</span></span>

<span data-ttu-id="cd7c6-113">Cuando se registra una orden de venta, se actualiza la cuenta del cliente, la contabilidad y los movimientos de producto.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-113">When a sales order is posted, the customer's account, the general ledger, and the item ledger entries are updated.</span></span>

<span data-ttu-id="cd7c6-114">Por cada orden de venta, se crea un movimiento de venta en la tabla **Mov. contabilidad**.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-114">For each sales order, a sales entry is created in the **G/L Entry** table.</span></span> <span data-ttu-id="cd7c6-115">Se crea también un movimiento en la cuenta de cliente de la tabla **Mov. cliente** y un movimiento de contabilidad en la cuenta de cliente correspondiente.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-115">An entry is also created in the customer's account in the **Cust. Ledger Entry** table and a general ledger entry is created in the relevant receivables account.</span></span> <span data-ttu-id="cd7c6-116">Además, el registro de la orden puede dar como resultado un movimiento de IVA y uno de contabilidad para el importe de descuento.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-116">In addition, posting the order may result in a VAT entry and a general ledger entry for the discount amount.</span></span> <span data-ttu-id="cd7c6-117">El registro de un movimiento para el descuento depende del contenido del campo **Registro dto.** de la ventana **Conf. ventas y cobros**.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-117">Whether an entry for the discount is posted depends on the contents of the **Discount Posting** field in the **Sales & Receivables Setup** window.</span></span>

<span data-ttu-id="cd7c6-118">Por cada línea de orden de venta, se creará un movimiento de producto en la tabla **Mov. producto** (si las líneas de venta contienen números de producto) o un movimiento de contabilidad en la tabla **Mov. contabilidad** (si las líneas de venta contienen una cuenta de contabilidad).</span><span class="sxs-lookup"><span data-stu-id="cd7c6-118">For each sales order line, an item ledger entry will be created in the **Item Ledger Entry** table (if the sales lines contain item numbers) or a general ledger entry will be created in the **G/L Entry** table (if the sales lines contain a general ledger account).</span></span> <span data-ttu-id="cd7c6-119">Además, las órdenes de venta siempre se registran en las tablas **Histórico cab. remisión venta** y **Histórico cab. factura venta**.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-119">In addition to this, sales orders are always recorded in the **Sales Shipment Header** and **Sales Invoice Header** tables.</span></span>

<span data-ttu-id="cd7c6-120">**Importante**: Cuando registre una orden, puede crear una remisión y una factura.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-120">**Important**: When you post an order, you can create both a shipment and an invoice.</span></span> <span data-ttu-id="cd7c6-121">Esto se puede realizar al mismo tiempo o de manera independiente.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-121">These can be done at the same time or independently.</span></span> <span data-ttu-id="cd7c6-122">También puede crear una remisión y una factura parciales completando los campos **Cantidad a enviar** y **Cantidad a facturar** en las líneas individuales de la orden de venta antes de registrar.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-122">You can also create a partial shipment and a partial invoice by completing the **Qty. to Ship** and **Qty. to Invoice** fields on the individual sales order lines before you post.</span></span> <span data-ttu-id="cd7c6-123">Tenga en cuenta que no puede crear una factura de algo no se ha enviado.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-123">Note that you cannot create an invoice for something that is not shipped.</span></span> <span data-ttu-id="cd7c6-124">Es decir, antes de poder facturar, tiene que haber registrado una remisión de venta o haber seleccionado, al mismo tiempo, entregar y facturar.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-124">That is, before you can invoice, you must have recorded a shipment, or you must choose to ship and invoice at the same time.</span></span> 

<span data-ttu-id="cd7c6-125">Una vez completado el registro, las líneas de venta registradas se quitan de la orden.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-125">When the posting is completed, the posted sales lines are removed from the order.</span></span> <span data-ttu-id="cd7c6-126">Al terminar el registro aparece un mensaje de aviso.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-126">A message tells you when the posting is completed.</span></span> <span data-ttu-id="cd7c6-127">Después de esto, podrá ver los movimientos registrados en las diferentes ventanas que los contienen, como **Movs. cliente**, **Movs. contabilidad**, **Movs. producto**, **Histórico albaranes ventas** y **Histórico facturas venta**.</span><span class="sxs-lookup"><span data-stu-id="cd7c6-127">After this, you will be able to see the posted entries in the various windows that contain posted entries, such as the **Cust. Ledger Entries**, **G/L Entries**, **Item Ledger Entries**, **Posted Sales Shipments**, and **Posted Sales Invoices** windows.</span></span>

## <a name="see-also"></a><span data-ttu-id="cd7c6-128">Consulte también</span><span class="sxs-lookup"><span data-stu-id="cd7c6-128">See Also</span></span>
[<span data-ttu-id="cd7c6-129">Enviar documentos por correo electrónico</span><span class="sxs-lookup"><span data-stu-id="cd7c6-129">How to: Send Documents by Email</span></span>](ui-how-send-documents-email.md)

