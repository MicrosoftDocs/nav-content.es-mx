---
title: 'Procedimiento: Configurar documentos entrantes'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d55329b571e4c59d4821a86a39362ea58480b86a
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-set-up-incoming-documents"></a><span data-ttu-id="58a20-102">Procedimiento: Configurar documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="58a20-102">How to: Set Up Incoming Documents</span></span>
<span data-ttu-id="58a20-103">Si crea líneas del diario general desde registros de documentos entrantes, debe especificar en la ventana **Configuración de documentos entrantes** qué proceso y libro de diario quiere usar.</span><span class="sxs-lookup"><span data-stu-id="58a20-103">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="58a20-104">Si no desea que los usuarios creen facturas o líneas de diario general de los registros de documento entrante a menos que los documentos se aprueben primero, debe configurar a los aprobadores en la ventana **Aprobadores de documentos entrantes**.</span><span class="sxs-lookup"><span data-stu-id="58a20-104">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="58a20-105">Para convertir archivos PDF y de imágenes en documentos electrónicos que pueda convertir, por ejemplo, facturas de compra de Dynamics NAV, primero debe configurar la función OCR y habilitar el servicio.</span><span class="sxs-lookup"><span data-stu-id="58a20-105">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside Dynamics NAV, you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="58a20-106">Al configurar la función Documentos entrantes, puede usar distintas funciones para revisar recibos de gastos, gestionar tareas de OCR y convertir archivos de documentos entrantes, manual o automáticamente en los documentos pertinentes o en líneas de diario.</span><span class="sxs-lookup"><span data-stu-id="58a20-106">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="58a20-107">Los archivos externos se pueden adjuntar en cualquier etapa del proceso, incluidos los documentos registrados y los movimientos de proveedor, cliente y de contabilidad resultantes.</span><span class="sxs-lookup"><span data-stu-id="58a20-107">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="58a20-108">Para obtener más información, vea [Procedimiento: Procesar documentos entrantes](across-process-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="58a20-108">For more information, see [How to: Process Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="58a20-109">Para configurar la característica Documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="58a20-109">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="58a20-110">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de documentos entrantes** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="58a20-110">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="58a20-111">Rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="58a20-111">Fill in the fields as necessary.</span></span> <span data-ttu-id="58a20-112">Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.</span><span class="sxs-lookup"><span data-stu-id="58a20-112">Choose a field to read a short description of the field or link to more information.</span></span>

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="58a20-113">Para configurar aprobadores de registros de documento entrante</span><span class="sxs-lookup"><span data-stu-id="58a20-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="58a20-114">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de documentos entrantes** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="58a20-114">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="58a20-115">En la ventana **Configuración de documentos entrantes**, seleccione la opción **Aprobadores**.</span><span class="sxs-lookup"><span data-stu-id="58a20-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="58a20-116">La ventana **Aprobadores de documentos entrantes** muestra todos los usuarios configurados en Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="58a20-116">The **Incoming Document Approvers** window shows all users that are set up in your Dynamics NAV .</span></span>  
3. <span data-ttu-id="58a20-117">Seleccione uno o más usuarios que pueden aprobar un documento entrante para que un documento o una línea de diario relacionado se pueda crear.</span><span class="sxs-lookup"><span data-stu-id="58a20-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="58a20-118">Cuando se hayan configurado los aprobadores en la ventana **Aprobadores de documentos entrantes**, solo estos usuarios pueden aprobar un documento entrante si la casilla **Requerir aprobación para crear** de la ventana **Configuración de documentos entrantes** está marcada.</span><span class="sxs-lookup"><span data-stu-id="58a20-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

<span data-ttu-id="58a20-119">**Nota**: Esta configuración de aprobación no está relacionada con flujos de trabajo de aprobación.</span><span class="sxs-lookup"><span data-stu-id="58a20-119">**Note**: This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="58a20-120">Para obtener más información, consulte [Procedimiento: Usar flujos de trabajo de aprobación](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="58a20-120">For more information, see [How to: Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="58a20-121">Para configurar un servicio de OCR</span><span class="sxs-lookup"><span data-stu-id="58a20-121">To set up an OCR service</span></span>
1. <span data-ttu-id="58a20-122">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración del servicio OCR** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="58a20-122">In the top right corner, choose the **Search for Page or Report** icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="58a20-123">Rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="58a20-123">Fill in the fields as necessary.</span></span> <span data-ttu-id="58a20-124">Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.</span><span class="sxs-lookup"><span data-stu-id="58a20-124">Choose a field to read a short description of the field or link to more information.</span></span>


## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="58a20-125">Para cifrar la información de inicio de sesión</span><span class="sxs-lookup"><span data-stu-id="58a20-125">To encrypt your login information</span></span>
<span data-ttu-id="58a20-126">Se recomienda usar esta función para proteger la información de inicio de sesión que se introduce en la ventana **Configuración del servicio OCR**.</span><span class="sxs-lookup"><span data-stu-id="58a20-126">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="58a20-127">Puede cifrar datos en el servidor generando claves de cifrado nuevas o importando claves existentes que se activarán en la instancia del servidor que conecta con la base de datos.</span><span class="sxs-lookup"><span data-stu-id="58a20-127">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="58a20-128">En la ventana **Configuración del servicio OCR**, seleccione la acción **Administración del cifrado**.</span><span class="sxs-lookup"><span data-stu-id="58a20-128">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="58a20-129">En la ventana **Administración del cifrado de datos**, habilite el cifrado de los datos.</span><span class="sxs-lookup"><span data-stu-id="58a20-129">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="58a20-130">Consulte también</span><span class="sxs-lookup"><span data-stu-id="58a20-130">See Also</span></span>  
[<span data-ttu-id="58a20-131">Procesar documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="58a20-131">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="58a20-132">Documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="58a20-132">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="58a20-133">Gestionar compras</span><span class="sxs-lookup"><span data-stu-id="58a20-133">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="58a20-134">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="58a20-134">Work With Dynamics NAV</span></span>](ui-work-product.md)

