---
title: "Procedimiento para generar facturas electrónicas"
description: "Después de registrar una factura de venta en [!INCLUDE[navnow](../../includes/navnow_md.md)], debe generar una factura electrónica que se enviará al cliente. Asimismo, puede exportar dicha factura electrónica como un archivo XML, que puede guardar en una ubicación especificada."
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
ms.openlocfilehash: c5a242a8b51cd343870151bab0383aa17f3ba8c8
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-generate-electronic-invoices"></a><span data-ttu-id="2518b-104">Procedimiento: Generar facturas electrónicas</span><span class="sxs-lookup"><span data-stu-id="2518b-104">How to: Generate Electronic Invoices</span></span>
<span data-ttu-id="2518b-105">Después de registrar una factura de venta en [!INCLUDE[navnow](../../includes/navnow_md.md)], debe generar una factura electrónica que se enviará al cliente.</span><span class="sxs-lookup"><span data-stu-id="2518b-105">In [!INCLUDE[navnow](../../includes/navnow_md.md)], after you post a sales invoice you must generate an electronic invoice that will be sent to the customer.</span></span> <span data-ttu-id="2518b-106">Asimismo, puede exportar dicha factura electrónica como un archivo XML, que puede guardar en una ubicación especificada.</span><span class="sxs-lookup"><span data-stu-id="2518b-106">You can also export the electronic invoice as an XML file, which you can save to a specified location.</span></span>  
  
 <span data-ttu-id="2518b-107">En el procedimiento siguiente se describe cómo generar facturas electrónicas para facturas de venta, aunque los mismos pasos también se aplican a facturas y notas de crédito de servicios.</span><span class="sxs-lookup"><span data-stu-id="2518b-107">The following procedure describes how to generate electronic invoices for sales invoices, but the same steps also apply to service invoices and credit memos.</span></span>  
  
### <a name="to-generate-electronic-invoices-for-sales-invoices"></a><span data-ttu-id="2518b-108">Para generar facturas electrónicas de facturas de ventas</span><span class="sxs-lookup"><span data-stu-id="2518b-108">To generate electronic invoices for sales invoices</span></span>  
  
1.  <span data-ttu-id="2518b-109">Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Factura venta reg.** y, a continuación, elija el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="2518b-109">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Posted Sales Invoice**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="2518b-110">Seleccione la factura registrada.</span><span class="sxs-lookup"><span data-stu-id="2518b-110">Select the posted invoice.</span></span>  
  
3.  <span data-ttu-id="2518b-111">En la pestaña **Acciones**, del grupo **Funciones**, seleccione **Send Electronic Document**.</span><span class="sxs-lookup"><span data-stu-id="2518b-111">On the **Actions** tab, in the **Functions** group, choose **Send Electronic Document**.</span></span> <span data-ttu-id="2518b-112">De este modo, se enviará un correo electrónico al cliente con la factura electrónica adjuntada como archivo XML.</span><span class="sxs-lookup"><span data-stu-id="2518b-112">An email will be sent to the customer with the electronic invoice attached as an XML file.</span></span> <span data-ttu-id="2518b-113">Si seleccionó el campo **Enviar informe PDF** de la ventana **Configuración de contabilidad**, también se incluirá un documento PDF con el archivo XML.</span><span class="sxs-lookup"><span data-stu-id="2518b-113">If you selected the **Send PDF Report** field in the **General Ledger Setup** window, a PDF will be included with the XML file.</span></span>  
  
4.  <span data-ttu-id="2518b-114">Como alternativa, vaya a la pestaña **Acciones**, del grupo **Funciones**, y seleccione **Exportar documento electrónico como XML**.</span><span class="sxs-lookup"><span data-stu-id="2518b-114">Optionally, on the **Actions** tab, in the **Functions** group, choose **Export E-Document as XML**.</span></span> <span data-ttu-id="2518b-115">Seleccione la ubicación donde desea guardar la factura electrónica como archivo XML.</span><span class="sxs-lookup"><span data-stu-id="2518b-115">Select the location where you want to save the electronic invoice as an XML file.</span></span>  
  
     <span data-ttu-id="2518b-116">Para comprobar la actividad de facturas electrónicas, en la ventana **Factura venta reg.**, en la ficha desplegable **Facturación**, se actualizarán los campos **Documento electrónico enviado** y **No. of E-Document Submissions**.</span><span class="sxs-lookup"><span data-stu-id="2518b-116">To verify the electronic invoice activity, in the **Posted Sales Invoice** window, on the **Invoicing** FastTab, the **Electronic Document Sent** and **No. of E-Document Submissions** fields will be updated.</span></span>  
  
> [!NOTE]  
>  <span data-ttu-id="2518b-117">ADD INCLUDE<!--[!INCLUDE[bp_refimplementation](../../includes/bp_refimplementation_md.md)]--></span><span class="sxs-lookup"><span data-stu-id="2518b-117">ADD INCLUDE<!--[!INCLUDE[bp_refimplementation](../../includes/bp_refimplementation_md.md)]--></span></span>  
  
## <a name="see-also"></a><span data-ttu-id="2518b-118">Consulte también</span><span class="sxs-lookup"><span data-stu-id="2518b-118">See Also</span></span>  
 <span data-ttu-id="2518b-119">[Procedimiento: Configurar la facturación electrónica](how-to-set-up-electronic-invoicing.md) </span><span class="sxs-lookup"><span data-stu-id="2518b-119">[How to: Set Up Electronic Invoicing](how-to-set-up-electronic-invoicing.md) </span></span>  
 <span data-ttu-id="2518b-120">[Facturación electrónica](electronic-invoicing.md) </span><span class="sxs-lookup"><span data-stu-id="2518b-120">[Electronic Invoicing](electronic-invoicing.md) </span></span>  
 <span data-ttu-id="2518b-121">Factura venta reg.</span><span class="sxs-lookup"><span data-stu-id="2518b-121">Posted Sales Invoice</span></span>   
 <span data-ttu-id="2518b-122">Configuración de contabilidad</span><span class="sxs-lookup"><span data-stu-id="2518b-122">General Ledger Setup</span></span>
