---
title: "Factura electrónica"
description: "Las empresas mexicanas deben tener la posibilidad de enviar facturas de forma electrónica como archivos de Comprobante Fiscal Digital por Internet (CFDI). [!INCLUDE[navnow](../../includes/navnow_md.md)] admite CFDI para que pueda exportar facturas de ventas y servicios, así como notas de crédito con formato de documentos electrónicos que cuenten con la firma digital requerida."
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
ms.openlocfilehash: e5b0811565f6475784b4a5d2d2b1ef67b3483b9d
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="electronic-invoicing"></a><span data-ttu-id="f6c83-104">Factura electrónica</span><span class="sxs-lookup"><span data-stu-id="f6c83-104">Electronic Invoicing</span></span>
<span data-ttu-id="f6c83-105">Las empresas mexicanas deben tener la posibilidad de enviar facturas de forma electrónica como archivos de Comprobante Fiscal Digital por Internet (CFDI).</span><span class="sxs-lookup"><span data-stu-id="f6c83-105">Mexican companies must be able to send invoices electronically as Comprobante Fiscal Digital por Internet (CFDI) files.</span></span> [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="f6c83-106"> admite CFDI para que pueda exportar facturas de ventas y servicios, así como notas de crédito con formato de documentos electrónicos que cuenten con la firma digital requerida.</span><span class="sxs-lookup"><span data-stu-id="f6c83-106"> supports CFDI so that you can export sales and service invoices and credit memos as electronic documents that have the required digital signature.</span></span>  
  
 <span data-ttu-id="f6c83-107">El archivo de CFDI es un archivo XML que incluye lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f6c83-107">The CFDI file is an XML file that contains:</span></span>  
  
-   <span data-ttu-id="f6c83-108">Nombre de la empresa emisora.</span><span class="sxs-lookup"><span data-stu-id="f6c83-108">Name of issuing company.</span></span>  
  
-   <span data-ttu-id="f6c83-109">Domicilio fiscal de la empresa emisora.</span><span class="sxs-lookup"><span data-stu-id="f6c83-109">Fiscal address of issuing company.</span></span>  
  
-   <span data-ttu-id="f6c83-110">Régimen tributario de la empresa emisora.</span><span class="sxs-lookup"><span data-stu-id="f6c83-110">Tax scheme of the issuing company.</span></span>  
  
-   <span data-ttu-id="f6c83-111">Número de registro federal de contribuyente (RFC) de la empresa emisora.</span><span class="sxs-lookup"><span data-stu-id="f6c83-111">Federal tax registration number (RFC) of issuing company.</span></span>  
  
-   <span data-ttu-id="f6c83-112">RFC de la empresa receptora.</span><span class="sxs-lookup"><span data-stu-id="f6c83-112">RFC of the receiving company.</span></span>  
  
-   <span data-ttu-id="f6c83-113">Cantidad y descripción de los bienes o servicios.</span><span class="sxs-lookup"><span data-stu-id="f6c83-113">Quantity and description of the goods or services.</span></span>  
  
-   <span data-ttu-id="f6c83-114">Precio unitario.</span><span class="sxs-lookup"><span data-stu-id="f6c83-114">Unit price.</span></span>  
  
-   <span data-ttu-id="f6c83-115">Importes de impuestos enumerados por tipo de impuesto.</span><span class="sxs-lookup"><span data-stu-id="f6c83-115">Tax amounts listed by tax type.</span></span>  
  
-   <span data-ttu-id="f6c83-116">Código de divisa.</span><span class="sxs-lookup"><span data-stu-id="f6c83-116">Currency code.</span></span>  
  
-   <span data-ttu-id="f6c83-117">Ubicación de aduana, que ../../incluye la fecha y el número del documento de la aduana, si la transacción es una importación.</span><span class="sxs-lookup"><span data-stu-id="f6c83-117">Customs location, which ../../includes the date and number of the customs document, if the transaction is an import.</span></span>  
  
-   <span data-ttu-id="f6c83-118">Sello digital de la empresa emisora, asignado por las autoridades fiscales (SAT).</span><span class="sxs-lookup"><span data-stu-id="f6c83-118">Digital stamp of the issuing company, which is assigned by the tax authorities (SAT).</span></span>  
  
-   <span data-ttu-id="f6c83-119">Sello digital de un proveedor de servicios autorizado (PAC), que usted elija.</span><span class="sxs-lookup"><span data-stu-id="f6c83-119">Digital stamp of an authorized service provider, PAC, that you choose.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="f6c83-120">Deberá enviar las facturas electrónicas a un PAC, que es un proveedor de servicios autorizado designado por las autoridades fiscales de México (SAT).</span><span class="sxs-lookup"><span data-stu-id="f6c83-120">You will be submitting the electronic invoices to a PAC, which is an authorized service provider appointed by the Mexican tax authorities (SAT).</span></span>  
  
## <a name="getting-started"></a><span data-ttu-id="f6c83-121">Introducción</span><span class="sxs-lookup"><span data-stu-id="f6c83-121">Getting Started</span></span>  
 <span data-ttu-id="f6c83-122">Antes de poder utilizar ADD INCLUDE<!--[!INCLUDE[navnow](how-to-set-up-electronic-invoicing.md).</span><span class="sxs-lookup"><span data-stu-id="f6c83-122">Before you can use ADD INCLUDE<!--[!INCLUDE[navnow](how-to-set-up-electronic-invoicing.md).</span></span> <span data-ttu-id="f6c83-123">Para obtener información sobre los certificados y las claves de SAT, consulte el sitio web del [Servicio de Administración Tributaria](http://go.microsoft.com/fwlink/?LinkId=242772).</span><span class="sxs-lookup"><span data-stu-id="f6c83-123">For information about SAT certificates and keys, see the [Servicio de Administracíon Tributaria](http://go.microsoft.com/fwlink/?LinkId=242772) website.</span></span>  
  
 <span data-ttu-id="f6c83-124">Además, debe especificar los servicios web que utilizará para comunicarse con el PAC con el fin de obtener los sellos digitales correspondientes.</span><span class="sxs-lookup"><span data-stu-id="f6c83-124">You also must specify the web services that you will use to communicate with the PAC in order to obtain digital stamps.</span></span> <span data-ttu-id="f6c83-125">Para obtener más información, consulte [Procedimiento: Configurar servicios web de PAC](how-to-set-up-pac-web-services.md).</span><span class="sxs-lookup"><span data-stu-id="f6c83-125">For more information, see [How to: Set Up PAC Web Services](how-to-set-up-pac-web-services.md).</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="f6c83-126">Tenga en cuenta que SAT ha certificado a varios PAC en México, por lo que deberá obtener la información pertinente para comunicarse con el PAC que elija.</span><span class="sxs-lookup"><span data-stu-id="f6c83-126">SAT has certified more than one PAC in Mexico, and you must obtain the appropriate information to communicate with the PAC of your choice.</span></span>  
  
## <a name="sending-electronic-invoices"></a><span data-ttu-id="f6c83-127">Envío de facturas electrónicas</span><span class="sxs-lookup"><span data-stu-id="f6c83-127">Sending Electronic Invoices</span></span>  
 <span data-ttu-id="f6c83-128">Una vez que haya registrado una factura o una nota de crédito, podrá enviarla al cliente.</span><span class="sxs-lookup"><span data-stu-id="f6c83-128">When you have posted an invoice or credit memo, you can send it to your customer.</span></span> <span data-ttu-id="f6c83-129">Pero antes debe obtener el sello digital de un PAC.</span><span class="sxs-lookup"><span data-stu-id="f6c83-129">But first you must obtain a digital stamp from a PAC.</span></span> [!INCLUDE[navnow](../../includes/navnow_md.md)]<span data-ttu-id="f6c83-130"> se comunica con el PAC a través de servicios web para solicitar un sello y, de este modo, su empresa y el PAC firman digitalmente el documento de forma automática.</span><span class="sxs-lookup"><span data-stu-id="f6c83-130"> communicates with the PAC through web services to request a stamp, and the document is automatically digitally signed by your company and the PAC.</span></span>  
  
 <span data-ttu-id="f6c83-131">Al enviar una factura o una nota de crédito al cliente, [!INCLUDE[navnow](../../includes/navnow_md.md)] utiliza la dirección de correo electrónico que se ha especificado en la ventana **Información de empresa**.</span><span class="sxs-lookup"><span data-stu-id="f6c83-131">When you send an electronic invoice or credit memo to your customer, [!INCLUDE[navnow](../../includes/navnow_md.md)] uses the email address that you have specified in the **Company Information** window.</span></span> <span data-ttu-id="f6c83-132">El documento se envía a la dirección de correo electrónico que se ha especificado en la ventana **Ficha cliente** del cliente de facturación que consta en la factura o la nota de crédito.</span><span class="sxs-lookup"><span data-stu-id="f6c83-132">The document is sent to the email address that you have specified in the **Customer Card** window for the bill-to customer on the invoice or credit memo.</span></span> <span data-ttu-id="f6c83-133">En la ventana **Configuración de contabilidad**, también puede elegir si desea incluir documentos como archivos PDF en el mensaje de correo electrónico que se envía.</span><span class="sxs-lookup"><span data-stu-id="f6c83-133">In the **General Ledger Setup** window, you also can choose to include the documents as PDF files in the email that is sent.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="f6c83-134">Los usuarios encargados de enviar las facturas electrónicas deben ser capaces de enviar correo a través del Protocolo simple de transferencia de correo (SMTP).</span><span class="sxs-lookup"><span data-stu-id="f6c83-134">The users who will send electronic invoices must be able to send mail using the Simple Mail Transfer Protocol (SMTP).</span></span> <span data-ttu-id="f6c83-135">En función de la configuración de la empresa, puede que deba conceder permisos explícitos a cada usuario y equipo correspondiente.</span><span class="sxs-lookup"><span data-stu-id="f6c83-135">Depending on the configuration in your company, you may have to grant explicit permissions to each relevant user and computer.</span></span>  
  
 <span data-ttu-id="f6c83-136">Asimismo, si desea imprimir los documentos, estos incluirán un código de barras de respuesta rápida (QR) y otra información identificatoria de la factura electrónica relacionada.</span><span class="sxs-lookup"><span data-stu-id="f6c83-136">If you also want to print the documents, the documents will include a Quick Response (QR) bar code and other information that identifies the related electronic invoice.</span></span> <span data-ttu-id="f6c83-137">Dicha información permite que un equipo informático pueda leer el documento impreso y proporciona un vínculo entre el documento electrónico y el documento impreso.</span><span class="sxs-lookup"><span data-stu-id="f6c83-137">This information makes the printed document computer-readable and provides a link between the electronic document and the printed document.</span></span>  
  
 <span data-ttu-id="f6c83-138">Para obtener más información, consulte [Procedimiento: Generar facturas electrónicas](how-to-generate-electronic-invoices.md).</span><span class="sxs-lookup"><span data-stu-id="f6c83-138">For more information, see [How to: Generate Electronic Invoices](how-to-generate-electronic-invoices.md).</span></span>  
  
## <a name="communication-component"></a><span data-ttu-id="f6c83-139">Componentes de comunicación</span><span class="sxs-lookup"><span data-stu-id="f6c83-139">Communication Component</span></span>  
 <span data-ttu-id="f6c83-140">El ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/nav_windows_md.md)]-->.</span><span class="sxs-lookup"><span data-stu-id="f6c83-140">The ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/nav_windows_md.md)]-->.</span></span> <span data-ttu-id="f6c83-141">El componente gestiona la comunicación con los servicios web del PAC y también genera los códigos QR que se incluyen en los documentos impresos.</span><span class="sxs-lookup"><span data-stu-id="f6c83-141">The component handles the communication with the PAC web services and also generates the QR codes that are included in the printed documents.</span></span> <span data-ttu-id="f6c83-142">Para consultar ejemplos sobre cómo utilizar el ensamblado Microsoft.Dynamics.NAV.MX.dll, consulte la codeunit 10145 **Admin. de facturas elect.** y la codeunit 10147 **Generador de objetos de factura electrónica**.</span><span class="sxs-lookup"><span data-stu-id="f6c83-142">For examples of how to use the Microsoft.Dynamics.NAV.MX.dll assembly, see codeunit 10145 **E-Invoice Mgt.** and codeunit 10147 **E-Invoice Object Factory**.</span></span>  
  
 <span data-ttu-id="f6c83-143">Al generar un documento electrónico para solicitar un sello, [!INCLUDE[navnow](../../includes/navnow_md.md)] crea un documento XML y lo envía al PAC para su procesamiento.</span><span class="sxs-lookup"><span data-stu-id="f6c83-143">When you generate an electronic document to request a stamp, [!INCLUDE[navnow](../../includes/navnow_md.md)] creates an XML document and sends it to the PAC for processing.</span></span> <span data-ttu-id="f6c83-144">El documento XML original incluye la misma información que el campo de cadena original que se muestra en el documento impreso.</span><span class="sxs-lookup"><span data-stu-id="f6c83-144">The original XML document contains the same information as the original string field that is shown on the printed document.</span></span> <span data-ttu-id="f6c83-145">La cadena original ../../incluye la información siguiente:</span><span class="sxs-lookup"><span data-stu-id="f6c83-145">The original string ../../includes the following information:</span></span>  
  
