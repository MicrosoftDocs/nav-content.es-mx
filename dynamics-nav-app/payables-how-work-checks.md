---
title: 'Procedimiento: Trabajar con cheques'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 421516a7580a90d6eabc8ecfcc841215839994c9
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-checks"></a><span data-ttu-id="23cb6-102">Procedimiento: Trabajar con cheques</span><span class="sxs-lookup"><span data-stu-id="23cb6-102">How to: Work With Checks</span></span>
<span data-ttu-id="23cb6-103">Dynamics NAV admite la emisión de cheques electrónica y manual.</span><span class="sxs-lookup"><span data-stu-id="23cb6-103">Dynamics NAV supports electronic and manual check issuance.</span></span> <span data-ttu-id="23cb6-104">Ambos métodos utilizan el diario de pagos para emitir los cheques a proveedores.</span><span class="sxs-lookup"><span data-stu-id="23cb6-104">Both methods use the payment journal to issue checks to vendors.</span></span> <span data-ttu-id="23cb6-105">También puede anular cheques y ver movimientos de cheques.</span><span class="sxs-lookup"><span data-stu-id="23cb6-105">You can also void checks and view check ledger entries.</span></span>

<span data-ttu-id="23cb6-106">El proceso de emisión de cheques propone pagos, crea movimientos e imprime los cheques automáticos.</span><span class="sxs-lookup"><span data-stu-id="23cb6-106">The process of issuing checks suggests payments, creates ledger entries, and prints the computer checks.</span></span>

<span data-ttu-id="23cb6-107">Su impresora tiene que haber configurado correctamente los documentos y usted deberá definir qué plantilla de cheques va a usar.</span><span class="sxs-lookup"><span data-stu-id="23cb6-107">Your printer must be correctly set up with the check forms, and you must define which check layout to use.</span></span> <span data-ttu-id="23cb6-108">Para obtener más información , vea [Procedimiento: Definir plantillas de cheques](finance-setup-how-define-check-layouts.md)</span><span class="sxs-lookup"><span data-stu-id="23cb6-108">For more information, see [How to: Define Check Layouts](finance-setup-how-define-check-layouts.md)</span></span>

## <a name="to-issue-checks"></a><span data-ttu-id="23cb6-109">Para emitir cheques</span><span class="sxs-lookup"><span data-stu-id="23cb6-109">To issue checks</span></span>
1. <span data-ttu-id="23cb6-110">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de pago** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="23cb6-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Payment Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="23cb6-111">Rellene el diario con los pagos relevantes, por ejemplo, mediante la función Proponer pagos a proveedores.</span><span class="sxs-lookup"><span data-stu-id="23cb6-111">Fill in the journal with relevant payments, for example by using the Suggest Vendor Payments function.</span></span> <span data-ttu-id="23cb6-112">Para obtener más información, vea [Procedimiento: Proponer pagos a proveedores](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="23cb6-112">For more information, see [How to: Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>
3. <span data-ttu-id="23cb6-113">En el campo **Tipo de pago bancario** en las líneas de diario para el pago que desea realizar mediante cheques, seleccione una de las opciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="23cb6-113">In the **Bank Payment Type** field on journal lines for payment that you want to make with checks, select one of the following options:</span></span>

 - <span data-ttu-id="23cb6-114">**Cheque automático**: Seleccione esta opción si desea imprimir un cheque por el importe de la línea del diario de pagos.</span><span class="sxs-lookup"><span data-stu-id="23cb6-114">**Computer Check**: Select this option if you want to print a check for the amount on the payment journal line.</span></span> <span data-ttu-id="23cb6-115">Debe imprimir los cheques antes de que pueda registrar las líneas del diario.</span><span class="sxs-lookup"><span data-stu-id="23cb6-115">You must print the checks before you can post the journal lines.</span></span> <span data-ttu-id="23cb6-116">solo puede seleccionar **Cheque automático** si el valor de **Tipo contrapartida** o el de **Tipo mov.** es **Cuenta banco**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-116">You can only select **Computer Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

 - <span data-ttu-id="23cb6-117">**Cheque manual**: Seleccione esta opción si ha creado manualmente un cheque y desea crear el movimiento de cheque correspondiente a ese importe.</span><span class="sxs-lookup"><span data-stu-id="23cb6-117">**Manual Check**: Select this option if you have created a check manually and want to create a corresponding check ledger entry for this amount.</span></span> <span data-ttu-id="23cb6-118">Usando esta opción no puede imprimir cheques de Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="23cb6-118">By using this option, you cannot print checks from Dynamics NAV.</span></span> <span data-ttu-id="23cb6-119">solo puede seleccionar **Cheque manual** si el valor de **Tipo contrapartida** o el de **Tipo mov.** es **Cuenta banco**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-119">You can only select **Manual Check** if the **Bal. Account Type** or the **Account Type** is **Bank Account**.</span></span>

    <span data-ttu-id="23cb6-120">**Nota**: Debe imprimir los cheques automáticos antes de registrar las líneas del diario relacionadas.</span><span class="sxs-lookup"><span data-stu-id="23cb6-120">**Note**: You must print computer checks before you post the related journal lines.</span></span>
