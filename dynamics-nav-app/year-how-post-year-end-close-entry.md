---
title: 'Procedimiento: Registrar movimiento de cierre del ejercicio'
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: fe32ee973c90ba857852ae092acf03db09e648ee
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---
# <a name="how-to-post-year-end-closing-entry"></a><span data-ttu-id="6612f-102">Procedimiento: Registrar movimiento de cierre del ejercicio</span><span class="sxs-lookup"><span data-stu-id="6612f-102">How to: Post Year-End Closing Entry</span></span>
<span data-ttu-id="6612f-103">Como parte del cierre de los libros de un ejercicio fiscal, ejecutará el proceso Asiento regularización para transferir el resultado del año a una cuenta del balance y cerrar las cuentas de regularización.</span><span class="sxs-lookup"><span data-stu-id="6612f-103">As part of closing the books for a fiscal year, you will run the Close Income Statement batch job to transfer the year's result to an account in the balance sheet and close the income statement accounts.</span></span> <span data-ttu-id="6612f-104">Después de ejecutar el proceso Cerrar cuenta de resultado, debe abrir el diario especificado en el proceso y revisar y registrar los movimientos.</span><span class="sxs-lookup"><span data-stu-id="6612f-104">After you run the Close Income Statement batch job, you must open the journal you specified in the batch job, and then review and post the entries.</span></span>

## <a name="to-post-the-year-end-closing-entry"></a><span data-ttu-id="6612f-105">Para registrar el movimiento de cierre del ejercicio</span><span class="sxs-lookup"><span data-stu-id="6612f-105">To post the year end closing entry</span></span>
1. <span data-ttu-id="6612f-106">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="6612f-106">In the top right corner, choose the **Search for Page or Report** icon, enter **General Journal**, and then choose the related link.</span></span>
2. <span data-ttu-id="6612f-107">En la ventana **Diario general**, en el campo **Nombre de sección**, seleccione la sección que contiene los movimientos de cierre.</span><span class="sxs-lookup"><span data-stu-id="6612f-107">In the **General Journal** window, in the **Batch Name** field, select the batch that contains the closing entries.</span></span>
3. <span data-ttu-id="6612f-108">Revise los movimientos.</span><span class="sxs-lookup"><span data-stu-id="6612f-108">Review the entries.</span></span>
4. <span data-ttu-id="6612f-109">Para registrar el diario, elija la acción **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="6612f-109">To post the journal, choose the **Post** action.</span></span>

<span data-ttu-id="6612f-110">**Nota**: Si se detecta algún error, se mostrará un mensaje de error.</span><span class="sxs-lookup"><span data-stu-id="6612f-110">**Note**: If an error is detected, an error message is displayed.</span></span> <span data-ttu-id="6612f-111">Si el registro es correcto, se eliminan los movimientos registrados del diario.</span><span class="sxs-lookup"><span data-stu-id="6612f-111">If the posting is successful, the posted entries are removed from the journal.</span></span> <span data-ttu-id="6612f-112">Una vez registrados, los movimientos se registran en cada una de las cuentas de regularización, de forma que sus saldos pasan a ser cero y el resultado del año se transfiere al balance.</span><span class="sxs-lookup"><span data-stu-id="6612f-112">After posting is complete, an entry is posted to each income statement account so that its balance becomes zero and the year's result is transferred to the balance sheet.</span></span>

## <a name="see-also"></a><span data-ttu-id="6612f-113">Consulte también</span><span class="sxs-lookup"><span data-stu-id="6612f-113">See Also</span></span>
[<span data-ttu-id="6612f-114">Cerrar libros</span><span class="sxs-lookup"><span data-stu-id="6612f-114">Close Books</span></span>](year-close-books.md)  
[<span data-ttu-id="6612f-115">Asiento regularización</span><span class="sxs-lookup"><span data-stu-id="6612f-115">Close Income Statement</span></span>](year-close-income-statement.md)  
[<span data-ttu-id="6612f-116">Procedimiento para cerrar periodos contables</span><span class="sxs-lookup"><span data-stu-id="6612f-116">How to: Close Accounting Periods</span></span>](year-close-account-periods.md)  