-   <span data-ttu-id="f6c83-146">Fecha de documento</span><span class="sxs-lookup"><span data-stu-id="f6c83-146">Document date</span></span>  
  
-   <span data-ttu-id="f6c83-147">Tipo de documento</span><span class="sxs-lookup"><span data-stu-id="f6c83-147">Document type</span></span>  
  
-   <span data-ttu-id="f6c83-148">Condiciones de pago</span><span class="sxs-lookup"><span data-stu-id="f6c83-148">Payment terms</span></span>  
  
-   <span data-ttu-id="f6c83-149">Nombre, dirección y número de registro federal de su empresa</span><span class="sxs-lookup"><span data-stu-id="f6c83-149">Name, address, and federal registration number of your company</span></span>  
  
-   <span data-ttu-id="f6c83-150">Nombre, dirección y número de registro federal del cliente</span><span class="sxs-lookup"><span data-stu-id="f6c83-150">Name, address, and federal registration number of the customer</span></span>  
  
-   <span data-ttu-id="f6c83-151">Importes y cantidades de línea</span><span class="sxs-lookup"><span data-stu-id="f6c83-151">Line amounts and quantities</span></span>  
  
 <span data-ttu-id="f6c83-152">El PAC devuelve un documento XML que incluye la cadena original y, también, ../../una sección para el sello digital.</span><span class="sxs-lookup"><span data-stu-id="f6c83-152">The PAC returns an XML document that has the original string, but this file also ../../includes a section for the digital stamp.</span></span> <span data-ttu-id="f6c83-153">En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede exportar los archivos XML de los documentos que tienen una firma digital y obtener así más detalles sobre los datos que se incluyen en cada elemento XML.</span><span class="sxs-lookup"><span data-stu-id="f6c83-153">In [!INCLUDE[navnow](../../includes/navnow_md.md)], you can export the XML files for documents that have a digital stamp and learn more about the data that goes into each XML element.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="f6c83-154">Consulte también</span><span class="sxs-lookup"><span data-stu-id="f6c83-154">See Also</span></span>  
 <span data-ttu-id="f6c83-155">[Procedimiento: Configurar la facturación electrónica](how-to-set-up-electronic-invoicing.md) </span><span class="sxs-lookup"><span data-stu-id="f6c83-155">[How to: Set Up Electronic Invoicing](how-to-set-up-electronic-invoicing.md) </span></span>  
 <span data-ttu-id="f6c83-156">[Procedimiento: Configurar servicios web de PAC](how-to-set-up-pac-web-services.md) </span><span class="sxs-lookup"><span data-stu-id="f6c83-156">[How to: Set Up PAC Web Services](how-to-set-up-pac-web-services.md) </span></span>  
 [<span data-ttu-id="f6c83-157">Procedimiento: Generar facturas electrónicas</span><span class="sxs-lookup"><span data-stu-id="f6c83-157">How to: Generate Electronic Invoices</span></span>](how-to-generate-electronic-invoices.md)
