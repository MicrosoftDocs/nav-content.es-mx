---
title: "Nuevo cálculo de IVA"
description: "Cuando un cliente efectúa un pago en divisa extranjera, se debe volver a calcular el IVA con el tipo de cambio vigente al momento del pago de la factura."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 11f227bccc0be52bf6da79206a961d28428d32ea
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="vat-recalculation"></a><span data-ttu-id="11b54-103">Nuevo cálculo de IVA</span><span class="sxs-lookup"><span data-stu-id="11b54-103">VAT Recalculation</span></span>
<span data-ttu-id="11b54-104">Cuando un cliente efectúa un pago en divisa extranjera, se debe volver a calcular el IVA con el tipo de cambio vigente al momento del pago de la factura.</span><span class="sxs-lookup"><span data-stu-id="11b54-104">When a customer makes payment in a foreign currency, VAT must be recalculated using the exchange rate at the time of the invoice payment.</span></span>  
  
 <span data-ttu-id="11b54-105">Una empresa confecciona una factura en divisa extranjera cuando un cliente extranjero compra bienes o servicios sujetos a impuestos.</span><span class="sxs-lookup"><span data-stu-id="11b54-105">A company creates an invoice in a foreign currency for the purchase of taxable goods and taxable services by a foreign customer.</span></span> <span data-ttu-id="11b54-106">La factura ../../el IVA.</span><span class="sxs-lookup"><span data-stu-id="11b54-106">This invoice ../../includes VAT.</span></span> <span data-ttu-id="11b54-107">Cuando el cliente posteriormente realiza el pago, se vuelve a calcular el IVA en función del importe de venta original y se ajusta según el tipo de cambio actual.</span><span class="sxs-lookup"><span data-stu-id="11b54-107">When the customer makes the payment at a later date, VAT is recalculated based on the original sales amount, and adjusted for the new currency rates.</span></span>  
  
 <span data-ttu-id="11b54-108">A continuación, se muestra cómo crear un informe sobre importes de IVA no realizados:</span><span class="sxs-lookup"><span data-stu-id="11b54-108">The following steps show how to create a report for unrealized VAT amounts:</span></span>  
  
-   <span data-ttu-id="11b54-109">Defina una opción para permitir volver a calcular el IVA después de recibido el pago.</span><span class="sxs-lookup"><span data-stu-id="11b54-109">Set up an option to allow recalculation of VAT upon receipt of payment.</span></span>  
  
-   <span data-ttu-id="11b54-110">Vuelva a calcular el IVA después de recibido el pago.</span><span class="sxs-lookup"><span data-stu-id="11b54-110">Recalculate VAT upon receipt of payment.</span></span>  
  
-   <span data-ttu-id="11b54-111">Ajuste los movimientos del diario correspondientes a la realización de los impuestos de IVA para reconocer las diferencias de tipo de cambio.</span><span class="sxs-lookup"><span data-stu-id="11b54-111">Adjust journal entries for realization of VAT taxes payable to recognize exchange differences.</span></span>  
  
-   <span data-ttu-id="11b54-112">Cree una declaración de IVA que muestre los importes de IVA no realizados.</span><span class="sxs-lookup"><span data-stu-id="11b54-112">Create a VAT statement that shows the unrealized VAT amounts.</span></span> <span data-ttu-id="11b54-113">Para obtener más información, consulte [Crear una declaración de IVA](how-to-define-vat-statements.md).</span><span class="sxs-lookup"><span data-stu-id="11b54-113">For more information, see [Create a VAT Statement](how-to-define-vat-statements.md).</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="11b54-114">Consulte también</span><span class="sxs-lookup"><span data-stu-id="11b54-114">See Also</span></span>  
 <span data-ttu-id="11b54-115">[Procedimiento para definir declaraciones de IVA](how-to-define-vat-statements.md) </span><span class="sxs-lookup"><span data-stu-id="11b54-115">[How to: Define VAT Statements](how-to-define-vat-statements.md) </span></span>  
 <span data-ttu-id="11b54-116">Lín. declaración IVA</span><span class="sxs-lookup"><span data-stu-id="11b54-116">VAT Statement Line</span></span>   
 <span data-ttu-id="11b54-117">[Procedimiento: Configurar el impuesto sobre las ventas no realizado y los descuentos por pago de ventas](how-to-set-up-unrealized-sales-tax-and-sales-payment-discounts.md) </span><span class="sxs-lookup"><span data-stu-id="11b54-117">[How to: Set Up Unrealized Sales Tax and Sales Payment Discounts](how-to-set-up-unrealized-sales-tax-and-sales-payment-discounts.md) </span></span>  
 [<span data-ttu-id="11b54-118">Funcionalidad local de México</span><span class="sxs-lookup"><span data-stu-id="11b54-118">Mexico Local Functionality</span></span>](mexico-local-functionality.md)
