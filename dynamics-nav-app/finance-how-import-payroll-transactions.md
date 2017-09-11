---
title: "Procedimiento: importar transacciones de nómina "
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: d5e70a0a1659c7facdeec3f0971eda43ff8a03cc
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-import-payroll-transactions"></a><span data-ttu-id="56435-102">Procedimiento: importar transacciones de nómina </span><span class="sxs-lookup"><span data-stu-id="56435-102">How to: Import Payroll Transactions</span></span>
<span data-ttu-id="56435-103">Para contabilizar los pagos de salario y transacciones relacionadas, deberá importar y registrar las transacciones financieras de salario creadas para el proveedor de nóminas al libro mayor.</span><span class="sxs-lookup"><span data-stu-id="56435-103">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="56435-104">Para ello, primero importe un archivo csv</span><span class="sxs-lookup"><span data-stu-id="56435-104">To do this, you first import a csv.</span></span> <span data-ttu-id="56435-105">que recibirá del proveedor de nóminas a la ventana **Diario general**.</span><span class="sxs-lookup"><span data-stu-id="56435-105">file that you receive from the payroll provider into the **General Journal** window.</span></span> <span data-ttu-id="56435-106">A continuación asigne las cuentas externas del archivo de nóminas a las cuentas correspondientes.</span><span class="sxs-lookup"><span data-stu-id="56435-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="56435-107">Por último, registre las transacciones de nómina según el mapeo de cuentas.</span><span class="sxs-lookup"><span data-stu-id="56435-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="56435-108">Para importar un archivo de nómina</span><span class="sxs-lookup"><span data-stu-id="56435-108">To import a payroll file</span></span>
1. <span data-ttu-id="56435-109">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios generales** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="56435-109">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="56435-110">En la sección del diario general correspondiente, elija la acción **Importar transacciones de nómina**.</span><span class="sxs-lookup"><span data-stu-id="56435-110">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span>
3. <span data-ttu-id="56435-111">En la ventana **Importar**, seleccione el archivo de nómina correspondiente y, a continuación, elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="56435-111">In the **Import** window, select the relevant payroll file, and then choose the **OK** button.</span></span> <span data-ttu-id="56435-112">El archivo tiene que estar en formato CSV.</span><span class="sxs-lookup"><span data-stu-id="56435-112">The file must be in CSV format.</span></span> 
4. <span data-ttu-id="56435-113">Siga los pasos de la ventana **Importar transacciones de nómina** para importar transacciones y asignar las cuentas y, a continuación, elija el botón **Terminar**.</span><span class="sxs-lookup"><span data-stu-id="56435-113">Follow the steps in the **Import Payroll Transactions** window to import transactions and map accounts, and then choose the **Finish** button.</span></span>

    <span data-ttu-id="56435-114">El diario general se rellena con líneas que representan las transacciones que contiene el archivo de nóminas y con las cuentas relevantes de la columna **Cuenta**.</span><span class="sxs-lookup"><span data-stu-id="56435-114">The general journal is filled with lines representing the transactions that the payroll file contains and with the relevant accounts in the **G/L Account** column.</span></span>
4. <span data-ttu-id="56435-115">Edite o registre las líneas de diario como cualquier otra transacción de contabilidad.</span><span class="sxs-lookup"><span data-stu-id="56435-115">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="56435-116">Para obtener más información sobre cómo trabajar con el formulario, consulte [Trabajar con diarios generales](ui-work-general-journals.md).</span><span class="sxs-lookup"><span data-stu-id="56435-116">For more information, see [How to: Work With General Journals](ui-work-general-journals.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="56435-117">Consulte también</span><span class="sxs-lookup"><span data-stu-id="56435-117">See Also</span></span>
[<span data-ttu-id="56435-118">Finanzas</span><span class="sxs-lookup"><span data-stu-id="56435-118">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="56435-119">Procedimiento: trabajar con diarios generales</span><span class="sxs-lookup"><span data-stu-id="56435-119">How to: Work With General Journals</span></span>](ui-work-general-journals.md)  

