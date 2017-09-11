---
title: "Impuesto sobre bienes y servicios e impuesto de ventas en Canadá"
author: edupont04
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: c032a02b545441b927ef5c4facc9f77731f37ab7
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a><span data-ttu-id="0632a-102">Impuesto sobre bienes y servicios e impuesto de ventas en Canadá</span><span class="sxs-lookup"><span data-stu-id="0632a-102">Sales Tax and Goods and Services Tax in Canada</span></span>
<span data-ttu-id="0632a-103">En Canadá, cuando un proveedor no tiene una empresa física en la provincia en la que se realizan las compras, el proveedor solo aplicará el impuesto sobre bienes y servicios (GST) y el impuesto armonizado de ventas (HST).</span><span class="sxs-lookup"><span data-stu-id="0632a-103">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="0632a-104">Sin embargo, si la provincia tiene un impuesto de ventas provincial (PST), el comprador debe calcular el PST y pagarlo directamente a la provincia.</span><span class="sxs-lookup"><span data-stu-id="0632a-104">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="0632a-105">Cuando se selecciona un código de área del impuesto provincial, Dynamics NAV lo usa para calcular el PST y registrarlo para que haya una deuda tributaria tanto en los registros del libro mayor como en los de los movimientos de impuestos.</span><span class="sxs-lookup"><span data-stu-id="0632a-105">When a Provincial Tax Area Code is selected, Dynamics NAV uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="0632a-106">Por lo tanto, el código de área de impuesto seleccionado aquí debe ser uno en el que esté incluido únicamente el PST, no el GST.</span><span class="sxs-lookup"><span data-stu-id="0632a-106">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  
<span data-ttu-id="0632a-107">Para obtener más información acerca del impuesto de ventas, consulte [Impuesto de ventas y grupos de impuestos en EE. UU. y Canadá](us-finance-setup-sales-tax.md).</span><span class="sxs-lookup"><span data-stu-id="0632a-107">For more information about sales tax, see [Sales Tax and Tax Groups in the US and Canada](us-finance-setup-sales-tax.md).</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="0632a-108">Enviar el archivo de GST o HST</span><span class="sxs-lookup"><span data-stu-id="0632a-108">Submitting the GST/HST File</span></span>
<span data-ttu-id="0632a-109">La información de impuestos en documentos de compra se usa para generar una transferencia de archivos de Internet de GST o HST que debe proporcionarlo a las autoridades fiscales.</span><span class="sxs-lookup"><span data-stu-id="0632a-109">The tax information in purchase documents is used to generate a GST/HST internet file transfer that you must  provided to the tax authorities.</span></span> <span data-ttu-id="0632a-110">Este campo incluye el impuesto sobre bienes y servicios (GST) y el impuesto armonizado de ventas (HST).</span><span class="sxs-lookup"><span data-stu-id="0632a-110">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="0632a-111">El archivo se crea en el formato .tax, que se puede transferir a través de Internet.</span><span class="sxs-lookup"><span data-stu-id="0632a-111">The file is created in a .tax file format, which can be transferred via the internet.</span></span>  

## <a name="see-also"></a><span data-ttu-id="0632a-112">Consulte también</span><span class="sxs-lookup"><span data-stu-id="0632a-112">See Also</span></span>
[<span data-ttu-id="0632a-113">Finanzas</span><span class="sxs-lookup"><span data-stu-id="0632a-113">Finance</span></span>](finance-setup.md)  
[<span data-ttu-id="0632a-114">Configurar finanzas</span><span class="sxs-lookup"><span data-stu-id="0632a-114">Set Up Finance</span></span>](finance-setup-setup-finance-setup.md)  
[<span data-ttu-id="0632a-115">Impuesto de ventas y grupos de impuestos en EE. UU. y Canadá</span><span class="sxs-lookup"><span data-stu-id="0632a-115">Sales Tax and Tax Groups in the US and Canada</span></span>](us-finance-setup-sales-tax.md)

