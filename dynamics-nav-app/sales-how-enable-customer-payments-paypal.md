---
title: 'Procedimiento: Permitir los pagos de clientes mediante PayPal'
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
ms.openlocfilehash: a2268d8454af761c40b11d89b01778a3f92090fb
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a>Procedimiento: Permitir los pagos de clientes mediante PayPal#
Como alternativa a recopilar pagos a través de la transferencia bancaria o las tarjetas de crédito, puede ofrecer a sus clientes la opción de pagar a través de su cuenta de PayPal.

Cuando un cliente elige el vínculo de PayPal en una factura de ventas o un documento de orden de venta, aparece la página de servicio de su cuenta de PayPal y muestra los detalles del pago de la venta. El cliente podrá pagar la factura como cualquier otro pago de PayPal.

Para activar los pagos del cliente con PayPal, deberá seguir los pasos siguientes:

1. Configure Estándar de pagos de PayPal como un servicio de pago en la ventana **Servicios de pago**.
2. Seleccione Estándar de pagos de PayPal en el campo **Servicio de pago** en el documento de ventas en cuestión.

El servicio Estándar de pagos de PayPal se instala como una extensión de Dynamics NAV y ya está listo para usarse. Para obtener más información, vea [Personalización de Dynamics NAV usando extensiones](ui-extensions.md).

## <a name="to-enable-the-paypal-payments-standard-service"></a>Para habilitar el servicio Estándar de pagos de PayPal
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Servicios de pago** y, a continuación, seleccione el enlace relacionado.  
2. En la ventana **Servicios de pago**, seleccione la acción **Nuevo**.
3. Seleccione **Estándar de PayPal** y, a continuación, cierre la ventana.
4. En la ventana **Servicios de pago**, seleccione la acción **Configuración**.
5. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

    **Nota**: Marque la casilla **Incluir siempre en documentos** si el hipervínculo del servicio de pago de PayPal siempre debe estar visible en los documentos de ventas en que esté habilitado el pago a través de PayPal.

6. Cierre la ventana.

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a>Para seleccionar Estándar de pagos de PayPal en una factura de ventas
1. En la página Inicio, seleccione **Facturas de ventas**.
2. Abra la factura de ventas para la que desea activar los pagos de PayPal.
3. En el campo **Servicio de pago**, seleccione Estándar de pagos de PayPal.

**Nota**: El campo **Servicio de pago** solo está disponible si el servicio Estándar de pagos de PayPal está activado.   

## <a name="see-also"></a>Consulte también  
[Configurar ventas](sales-setup-sales.md)  
[Gestionar ventas](sales-manage-sales.md)  
[Personalizar Dynamics NAV usando extensiones](ui-extensions.md)

