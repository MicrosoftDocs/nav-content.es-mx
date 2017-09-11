---
title: 'Procedimiento: Crear registros de documento entrantes'
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
ms.openlocfilehash: e91c4570ff60d991974ac6afd16ba3bc3e73e44f
ms.contentlocale: es-mx
ms.lasthandoff: 07/19/2017

---

# <a name="how-to-create-incoming-document-records"></a><span data-ttu-id="15c9e-102">Procedimiento: Crear registros de documento entrantes</span><span class="sxs-lookup"><span data-stu-id="15c9e-102">How to: Create Incoming Document Records</span></span>
<span data-ttu-id="15c9e-103">En la ventana **Documentos entrantes**, puede usar distintas funciones para revisar recibos de gastos, gestionar tareas de OCR y convertir archivos de documentos entrantes, manual o automáticamente en los documentos pertinentes o en líneas de diario.</span><span class="sxs-lookup"><span data-stu-id="15c9e-103">In the **Incoming Documents** window, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="15c9e-104">Los archivos externos se pueden adjuntar en cualquier etapa del proceso, incluidos los documentos registrados y los movimientos de proveedor, cliente y de contabilidad resultantes.</span><span class="sxs-lookup"><span data-stu-id="15c9e-104">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span>

<span data-ttu-id="15c9e-105">Para registrar un documento externo en Dynamics NAV, debe crear o completar un registro de documento entrante.</span><span class="sxs-lookup"><span data-stu-id="15c9e-105">To record an external document in Dynamics NAV, you must first create or complete an incoming document record.</span></span> <span data-ttu-id="15c9e-106">Puede hacerlo manualmente o tomar una foto del documento externo y crear el registro de documento entrante con el archivo de imagen adjunto.</span><span class="sxs-lookup"><span data-stu-id="15c9e-106">You can do this manually, or you can take a photo of the external document and then create the incoming document record with the image file attached.</span></span>

<span data-ttu-id="15c9e-107">Para poder usar la función Documentos entrantes, debe realizar la configuración necesaria.</span><span class="sxs-lookup"><span data-stu-id="15c9e-107">Before you can use the Incoming Documents feature, you must perform the required setup.</span></span> <span data-ttu-id="15c9e-108">Para obtener más información, vea [Procedimiento: Configurar documentos entrantes](across-how-setup-income-documents.md).</span><span class="sxs-lookup"><span data-stu-id="15c9e-108">For more information, see [How to: Set Up Incoming Documents](across-how-setup-income-documents.md).</span></span>

## <a name="to-approve-or-reject-an-incoming-document"></a><span data-ttu-id="15c9e-109">Para aprobar o rechazar un documento entrante</span><span class="sxs-lookup"><span data-stu-id="15c9e-109">To approve or reject an incoming document</span></span>
<span data-ttu-id="15c9e-110">Si desea que los usuarios creen facturas o líneas de diario general a partir de los registros de documento entrante a menos que se aprueben, puede configurar aprobadores que deben aprobar los registros antes de que se puedan procesar.</span><span class="sxs-lookup"><span data-stu-id="15c9e-110">If you do want to allow users to create invoices or general journal lines from incoming document records unless they are approved, you can set up approvers who must approve the records before they can be processed.</span></span>

1. <span data-ttu-id="15c9e-111">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Documentos entrantes** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="15c9e-111">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="15c9e-112">Seleccione la línea con el documento que desea aprobar o rechazar y, a continuación, elija las acciones **Aprobar** o **Rechazar**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-112">Select the line with the document that you want to approve or reject, and then choose the **Approve** or **Reject** actions.</span></span>

<span data-ttu-id="15c9e-113">Si aprueba el registro de documento entrante, se marca la casilla **Lanzado** de la línea de documento entrante.</span><span class="sxs-lookup"><span data-stu-id="15c9e-113">If you approve the incoming document record, the **Released** check box on the incoming document line is selected.</span></span> <span data-ttu-id="15c9e-114">El usuario responsable de crear, por ejemplo, facturas de compra puede procesar el registro.</span><span class="sxs-lookup"><span data-stu-id="15c9e-114">The user in charge of creating, for example, purchase invoices can proceed to process the record.</span></span>

## <a name="to-create-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="15c9e-115">Para crear un registro de documento entrante tomando una foto</span><span class="sxs-lookup"><span data-stu-id="15c9e-115">To create an incoming document record by taking a photo</span></span>
<span data-ttu-id="15c9e-116">**Nota**: El procedimiento siguiente solo se aplica a los clientes de teléfonos y tabletas de Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="15c9e-116">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="15c9e-117">En la barra de aplicaciones, seleccione el mosaico **Crear documento entrante desde la cámara** y, a continuación, vaya al paso 4.</span><span class="sxs-lookup"><span data-stu-id="15c9e-117">On the app bar, choose the **Create Incoming Document from Camera** tile, and then go to step 4.</span></span>
2. <span data-ttu-id="15c9e-118">O bien, en la barra de aplicaciones, seleccione el botón de opciones, elija **Documentos entrantes** y, a continuación, elija **Todo**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-118">Alternatively, on the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
3. <span data-ttu-id="15c9e-119">En la ventana **Documentos entrantes**, elija el botón de puntos suspensivos y seleccione **Crear desde la cámara**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-119">In the **Incoming Documents** window, choose the ellipsis button, and then choose **Create from Camera**.</span></span> <span data-ttu-id="15c9e-120">La cámara de la tableta o del teléfono se activará.</span><span class="sxs-lookup"><span data-stu-id="15c9e-120">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="15c9e-121">Tome una foto de un documento, como una recepción de compra, que desee procesar como documento entrante y, a continuación, elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-121">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="15c9e-122">Se crea un nuevo registro de documento entrante con la imagen adjunta.</span><span class="sxs-lookup"><span data-stu-id="15c9e-122">A new incoming document record is created, with the image attached.</span></span>

