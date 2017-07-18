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

# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a>Impuesto sobre bienes y servicios e impuesto de ventas en Canadá
En Canadá, cuando un proveedor no tiene una empresa física en la provincia en la que se realizan las compras, el proveedor solo aplicará el impuesto sobre bienes y servicios (GST) y el impuesto armonizado de ventas (HST). Sin embargo, si la provincia tiene un impuesto de ventas provincial (PST), el comprador debe calcular el PST y pagarlo directamente a la provincia. Cuando se selecciona un código de área del impuesto provincial, Dynamics NAV lo usa para calcular el PST y registrarlo para que haya una deuda tributaria tanto en los registros del libro mayor como en los de los movimientos de impuestos. Por lo tanto, el código de área de impuesto seleccionado aquí debe ser uno en el que esté incluido únicamente el PST, no el GST.  
Para obtener más información acerca del impuesto de ventas, consulte [Impuesto de ventas y grupos de impuestos en EE. UU. y Canadá](us-finance-setup-sales-tax.md).  

## <a name="submitting-the-gsthst-file"></a>Enviar el archivo de GST o HST
La información de impuestos en documentos de compra se usa para generar una transferencia de archivos de Internet de GST o HST que debe proporcionarlo a las autoridades fiscales. Este campo incluye el impuesto sobre bienes y servicios (GST) y el impuesto armonizado de ventas (HST). El archivo se crea en el formato .tax, que se puede transferir a través de Internet.  

## <a name="see-also"></a>Consulte también
[Finanzas](finance-setup.md)  
[Configurar finanzas](finance-setup-setup-finance-setup.md)  
[Impuesto de ventas y grupos de impuestos en EE. UU. y Canadá](us-finance-setup-sales-tax.md)

