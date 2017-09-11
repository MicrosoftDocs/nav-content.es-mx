---
title: Cerrar periodos
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a><span data-ttu-id="28a5c-102">Cerrar periodos</span><span class="sxs-lookup"><span data-stu-id="28a5c-102">Close Periods</span></span>
<span data-ttu-id="28a5c-103">La aplicación no le exige que cierre los periodos, sin embargo, puede realizar muchas actividades de fin de periodo (fin de mes) si lo desea.</span><span class="sxs-lookup"><span data-stu-id="28a5c-103">The application does not force you to close periods, however, there are many period-end (month-end) activities that can be performed in the application if you want.</span></span> <span data-ttu-id="28a5c-104">Este tema proporciona una descripción general de estos procesos y actividades, que pueden ser o no ser necesarios para su empresa.</span><span class="sxs-lookup"><span data-stu-id="28a5c-104">This topic provides an overview of these processes and activities, which may or may not be necessary for your company.</span></span>

## <a name="general-ledger"></a><span data-ttu-id="28a5c-105">Contabilidad</span><span class="sxs-lookup"><span data-stu-id="28a5c-105">General Ledger</span></span>
* <span data-ttu-id="28a5c-106">Especifique fechas de registro para todos el sistema y específicos para el usuario.</span><span class="sxs-lookup"><span data-stu-id="28a5c-106">Specify system-wide and user-specific posting period.</span></span>

    <span data-ttu-id="28a5c-107">Esto especifica las fechas entre las cuales se permiten los registros.</span><span class="sxs-lookup"><span data-stu-id="28a5c-107">This specifies the dates between which postings are allowed.</span></span> <span data-ttu-id="28a5c-108">En función de sus necesidades comerciales, puede restringir los intervalos de fechas de registro de los usuarios al inicio del proceso de fin de periodo o posteriormente durante el fin del periodo.</span><span class="sxs-lookup"><span data-stu-id="28a5c-108">Depending on your business needs, you may want to restrict user posting date ranges at the start of the period-end process or at later time towards the end of the period.</span></span> <span data-ttu-id="28a5c-109">Para obtener más información, vea [Procedimiento: Especificar periodos de registro](finance-setup-how-specify-posting-periods.md).</span><span class="sxs-lookup"><span data-stu-id="28a5c-109">For more information, see [How to: Specify Posting Periods](finance-setup-how-specify-posting-periods.md).</span></span>
* <span data-ttu-id="28a5c-110">Lleve a cabo todos los ajustes de contabilidad necesarios</span><span class="sxs-lookup"><span data-stu-id="28a5c-110">Make all necessary G/L adjustments.</span></span>
* <span data-ttu-id="28a5c-111">Actualice y registre los Diarios periódicos.</span><span class="sxs-lookup"><span data-stu-id="28a5c-111">Update and post Recurring Journals.</span></span>
<!--* Process Consolidations-->
* <span data-ttu-id="28a5c-112">Ejecute los esquemas de cuentas como se indica a continuación:</span><span class="sxs-lookup"><span data-stu-id="28a5c-112">Run account schedules as follows:</span></span>
  1. <span data-ttu-id="28a5c-113">Abra la ventana **Estructura de cuentas** y seleccione la acción **Imprimir**.</span><span class="sxs-lookup"><span data-stu-id="28a5c-113">Open the **Account Schedule** window, and choose the **Print** action.</span></span>
  2. <span data-ttu-id="28a5c-114">Rellene la ventana de solicitud **Esquema cuentas** y seleccione la acción **Imprimir**.</span><span class="sxs-lookup"><span data-stu-id="28a5c-114">Fill the **Account Schedule** request window and choose the **Print** action.</span></span>

## <a name="sales--receivables"></a><span data-ttu-id="28a5c-115">Ventas y cobros</span><span class="sxs-lookup"><span data-stu-id="28a5c-115">Sales & Receivables</span></span>
* <span data-ttu-id="28a5c-116">Registre todas las órdenes, facturas, notas de crédito y devoluciones de ventas.</span><span class="sxs-lookup"><span data-stu-id="28a5c-116">Post all sales orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="28a5c-117">Registre todo los diarios de recepciones de efectivo.</span><span class="sxs-lookup"><span data-stu-id="28a5c-117">Post all cash receipt journals.</span></span>
* <span data-ttu-id="28a5c-118">Actualice y registre los diarios periódicos relativos a ventas y cobros.</span><span class="sxs-lookup"><span data-stu-id="28a5c-118">Update and post recurring journals that are related to Sales & Receivables.</span></span>
* <span data-ttu-id="28a5c-119">Concilie los cobros en el libro de contabilidad</span><span class="sxs-lookup"><span data-stu-id="28a5c-119">Reconcile accounts receivable to the general ledger.</span></span>
* <span data-ttu-id="28a5c-120">Ejecute el proceso **Eliminar peds. venta factdos**.</span><span class="sxs-lookup"><span data-stu-id="28a5c-120">Run the **Delete Invoiced Sales Orders** batch job.</span></span>

## <a name="purchases--payables"></a><span data-ttu-id="28a5c-121">Compras y pagos</span><span class="sxs-lookup"><span data-stu-id="28a5c-121">Purchases & Payables</span></span>
* <span data-ttu-id="28a5c-122">Registre todas las órdenes, facturas, notas de crédito y devoluciones de compra.</span><span class="sxs-lookup"><span data-stu-id="28a5c-122">Post all purchase orders, invoices, credit memos, and return orders.</span></span>
* <span data-ttu-id="28a5c-123">Registre todos los registros de pagos.</span><span class="sxs-lookup"><span data-stu-id="28a5c-123">Post all payment journals.</span></span>
* <span data-ttu-id="28a5c-124">Actualice y registre los diarios periódicos que son relativos a compras y pagos.</span><span class="sxs-lookup"><span data-stu-id="28a5c-124">Update and post recurring journals that are related to purchases & payables.</span></span>
* <span data-ttu-id="28a5c-125">Ejecute el informe **Antigüedad pagos** y concilie las cuentas por pagar en el libro de contabilidad.</span><span class="sxs-lookup"><span data-stu-id="28a5c-125">Run the **Aged Accounts Payable** report and reconcile accounts payable to the general ledger.</span></span>
* <span data-ttu-id="28a5c-126">Ejecute el proceso **Eliminar peds. compra factdos**.</span><span class="sxs-lookup"><span data-stu-id="28a5c-126">Run the **Delete Invoiced Purchase Orders** batch job.</span></span>

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a><span data-ttu-id="28a5c-127">Calcular y procesar los impuestos de venta</span><span class="sxs-lookup"><span data-stu-id="28a5c-127">Calculate and Process Sales Tax</span></span>
*  <span data-ttu-id="28a5c-128">Realice los extractos de impuesto.</span><span class="sxs-lookup"><span data-stu-id="28a5c-128">Complete Tax Statements.</span></span>

## <a name="see-also"></a><span data-ttu-id="28a5c-129">Consulte también</span><span class="sxs-lookup"><span data-stu-id="28a5c-129">See Also</span></span>
[<span data-ttu-id="28a5c-130">Cerrar años y periodos</span><span class="sxs-lookup"><span data-stu-id="28a5c-130">Closing Years and Periods</span></span>](year-close-years-periods.md)  
[<span data-ttu-id="28a5c-131">Cerrar libros</span><span class="sxs-lookup"><span data-stu-id="28a5c-131">Close Books</span></span>](year-close-books.md)