## <a name="to-attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a><span data-ttu-id="15c9e-123">Para a adjuntar una imagen un registro de documento entrante tomando una foto</span><span class="sxs-lookup"><span data-stu-id="15c9e-123">To attach an image to an incoming document record by taking a photo</span></span>
<span data-ttu-id="15c9e-124">**Nota**: El procedimiento siguiente solo se aplica a los clientes de teléfonos y tabletas de Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="15c9e-124">**Note**: The following procedure only applies to the Dynamics NAV Tablet and Phone clients.</span></span>

1. <span data-ttu-id="15c9e-125">En la barra de aplicaciones, elija el botón opciones, seleccione **Documentos entrantes** y, a continuación, elija **Todo**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-125">On the app bar, choose the options button, choose **Incoming Documents**, and then choose **All**.</span></span>
2. <span data-ttu-id="15c9e-126">Abra la ficha de un registro entrante de documento entrante existente.</span><span class="sxs-lookup"><span data-stu-id="15c9e-126">Open the card for an existing incoming document record.</span></span>
3. <span data-ttu-id="15c9e-127">En la ventana **Documento entrante**, elija el botón de puntos suspensivos y seleccione **Adjuntar imagen desde la cámara**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-127">In the **Incoming Document** window, choose the ellipsis button, and then choose **Attach Image from Camera**.</span></span> <span data-ttu-id="15c9e-128">La cámara de la tableta o del teléfono se activará.</span><span class="sxs-lookup"><span data-stu-id="15c9e-128">The camera on the tablet or phone is activated.</span></span>
4. <span data-ttu-id="15c9e-129">Tome una foto de un documento, como una recepción de compra, que desee procesar como documento entrante y, a continuación, elija el botón **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-129">Take a photo of a document, such as a purchase receipt, that you want to process as an incoming document, and then choose the **OK** button.</span></span>

<span data-ttu-id="15c9e-130">La imagen se adjunta al registro de documento entrante.</span><span class="sxs-lookup"><span data-stu-id="15c9e-130">The image is attached to the incoming document record.</span></span>

## <a name="to-create-an-incoming-document-record-manually"></a><span data-ttu-id="15c9e-131">Para crear un registro de documento entrante manualmente</span><span class="sxs-lookup"><span data-stu-id="15c9e-131">To create an incoming document record manually</span></span>
1. <span data-ttu-id="15c9e-132">En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Documentos entrantes** y, a continuación, seleccione el enlace relacionado.</span><span class="sxs-lookup"><span data-stu-id="15c9e-132">In the top right corner, choose the **Search for Page or Report** icon, enter **Incoming Documents**, and then choose the related link.</span></span>
2. <span data-ttu-id="15c9e-133">Elija la acción **Crear desde archivo**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-133">Choose the **Create from File** action.</span></span>  
3. <span data-ttu-id="15c9e-134">En la ventana **Insertar archivo**, seleccione un archivo y, a continuación, elija **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-134">In the **Insert File** window, select a file, and then choose **Open**.</span></span>

    <span data-ttu-id="15c9e-135">El campo se adjunta automáticamente.</span><span class="sxs-lookup"><span data-stu-id="15c9e-135">The file is automatically attached.</span></span>
4. <span data-ttu-id="15c9e-136">De forma alternativa, elija la acción **Nuevo**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-136">Alternatively, choose the **New** action.</span></span>
5. <span data-ttu-id="15c9e-137">Para adjuntar un archivo, elija la acción **Adjuntar archivo**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-137">To attach a file, choose the **Attach File** action.</span></span>
6. <span data-ttu-id="15c9e-138">En la ventana **Insertar archivo**, seleccione el archivo que representa el documento entrante en cuestión y, a continuación, elija el botón **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="15c9e-138">In the **Insert File** window, select the file that represents the incoming document in question, and then choose the **Open** button.</span></span>
7. <span data-ttu-id="15c9e-139">En la ventana **Documento entrante**, rellene los campos según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="15c9e-139">In the **Incoming Document** window, fill in the fields as necessary.</span></span> <span data-ttu-id="15c9e-140">Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.</span><span class="sxs-lookup"><span data-stu-id="15c9e-140">Choose a field to read a short description of the field or link to more information.</span></span>

##<a name="see-also"></a><span data-ttu-id="15c9e-141">Consulte también</span><span class="sxs-lookup"><span data-stu-id="15c9e-141">See Also</span></span>  
[<span data-ttu-id="15c9e-142">Procesar documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="15c9e-142">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="15c9e-143">Documentos entrantes</span><span class="sxs-lookup"><span data-stu-id="15c9e-143">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="15c9e-144">Gestionar compras</span><span class="sxs-lookup"><span data-stu-id="15c9e-144">Manage Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="15c9e-145">Trabajar con Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="15c9e-145">Work With Dynamics NAV</span></span>](ui-work-product.md)

