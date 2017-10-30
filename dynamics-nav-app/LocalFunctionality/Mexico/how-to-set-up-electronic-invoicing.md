---
title: "Procedimiento para configurar la facturación electrónica"
description: "Para poder enviar documentos electrónicos, primero debe configurar [!INCLUDE[navnow](../../includes/navnow_md.md)] para asegurarse de que el número de identificación fiscal (RFC), el número de identificación personal (CURP) y los identificadores de inscripción estatal estén disponibles para la empresa y para todos sus clientes y proveedores. Además, debe configurar los parámetros necesarios para el envío de facturas electrónicas a clientes y proveedores. Tales parámetros incluyen la huella digital del certificado, es decir, el certificado que recibe de la autoridad fiscal mexicana (SAT)."
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
ms.openlocfilehash: a2a53c8143bf6c5c98686d8d4d2261e34221345f
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-electronic-invoicing"></a><span data-ttu-id="1d0f9-105">Procedimiento: Configurar la facturación electrónica</span><span class="sxs-lookup"><span data-stu-id="1d0f9-105">How to: Set Up Electronic Invoicing</span></span>
<span data-ttu-id="1d0f9-106">Para poder enviar documentos electrónicos, primero debe configurar [!INCLUDE[navnow](../../includes/navnow_md.md)] para asegurarse de que el número de identificación fiscal (RFC), el número de identificación personal (CURP) y los identificadores de inscripción estatal estén disponibles para la empresa y para todos sus clientes y proveedores.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-106">Before you can send electronic documents, you must set up [!INCLUDE[navnow](../../includes/navnow_md.md)] to ensure that the tax identification number (RFC), personal identification number (CURP), and state inscription IDs are available for your company and all your customers and vendors.</span></span> <span data-ttu-id="1d0f9-107">Además, debe configurar los parámetros necesarios para el envío de facturas electrónicas a clientes y proveedores.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-107">You also need to set up the parameters that are needed for sending electronic invoices to customers and vendors.</span></span> <span data-ttu-id="1d0f9-108">Tales parámetros incluyen la huella digital del certificado, es decir, el certificado que recibe de la autoridad fiscal mexicana (SAT).</span><span class="sxs-lookup"><span data-stu-id="1d0f9-108">These parameters include the certificate thumbprint, which is the certificate that you received from the Mexico tax authority (SAT).</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="1d0f9-109">El certificado que recibe de la autoridad fiscal mexicana debe instalarse para cada usuario que envía facturas electrónicas.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-109">The certificate that you received from the Mexico tax authority must be installed for each user who sends electronic invoices.</span></span> <span data-ttu-id="1d0f9-110">Para obtener más información, consulte el sitio web del [Servicio de Administración Tributaria](http://go.microsoft.com/fwlink/?LinkId=242772).</span><span class="sxs-lookup"><span data-stu-id="1d0f9-110">For more information, see the [Servicio de Administracíon Tributaria](http://go.microsoft.com/fwlink/?LinkId=242772) website.</span></span>  
>   
>  <span data-ttu-id="1d0f9-111">Asimismo, la empresa debe tener configurado el correo SMTP para el envío de facturas electrónicas.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-111">Your company must also have SMTP mail set up for emailing electronic invoices.</span></span> <span data-ttu-id="1d0f9-112">En función de la configuración de la empresa, quizá sea necesario conceder permisos explícitos de SMTP a cada usuario y equipo correspondiente.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-112">Depending on the configuration in your company, you may need to grant explicit SMTP permissions to each relevant user and computer.</span></span> <span data-ttu-id="1d0f9-113">Los documentos se enviarán desde la dirección especificada en la ventana **Información de empresa**.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-113">The documents will be sent from the address that is specified in the **Company Information** window.</span></span>  
  
### <a name="to-set-up-company-information"></a><span data-ttu-id="1d0f9-114">Para configurar la información de la empresa</span><span class="sxs-lookup"><span data-stu-id="1d0f9-114">To set up company information</span></span>  
  
1.  <span data-ttu-id="1d0f9-115">Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Información de la empresa** y, a continuación, seleccione el vínculo relacionado.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Company Information**, and then choose the related link.</span></span>  
  