4. <span data-ttu-id="23cb6-121">En el caso de los cheques automáticos, seleccione **Imprimir cheque**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-121">In case of computer checks, choose **Print Check**.</span></span>
5. <span data-ttu-id="23cb6-122">En la ventana **Cheque**, rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="23cb6-122">In the **Check** window, fill in the fields as necessary.</span></span> <span data-ttu-id="23cb6-123">Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.</span><span class="sxs-lookup"><span data-stu-id="23cb6-123">Choose a field to read a short description of the field or link to more information.</span></span>
6. <span data-ttu-id="23cb6-124">Elija el botón **Imprimir**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-124">Choose the **Print** button.</span></span>

<span data-ttu-id="23cb6-125">**Nota**: Si desea imprimir cheques en varias divisas de cuentas bancarias distintas, deberá ejecutar el proceso **Imprimir cheque** por separado para cada divisa y especificar la cuenta bancaria correspondiente.</span><span class="sxs-lookup"><span data-stu-id="23cb6-125">**Note**: If you want to print checks in more than one currency from different bank accounts, you must run the **Print Check** batch job separately for each currency and specify the appropriate bank account.</span></span>

## <a name="to-cancel-printed-checks-that-are-not-posted"></a><span data-ttu-id="23cb6-126">Para anular los cheques imprimidos que no han sido registrados</span><span class="sxs-lookup"><span data-stu-id="23cb6-126">To cancel printed checks that are not posted</span></span>
<span data-ttu-id="23cb6-127">Puede anular los cheques no registrados después de que hayan sido imprimidos usando la acción **Anular cheque** de la ventana **Diario de pagos**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-127">You can cancel non-posted checks after they have been printed by using the **Void Check** action in the **Payment Journal** window.</span></span>
1. <span data-ttu-id="23cb6-128">En la ventana **Diario de pagos**, seleccione **Anular cheque** y, a continuación, seleccione que cheques desea cancelar.</span><span class="sxs-lookup"><span data-stu-id="23cb6-128">In the **Payment Journal** window, choose the **Void Check**, and then choose which checks to cancel.</span></span>

## <a name="to-void-checks"></a><span data-ttu-id="23cb6-129">Para anular cheques</span><span class="sxs-lookup"><span data-stu-id="23cb6-129">To void checks</span></span>
<span data-ttu-id="23cb6-130">Cuando se ha registrado el pago del cheque, solo puede cancelar (anular) cheques en los movimientos resultantes del banco.</span><span class="sxs-lookup"><span data-stu-id="23cb6-130">When check payment have been posted, you can only cancel (void) checks from the resulting bank ledger entries.</span></span>

1. <span data-ttu-id="23cb6-131">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="23cb6-131">In the top right corner, choose the **Search for Page or Report** icon, enter **Bank Accounts**, and then choose the related link.</span></span>
2. <span data-ttu-id="23cb6-132">Seleccione la cuenta bancaria correspondiente, seleccione la acción **Editar** y, a continuación, seleccione la acción **Movs. cheques**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-132">Select the relevant bank account, choose the **Edit** action, and then choose the **Check Ledger Entries** action.</span></span>
3. <span data-ttu-id="23cb6-133">En la ventana **Movs. cheques**, seleccione la acción **Anular cheque**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-133">In the **Check Ledger Entries** window, choose the **Void Check** action.</span></span>
4. <span data-ttu-id="23cb6-134">Active la casilla **Anular cheque sólo**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-134">Select the **Void Check Only** check box.</span></span>
5. <span data-ttu-id="23cb6-135">Elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="23cb6-135">Choose the **OK**button.</span></span>

## <a name="see-also"></a><span data-ttu-id="23cb6-136">Consulte también</span><span class="sxs-lookup"><span data-stu-id="23cb6-136">See Also</span></span>
[<span data-ttu-id="23cb6-137">Gestionar pagos</span><span class="sxs-lookup"><span data-stu-id="23cb6-137">Manage Payables</span></span>](payables-manage-payables.md)  
[<span data-ttu-id="23cb6-138">Configurar la banca</span><span class="sxs-lookup"><span data-stu-id="23cb6-138">Set Up Banking</span></span>](bank-setup-banking.md)  

