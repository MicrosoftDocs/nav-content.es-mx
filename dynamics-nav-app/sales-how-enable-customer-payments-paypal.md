---
title: 'Procedimiento: Permitir los pagos de clientes mediante PayPal'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 15f30a03c3e7ccc865ef527a707794c2c6428b2f
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-enable-customer-payments-through-paypal"></a><span data-ttu-id="46cd9-102">Procedimiento: Permitir los pagos de clientes mediante PayPal#</span><span class="sxs-lookup"><span data-stu-id="46cd9-102">How to: Enable Customer Payments Through PayPal#</span></span>
<span data-ttu-id="46cd9-103">Como alternativa a recopilar pagos a través de la transferencia bancaria o las tarjetas de crédito, puede ofrecer a sus clientes la opción de pagar a través de su cuenta de PayPal.</span><span class="sxs-lookup"><span data-stu-id="46cd9-103">As an alternative to collecting payments through bank transfer or credit cards, you can offer your customers to pay you through their PayPal account.</span></span>

<span data-ttu-id="46cd9-104">Cuando un cliente elige el vínculo de PayPal en una factura de ventas o un documento de orden de venta, aparece la página de servicio de su cuenta de PayPal y muestra los detalles del pago de la venta.</span><span class="sxs-lookup"><span data-stu-id="46cd9-104">When a customer chooses the PayPal link on a sales invoice or sales order document, the service page for their PayPal account appears showing the payment details for the sale.</span></span> <span data-ttu-id="46cd9-105">El cliente podrá pagar la factura como cualquier otro pago de PayPal.</span><span class="sxs-lookup"><span data-stu-id="46cd9-105">The customer can then pay the invoice as any other PayPal payment.</span></span>

<span data-ttu-id="46cd9-106">Para activar los pagos del cliente con PayPal, deberá seguir los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="46cd9-106">To enable customer payments through PayPal, you must do the following:</span></span>

1. <span data-ttu-id="46cd9-107">Configure Estándar de pagos de PayPal como un servicio de pago en la ventana **Servicios de pago**.</span><span class="sxs-lookup"><span data-stu-id="46cd9-107">Set up PayPal Payments Standard as a payment service in the **Payments Services** window.</span></span>
2. <span data-ttu-id="46cd9-108">Seleccione Estándar de pagos de PayPal en el campo **Servicio de pago** en el documento de ventas en cuestión.</span><span class="sxs-lookup"><span data-stu-id="46cd9-108">Select PayPal Payments Standard in the **Payment Service** field on the sales document in question.</span></span>

<span data-ttu-id="46cd9-109">El servicio Estándar de pagos de PayPal se instala como una extensión de Dynamics NAV y ya está lista para usar.</span><span class="sxs-lookup"><span data-stu-id="46cd9-109">The PayPal Payments Standard service is installed as an extension to Dynamics NAV and ready to enabled.</span></span> <span data-ttu-id="46cd9-110">Para obtener más información, consulte [Personalizar Dynamics NAV mediante extensiones](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="46cd9-110">For more information, see [Customizing Dynamics NAV Using Extensions ](ui-extensions.md).</span></span>

## <a name="to-enable-the-paypal-payments-standard-service"></a><span data-ttu-id="46cd9-111">Para habilitar el servicio Estándar de pagos de PayPal</span><span class="sxs-lookup"><span data-stu-id="46cd9-111">To enable the PayPal Payments Standard service</span></span>
1. <span data-ttu-id="46cd9-112">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Servicios de pago** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="46cd9-112">In the top right corner, choose the **Search for Page or Report** icon, **Payment Services**, and then choose the related link.</span></span>  
2. <span data-ttu-id="46cd9-113">En la ventana **Servicios de pago**, seleccione la acción **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="46cd9-113">In the **Payment Services** window, choose the **New** action.</span></span>
3. <span data-ttu-id="46cd9-114">Seleccione **Estándar de PayPal** y, a continuación, cierre la ventana.</span><span class="sxs-lookup"><span data-stu-id="46cd9-114">Select **PayPal Standard**, and then close the window.</span></span>
4. <span data-ttu-id="46cd9-115">En la ventana **Servicios de pago**, seleccione la acción **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="46cd9-115">In the **Payment Services** window, choose the **Setup** action.</span></span>
5. <span data-ttu-id="46cd9-116">Rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="46cd9-116">Fill in the fields as necessary.</span></span> <span data-ttu-id="46cd9-117">Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.</span><span class="sxs-lookup"><span data-stu-id="46cd9-117">Choose a field to read a short description of the field or link to more information.</span></span>

    <span data-ttu-id="46cd9-118">**Nota**: Marque la casilla **Incluir siempre en documentos** si el hipervínculo del servicio de pago de PayPal siempre debe estar visible en los documentos de ventas en que esté habilitado el pago a través de PayPal.</span><span class="sxs-lookup"><span data-stu-id="46cd9-118">**Note**: Select the **Always Include on Documents** check box if the hyperlink for the PayPal payment service should always be visible on sales documents where payment through PayPal is enabled.</span></span>

6. <span data-ttu-id="46cd9-119">Cierre la ventana.</span><span class="sxs-lookup"><span data-stu-id="46cd9-119">Close the window.</span></span>

## <a name="to-select-paypal-payments-standard-on-a-sales-invoice"></a><span data-ttu-id="46cd9-120">Para seleccionar Estándar de pagos de PayPal en una factura de ventas</span><span class="sxs-lookup"><span data-stu-id="46cd9-120">To select PayPal Payments Standard on a sales invoice</span></span>
1. <span data-ttu-id="46cd9-121">En la página Inicio, seleccione **Facturas de ventas**.</span><span class="sxs-lookup"><span data-stu-id="46cd9-121">On the Home page, choose **Sales Invoices**.</span></span>
2. <span data-ttu-id="46cd9-122">Abra la factura de ventas para la que desea activar los pagos de PayPal.</span><span class="sxs-lookup"><span data-stu-id="46cd9-122">Open the sales invoice that you want to enable PayPal payments for.</span></span>
3. <span data-ttu-id="46cd9-123">En el campo **Servicio de pago**, seleccione Estándar de pagos de PayPal.</span><span class="sxs-lookup"><span data-stu-id="46cd9-123">In the **Payment Service** field, choose PayPal Payments Standard.</span></span>

<span data-ttu-id="46cd9-124">**Nota**: El campo **Servicio de pago** solo está disponible si el servicio Estándar de pagos de PayPal está activado.</span><span class="sxs-lookup"><span data-stu-id="46cd9-124">**Note**: The **Payment Service** field is only visible if the PayPal Payments Standard service is enabled.</span></span>   

## <a name="see-also"></a><span data-ttu-id="46cd9-125">Consulte también</span><span class="sxs-lookup"><span data-stu-id="46cd9-125">See Also</span></span>  
[<span data-ttu-id="46cd9-126">Configurar ventas</span><span class="sxs-lookup"><span data-stu-id="46cd9-126">Set Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="46cd9-127">Gestionar ventas</span><span class="sxs-lookup"><span data-stu-id="46cd9-127">Manage Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="46cd9-128">Personalizar Dynamics NAV usando extensiones</span><span class="sxs-lookup"><span data-stu-id="46cd9-128">Customizing Dynamics NAV Using Extensions</span></span>](ui-extensions.md)

