---
title: Permitir los pagos de clientes mediante servicios de pago
description: Facilite a los clientes el pago de las facturas activando los servicios de pago.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: online payment
ms.date: 07/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: a16640e014e157d4dbcaabc53d0df2d3e063f8f9
ms.openlocfilehash: f56df1759d375548b7415234c9b303a49e50687d
ms.contentlocale: es-mx
ms.lasthandoff: 10/26/2017

---
# <a name="how-to-enable-customer-payments-through-payment-services"></a>Permitir los pagos de clientes mediante servicios de pago
Como alternativa a recopilar pagos a través de transferencia bancaria o tarjetas de crédito, los clientes pueden pagarle a través de su cuenta en servicios de pago, como PayPal y WorldPay.  

Al habilitar un servicio de pago en [!INCLUDE[d365fin](includes/d365fin_md.md)], hay disponible un vínculo al servicio en los documentos de venta que envíe por correo electrónico a los clientes. Los clientes pueden utilizar el vínculo para ir al servicio de pago y pagar la factura, directamente desde el documento de venta. Si no desea incluir el vínculo, por ejemplo, si un cliente paga en efectivo, puede quitar el servicio de pago de la factura antes de registrarla.  

Las extensiones Estándar de pagos de PayPal y Estándar de pagos de WorldPay están instalados en [!INCLUDE[d365fin](includes/d365fin_md.md)] y están preparados para que los active.  

## <a name="to-enable-a-payment-service-in-included365finincludesd365finmdmd"></a>Para activar un servicio de pago en [!INCLUDE[d365fin](includes/d365fin_md.md)]
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Servicios de pago** y, a continuación, seleccione el vínculo relacionado.  
2. En la ventana **Servicios de pago**, seleccione la acción **Nuevo**.  
3. Seleccione el servicio de pago y luego cierre la ventana.  
4. En la ventana **Servicios de pago**, seleccione la acción **Configuración**.  
5. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
6. Cierre la ventana.  

## <a name="to-select-a-payment-service-on-a-sales-invoice"></a>Para seleccionar un servicio de pago en una factura de ventas
1. En la página Inicio, seleccione **Facturas de ventas**.  
2. Abra la factura de venta que desee pagar mediante el servicio de pago.  
3. En el campo **Servicio de pago**, elija el servicio de pago.  

    > [!NOTE]  
>   El campo **Servicio de pago** solo está disponible si ha activado el servicio de pago.  

## <a name="see-also"></a>Consulte también  
[Configuración de ventas](sales-setup-sales.md)  
[Ventas](sales-manage-sales.md)  
[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] usando extensiones](ui-extensions.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  

