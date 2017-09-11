---
title: "Configurar o cambiar el catálogo de cuentas"
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
ms.openlocfilehash: 2a2f1f2ec3ac5bdd935ec19c11d74e16bdee7686
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a><span data-ttu-id="ed825-102">Configurar o cambiar el catálogo de cuentas</span><span class="sxs-lookup"><span data-stu-id="ed825-102">Set Up or Change the Chart of Accounts</span></span>
<span data-ttu-id="ed825-103">El catálogo de cuentas muestra las cuentas de contabilidad que almacenan sus datos financieros.</span><span class="sxs-lookup"><span data-stu-id="ed825-103">The chart of accounts shows the ledger accounts that store your financial data.</span></span> <span data-ttu-id="ed825-104">Dynamics NAV incluye un catálogo de cuentas estándar que está preparado para respaldar su negocio.</span><span class="sxs-lookup"><span data-stu-id="ed825-104">Dynamics NAV includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="ed825-105">Sin embargo, puede cambiar las cuentas predeterminadas y puede agregar nuevas cuentas.</span><span class="sxs-lookup"><span data-stu-id="ed825-105">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="ed825-106">Agregar o cambiar cuentas</span><span class="sxs-lookup"><span data-stu-id="ed825-106">Adding or Changing Accounts</span></span>
<span data-ttu-id="ed825-107">Desde el catálogo de cuentas, puede abrir cada cuenta de contabilidad y agregar o cambiar opciones.</span><span class="sxs-lookup"><span data-stu-id="ed825-107">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

<span data-ttu-id="ed825-108">**Nota**: Puede eliminar una cuenta contable.</span><span class="sxs-lookup"><span data-stu-id="ed825-108">**Note**: You can delete a general ledger account.</span></span> <span data-ttu-id="ed825-109">Sin embargo, antes de eliminarla, deben cumplirse las condiciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="ed825-109">However, before you delete it, the following must be true:</span></span>  
- <span data-ttu-id="ed825-110">El saldo de la cuenta debe ser cero.</span><span class="sxs-lookup"><span data-stu-id="ed825-110">The balance on the account must be zero.</span></span>  
- <span data-ttu-id="ed825-111">El campo **Permite borrar ctas. anteriores a** se debe configurar en la ventana **Configuración de contabilidad** y la cuenta no debe tener movimientos contables en o después de esa fecha.</span><span class="sxs-lookup"><span data-stu-id="ed825-111">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
- <span data-ttu-id="ed825-112">Si se selecciona el campo **Chequear uso ctas. cont.** en la ventana **Configuración de contabilidad**, la cuenta no se debe usar en grupos contables ni en la configuración de grupos contables.</span><span class="sxs-lookup"><span data-stu-id="ed825-112">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

<span data-ttu-id="ed825-113">Dynamics NAV impedirá que elimine una cuenta de contabilidad que almacena los datos que se necesitan en el catálogo de cuentas.</span><span class="sxs-lookup"><span data-stu-id="ed825-113">Dynamics NAV will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

##<a name="see-also"></a><span data-ttu-id="ed825-114">Consulte también</span><span class="sxs-lookup"><span data-stu-id="ed825-114">See Also</span></span>  
[<span data-ttu-id="ed825-115">Libro mayor y plan de cuentas</span><span class="sxs-lookup"><span data-stu-id="ed825-115">The General Ledger and the Chart of Accounts</span></span>](finance-setup-general-ledger.md)  
[<span data-ttu-id="ed825-116">Administrar cuentas bancarias</span><span class="sxs-lookup"><span data-stu-id="ed825-116">Manage Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="ed825-117">Dimensiones</span><span class="sxs-lookup"><span data-stu-id="ed825-117">Dimensions</span></span>](finance-setup-dimensions.md)  
[<span data-ttu-id="ed825-118">Procedimiento: Trabajar con los códigos GIFI en Canadá</span><span class="sxs-lookup"><span data-stu-id="ed825-118">How to: Work With GIFI Codes in Canada</span></span>](ca-finance-setup-work-GiFI-codes.md)

