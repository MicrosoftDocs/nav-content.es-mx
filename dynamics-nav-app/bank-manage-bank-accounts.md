---
title: Administrar cuentas bancarias
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
ms.openlocfilehash: d97c3afba0e899768bda1b637c4f288db210d38c
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="manage-bank-accounts"></a><span data-ttu-id="cf8ed-102">Administrar cuentas bancarias</span><span class="sxs-lookup"><span data-stu-id="cf8ed-102">Manage Bank Accounts</span></span>
<span data-ttu-id="cf8ed-103">A intervalos regulares, debe conciliar sus movimientos bancarios en Dynamics NAV con las transacciones bancarias relacionadas a cuentas bancarias en su banco y, a continuación, registrar el saldo en su cuenta bancaria.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-103">At regular intervals, you must reconcile your bank ledger entries in Dynamics NAV with the related bank transactions in bank accounts at your bank, and then post the balance to your bank account.</span></span> <span data-ttu-id="cf8ed-104">Puede realizar esta tarea, ya sea como parte del procesamiento de los pagos representados en un estado de cuenta bancario en el **Diario de conciliación de pagos**.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-104">You can perform this task either as part of processing the payments represented on a bank statement in the **Payment Reconciliation Journal**.</span></span> <span data-ttu-id="cf8ed-105">O, de forma alternativa, puede realizar la tarea por separado del procesamiento de los pagos, en la ventana **Conciliación de cuentas bancarias** que admite movimientos de cheque.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-105">Alternatively, you can perform the task separately from payment processing, in the **Bank Acc. Reconciliation** window, which supports check ledger entries.</span></span> <span data-ttu-id="cf8ed-106">En ambos casos, puede rellenar las ventanas importando el estado de cuenta bancario a Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-106">In both cases, you fill the windows by importing the bank statement into Dynamics NAV.</span></span>

<span data-ttu-id="cf8ed-107">A veces, debe transferir importes entre las cuentas bancarias en Dynamics NAV para reflejar las transferencias en su cuenta bancaria.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-107">Sometimes, you need to transfer amounts between bank account in Dynamics NAV to reflect transfers at your bank.</span></span> <span data-ttu-id="cf8ed-108">Puede realizar esta tarea en la ventana **Diario general**, de diferentes maneras en función de la divisa de los fondos.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-108">You perform this task in the **General Journal** window, in different ways depending on the currency of the funds.</span></span>

<span data-ttu-id="cf8ed-109">Para poder gestionar las cuentas bancarias, debe configurar cada cuenta bancaria como una ficha de banco.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-109">Before you can manage bank accounts, you must set each bank account up as a bank account card.</span></span> <span data-ttu-id="cf8ed-110">Además, debe configurar los servicios electrónicos que puede usar para importar estados de cuenta bancarios y exportar archivos de pagos.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-110">In addition, you must set up electronic services that you may use for bank statement import and payment file export.</span></span> <span data-ttu-id="cf8ed-111">Para obtener más información, consulte [Configurar cuentas bancarias](bank-setup-banking.md).</span><span class="sxs-lookup"><span data-stu-id="cf8ed-111">For more information, see [Set Up Bank Accounts](bank-setup-banking.md).</span></span>

<span data-ttu-id="cf8ed-112">En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="cf8ed-113">Para</span><span class="sxs-lookup"><span data-stu-id="cf8ed-113">To</span></span> |<span data-ttu-id="cf8ed-114">Vea</span><span class="sxs-lookup"><span data-stu-id="cf8ed-114">See</span></span> |
|---|----|
|<span data-ttu-id="cf8ed-115">Concilie cuentas bancarias relacionadas en relación con el procesamiento de pagos en la ventana **Diario de conciliación de pagos**.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-115">Reconcile bank accounts in connection with payment processing in the **Payment Reconciliation Journal** window.</span></span>|[<span data-ttu-id="cf8ed-116">Liquidar pagos automáticamente y conciliar cuentas bancarias</span><span class="sxs-lookup"><span data-stu-id="cf8ed-116">Apply Payments Automatically and Reconcile Bank Accounts</span></span>](receivables-apply-payments-auto-reconcile-bank-accounts.md)|
|<span data-ttu-id="cf8ed-117">Concilie cuentas bancarias, incluidos los movimientos de cheque, como una tarea independiente en la ventana **Conciliación de cuentas bancarias**.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-117">Reconcile bank accounts, including check ledger entries, as a separate task in the **Bank Acc. Reconciliation** window.</span></span>|[<span data-ttu-id="cf8ed-118">Conciliar cuentas bancarias</span><span class="sxs-lookup"><span data-stu-id="cf8ed-118">How to: Reconcile Bank Accounts Separately</span></span>](bank-how-reconcile-bank-accounts-separately.md)|
|<span data-ttu-id="cf8ed-119">Registre transferencias entre bancos en la misma divisa o en divisas diferentes.</span><span class="sxs-lookup"><span data-stu-id="cf8ed-119">Post transfers between bank accounts in the same currency or in different currencies.</span></span>|[<span data-ttu-id="cf8ed-120">Procedimiento: Transferir fondos bancarios</span><span class="sxs-lookup"><span data-stu-id="cf8ed-120">How to: Transfer Bank Funds</span></span>](bank-how-transfer-bank-funds.md)
## <a name="see-also"></a><span data-ttu-id="cf8ed-121">Consulte también</span><span class="sxs-lookup"><span data-stu-id="cf8ed-121">See Also</span></span>  
[<span data-ttu-id="cf8ed-122">Configurar la banca</span><span class="sxs-lookup"><span data-stu-id="cf8ed-122">Set Up Banking</span></span>](bank-setup-banking.md)  
[<span data-ttu-id="cf8ed-123">Gestionar cobros</span><span class="sxs-lookup"><span data-stu-id="cf8ed-123">Manage Receivables</span></span>](receivables-manage-receivables.md)  
<span data-ttu-id="cf8ed-124">[Gestionar pagos](payables-manage-payables.md)  </span><span class="sxs-lookup"><span data-stu-id="cf8ed-124">[Manage Payables](payables-manage-payables.md)  </span></span>  
[<span data-ttu-id="cf8ed-125">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="cf8ed-125">Work With Dynamics NAV</span></span>](ui-work-product.md)  
[<span data-ttu-id="cf8ed-126">Con varias áreas de negocio</span><span class="sxs-lookup"><span data-stu-id="cf8ed-126">Across Business Areas</span></span>](ui-across-business-areas.md)