2.  <span data-ttu-id="1d0f9-116">En la ventana **Información de empresa**, en la ficha desplegable **Impuesto**, rellene los campos tal como se describe en la tabla siguiente.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-116">In the **Company Information** window, on the **Tax** FastTab, fill in the fields as described in the following table.</span></span>  
  
    |<span data-ttu-id="1d0f9-117">Campo</span><span class="sxs-lookup"><span data-stu-id="1d0f9-117">Field</span></span>|<span data-ttu-id="1d0f9-118">Descripción</span><span class="sxs-lookup"><span data-stu-id="1d0f9-118">Description</span></span>|  
    |---
    <span data-ttu-id="1d0f9-119">title: Procedimiento para configurar la facturación electrónica description: Para poder enviar documentos electrónicos, primero debe configurar [!INCLUDE[navnow](../../includes/navnow_md.md)] para asegurarse de que el número de identificación fiscal (RFC), el número de identificación personal (CURP) y los identificadores de inscripción estatal estén disponibles para la empresa y para todos sus clientes y proveedores.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-119">title: How to Set Up Electronic Invoicing description: Before you can send electronic documents, you must set up [!INCLUDE[navnow](../../includes/navnow_md.md)] to ensure that the tax identification number (RFC), personal identification number (CURP), and state inscription IDs are available for your company and all your customers and vendors.</span></span> <span data-ttu-id="1d0f9-120">Además, debe configurar los parámetros necesarios para el envío de facturas electrónicas a clientes y proveedores.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-120">You also need to set up the parameters that are needed for sending electronic invoices to customers and vendors.</span></span> <span data-ttu-id="1d0f9-121">Tales parámetros incluyen la huella digital del certificado, es decir, el certificado que recibe de la autoridad fiscal mexicana (SAT).</span><span class="sxs-lookup"><span data-stu-id="1d0f9-121">These parameters include the certificate thumbprint, which is the certificate that you received from the Mexico tax authority (SAT).</span></span>
    
    <span data-ttu-id="1d0f9-122">documentationcenter: '' author: SorenGP</span><span class="sxs-lookup"><span data-stu-id="1d0f9-122">documentationcenter: '' author: SorenGP</span></span>

    <span data-ttu-id="1d0f9-123">ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe</span><span class="sxs-lookup"><span data-stu-id="1d0f9-123">ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe</span></span>

------
    title: How to Set Up Electronic Invoicing 
    description: Before you can send electronic documents, you must set up [!INCLUDE[navnow](../../includes/navnow_md.md)] to ensure that the tax identification number (RFC), personal identification number (CURP), and state inscription IDs are available for your company and all your customers and vendors. You also need to set up the parameters that are needed for sending electronic invoices to customers and vendors. These parameters include the certificate thumbprint, which is the certificate that you received from the Mexico tax authority (SAT).
    
    documentationcenter: ''
    author: SorenGP

    ms.prod: "dynamics-nav-2017"
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 07/01/2017
    ms.author: sgroespe

------
    title: How to Set Up Electronic Invoicing 
    description: Before you can send electronic documents, you must set up [!INCLUDE[navnow](../../includes/navnow_md.md)] to ensure that the tax identification number (RFC), personal identification number (CURP), and state inscription IDs are available for your company and all your customers and vendors. You also need to set up the parameters that are needed for sending electronic invoices to customers and vendors. These parameters include the certificate thumbprint, which is the certificate that you received from the Mexico tax authority (SAT).
    
    documentationcenter: ''
    author: SorenGP

    ms.prod: "dynamics-nav-2017"
    ms.topic: article
    ms.devlang: na
    ms.tgt_pltfrm: na
    ms.workload: na
    ms.search.keywords:
    ms.date: 07/01/2017
    ms.author: sgroespe

---------------------------------|---------------------------------------|  
    <span data-ttu-id="1d0f9-124">|**Huella digital de certificado del SAT**|Especifique el nombre descriptivo del certificado que desea usar para la emisión de facturas electrónicas.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-124">|**SAT Certificate Thumbprint**|Enter the friendly name of the certificate that you want to use for issuing electronic invoices.</span></span> <span data-ttu-id="1d0f9-125">**Nota:** Se necesita un certificado para cada usuario que envía facturas electrónicas.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-125">**Note:**  A certificate is needed for each user who sends electronic invoices.</span></span> <span data-ttu-id="1d0f9-126">Para obtener la huella digital del certificado, consulte la Ayuda del sistema operativo.|</span><span class="sxs-lookup"><span data-stu-id="1d0f9-126">To get the certificate thumbprint, see the Help for the operating system.|</span></span>  
    <span data-ttu-id="1d0f9-127">|**Enviar informe PDF**|Seleccione esta opción para incluir un archivo PDF al enviar facturas electrónicas por correo electrónica a los clientes y los proveedores.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-127">|**Send PDF Report**|Select to include a PDF when you email electronic invoices to customers or vendors.</span></span> <span data-ttu-id="1d0f9-128">Las facturas electrónicas siempre se envían como archivo XML. Esta opción permite incluir un documento PDF junto con dicho archivo XML.|</span><span class="sxs-lookup"><span data-stu-id="1d0f9-128">Electronic invoices are always sent as an XML file, this option allows you to include a PDF with the XML file.|</span></span>  
    <span data-ttu-id="1d0f9-129">|**Código PAC**|Indique el proveedor de servicios autorizado (PAC) al que desea aplicar sellos digitales en sus facturas electrónicas.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-129">|**PAC Code**|Specify the authorized service provider, PAC, that you want apply digital stamps to your electronic invoices.</span></span> <span data-ttu-id="1d0f9-130">**Nota:** Para usar un PAC, debe configurar servicios web.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-130">**Note:**  To use a PAC, you must set up web services.</span></span> <span data-ttu-id="1d0f9-131">Para obtener más información, consulte [Procedimiento: Configurar servicios web de PAC](how-to-set-up-pac-web-services.md).|</span><span class="sxs-lookup"><span data-stu-id="1d0f9-131">For more information, see [How to: Set Up PAC Web Services](how-to-set-up-pac-web-services.md).|</span></span>  
    <span data-ttu-id="1d0f9-132">|**Entorno PAC**|Especifique si la empresa usa facturas electrónicas y si usted está usando los servicios web del proveedor de servicios autorizado (PAC) en un entorno de prueba o producción.|</span><span class="sxs-lookup"><span data-stu-id="1d0f9-132">|**PAC Environment**|Specify if your company uses electronic invoices, and if you are using the web services of your authorized service provider, PAC, in a test environment or a production environment.|</span></span>  
  
 <span data-ttu-id="1d0f9-133">Como alternativa, puede solicitar a su Microsoft Certified Partner que modifique el texto que se incluye en el correo electrónico que se usa al enviar facturas electrónicas.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-133">Optionally, you can ask your Microsoft Certified Partner to modify the text that is included in the email that is sent when you send electronic invoices.</span></span> <span data-ttu-id="1d0f9-134">El texto se almacena como variables de texto en la codeunit 10145.</span><span class="sxs-lookup"><span data-stu-id="1d0f9-134">The text is stored as text variables in codeunit 10145.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="1d0f9-135">Consulte también</span><span class="sxs-lookup"><span data-stu-id="1d0f9-135">See Also</span></span>  
 <span data-ttu-id="1d0f9-136">[Facturación electrónica](electronic-invoicing.md) </span><span class="sxs-lookup"><span data-stu-id="1d0f9-136">[Electronic Invoicing](electronic-invoicing.md) </span></span>  
 <span data-ttu-id="1d0f9-137">[Procedimiento: Generar facturas electrónicas](how-to-generate-electronic-invoices.md) </span><span class="sxs-lookup"><span data-stu-id="1d0f9-137">[How to: Generate Electronic Invoices](how-to-generate-electronic-invoices.md) </span></span>  
 <span data-ttu-id="1d0f9-138">Información empresa</span><span class="sxs-lookup"><span data-stu-id="1d0f9-138">Company Information</span></span>   
 <span data-ttu-id="1d0f9-139">Ficha cliente</span><span class="sxs-lookup"><span data-stu-id="1d0f9-139">Customer Card</span></span>   
 <span data-ttu-id="1d0f9-140">Ficha proveedor</span><span class="sxs-lookup"><span data-stu-id="1d0f9-140">Vendor Card</span></span>   
 <span data-ttu-id="1d0f9-141">Configuración de contabilidad</span><span class="sxs-lookup"><span data-stu-id="1d0f9-141">General Ledger Setup</span></span>
