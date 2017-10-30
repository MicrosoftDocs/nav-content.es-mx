---
title: Usar Excel para importar datos en Dynamics NAV
description: "Utilice el paquete de configuración predeterminado para agregar datos de cliente en Excel e importar los datos en Dynamics NAV."
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migration, Excel
ms.date: 07/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: eb9b7137ee31824ba845ff336c00c6f0e59f6f5c
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="importing-data-from-legacy-accounting-software-using-a-configuration-package"></a><span data-ttu-id="42b53-103">Importar datos del software de contabilidad heredado mediante un paquete de configuración</span><span class="sxs-lookup"><span data-stu-id="42b53-103">Importing Data from Legacy Accounting Software using a Configuration Package</span></span>
<span data-ttu-id="42b53-104">Puede importar datos maestros y algunos datos transaccionales de otros sistemas de financieros mediante el paquete de configuración predeterminado en [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="42b53-104">You can import master data and some transactional data from other finance systems based on the default configuration package in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="42b53-105">En la ventana **Paquetes de configuración** puede trabajar con el paquete para importar y validar los datos antes de aplicar el paquete.</span><span class="sxs-lookup"><span data-stu-id="42b53-105">In the **Configuration Packages** window, you can work with the package to import and validate the data before you apply the package.</span></span>  

<span data-ttu-id="42b53-106">Si está familiarizado con los servicios de RapidStart para Microsoft Dynamics, también estará familiarizado con los paquetes de configuración.</span><span class="sxs-lookup"><span data-stu-id="42b53-106">If you are familiar with RapidStart Services for Microsoft Dynamics, you are also familiar with configuration packages.</span></span> <span data-ttu-id="42b53-107">El paquete de configuración predeterminado admite la mayoría de tipos de datos habituales que desea importar de un sistema heredado.</span><span class="sxs-lookup"><span data-stu-id="42b53-107">The default configuration package supports the most common types of data that you want to import from a legacy system.</span></span> <span data-ttu-id="42b53-108">En Excel, puede agregar los datos del sistema heredado y configurarlos según la lógica empresarial de [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="42b53-108">In Excel, you can then add the data from the legacy system and set it up according to the business logic of the [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

> [!TIP]  
>   <span data-ttu-id="42b53-109">Opcionalmente, utilice asistentes de migración para importar datos de QuickBooks GP o Dynamics GP.</span><span class="sxs-lookup"><span data-stu-id="42b53-109">Alternatively, use data migration wizards to import data from QuickBooks or Dynamics GP.</span></span> <span data-ttu-id="42b53-110">Para obtener más información, consulte [Migración de datos de QuickBooks](ui-extensions-quickbooks-data-migration.md) o [Migración de datos de Dynamics GP](ui-extensions-dynamicsgp-data-migration.md).</span><span class="sxs-lookup"><span data-stu-id="42b53-110">For more information, see [QuickBooks Data Migration](ui-extensions-quickbooks-data-migration.md) or [Dynamics GP Data Migration](ui-extensions-dynamicsgp-data-migration.md).</span></span>  

## <a name="working-with-data-in-excel"></a><span data-ttu-id="42b53-111">Trabajar con datos en Excel</span><span class="sxs-lookup"><span data-stu-id="42b53-111">Working with Data in Excel</span></span>
<span data-ttu-id="42b53-112">Al exportar el paquete de configuración predeterminado a Excel, el libro generado contiene una hoja de trabajo para cada tabla del paquete.</span><span class="sxs-lookup"><span data-stu-id="42b53-112">When you export the default configuration package to Excel, the generated workbook contains a worksheet for each table in the package.</span></span> <span data-ttu-id="42b53-113">Para simplificar sus tareas, puede aprovechar las herramientas de manipulación de XML que se integran en Excel.</span><span class="sxs-lookup"><span data-stu-id="42b53-113">To simplify your tasks, you can take advantage of the XML manipulation tools that are built into Excel.</span></span> <span data-ttu-id="42b53-114">También puede utilizar las funciones integradas de Excel para ayudar con el formato de datos y para colocar los datos en la celda correcta.</span><span class="sxs-lookup"><span data-stu-id="42b53-114">You can also use Excel built-in functions to help with data formatting and to put data in the correct cell.</span></span> <span data-ttu-id="42b53-115">Por ejemplo, agregue una hoja de cálculo en blanco y copie los datos heredados en ella.</span><span class="sxs-lookup"><span data-stu-id="42b53-115">For example, add a blank worksheet and copy the legacy data to it.</span></span> <span data-ttu-id="42b53-116">A continuación, cree una fórmula de Excel para asignar datos en la hoja de cálculo de transformación entre los campos en la hoja de cálculo exportada y los datos heredados del cliente.</span><span class="sxs-lookup"><span data-stu-id="42b53-116">Then make an Excel formula to map data in the transformation worksheet between the fields in the exported worksheet and customer legacy data.</span></span> <span data-ttu-id="42b53-117">Después de asignar todos los datos, copie el intervalo de datos en la hoja de cálculo de la tabla.</span><span class="sxs-lookup"><span data-stu-id="42b53-117">After you have mapped all of the data, copy the range of data onto the table worksheet.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="42b53-118">No cambie las columnas en las hojas de cálculo.</span><span class="sxs-lookup"><span data-stu-id="42b53-118">Do not change the columns in the worksheets.</span></span> <span data-ttu-id="42b53-119">Si se mueven, modifican o eliminan, la hoja de cálculo no podrá importarse a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="42b53-119">If they are moved, changed, or deleted, the worksheet cannot be imported into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

## <a name="tables-in-the-default-configuration-package"></a><span data-ttu-id="42b53-120">Tablas del paquete de configuración predeterminado</span><span class="sxs-lookup"><span data-stu-id="42b53-120">Tables in the Default Configuration Package</span></span>
<span data-ttu-id="42b53-121">El paquete de configuración predeterminado admite las tablas siguientes:</span><span class="sxs-lookup"><span data-stu-id="42b53-121">The default configuration package supports the following tables:</span></span>

-   <span data-ttu-id="42b53-122">Condiciones de pago</span><span class="sxs-lookup"><span data-stu-id="42b53-122">Payment Terms</span></span>
-   <span data-ttu-id="42b53-123">Grupo precio cliente</span><span class="sxs-lookup"><span data-stu-id="42b53-123">Customer Price Group</span></span>
-   <span data-ttu-id="42b53-124">Condiciones de envío</span><span class="sxs-lookup"><span data-stu-id="42b53-124">Shipment Method</span></span>
-   <span data-ttu-id="42b53-125">Vendedor/Comprador</span><span class="sxs-lookup"><span data-stu-id="42b53-125">Salesperson/Purchaser</span></span>
-   <span data-ttu-id="42b53-126">Lugar</span><span class="sxs-lookup"><span data-stu-id="42b53-126">Location</span></span>
-   <span data-ttu-id="42b53-127">Cuenta</span><span class="sxs-lookup"><span data-stu-id="42b53-127">GL Account</span></span>
-   <span data-ttu-id="42b53-128">Cliente</span><span class="sxs-lookup"><span data-stu-id="42b53-128">Customer</span></span>
-   <span data-ttu-id="42b53-129">Proveedor</span><span class="sxs-lookup"><span data-stu-id="42b53-129">Vendor</span></span>
-   <span data-ttu-id="42b53-130">Elemento</span><span class="sxs-lookup"><span data-stu-id="42b53-130">Item</span></span>
-   <span data-ttu-id="42b53-131">Cab. venta</span><span class="sxs-lookup"><span data-stu-id="42b53-131">Sales Header</span></span>
-   <span data-ttu-id="42b53-132">Lín. venta</span><span class="sxs-lookup"><span data-stu-id="42b53-132">Sales Line</span></span>
-   <span data-ttu-id="42b53-133">Cab. compra</span><span class="sxs-lookup"><span data-stu-id="42b53-133">Purchase Header</span></span>
-   <span data-ttu-id="42b53-134">Lín. compra</span><span class="sxs-lookup"><span data-stu-id="42b53-134">Purchase Line</span></span>
-   <span data-ttu-id="42b53-135">Lín. diario general</span><span class="sxs-lookup"><span data-stu-id="42b53-135">Gen. Journal Line</span></span>
-   <span data-ttu-id="42b53-136">Lín. diario producto</span><span class="sxs-lookup"><span data-stu-id="42b53-136">Item Journal Line</span></span>
-   <span data-ttu-id="42b53-137">Grupo contable cliente</span><span class="sxs-lookup"><span data-stu-id="42b53-137">Customer Posting Group</span></span>
-   <span data-ttu-id="42b53-138">Grupo contable proveedor</span><span class="sxs-lookup"><span data-stu-id="42b53-138">Vendor Posting Group</span></span>
-   <span data-ttu-id="42b53-139">Grupo contable inventario</span><span class="sxs-lookup"><span data-stu-id="42b53-139">Inventory Posting Group</span></span>
-   <span data-ttu-id="42b53-140">Unidad de medida</span><span class="sxs-lookup"><span data-stu-id="42b53-140">Unit of Measure</span></span>
-   <span data-ttu-id="42b53-141">Gr. contable negocio</span><span class="sxs-lookup"><span data-stu-id="42b53-141">Gen. Business Posting Group</span></span>
-   <span data-ttu-id="42b53-142">Gr. contable producto</span><span class="sxs-lookup"><span data-stu-id="42b53-142">Gen. Product Posting Group</span></span>
-   <span data-ttu-id="42b53-143">Configuración grupos contables</span><span class="sxs-lookup"><span data-stu-id="42b53-143">General Posting Setup</span></span>
-   <span data-ttu-id="42b53-144">Territorio</span><span class="sxs-lookup"><span data-stu-id="42b53-144">Territory</span></span>
-   <span data-ttu-id="42b53-145">Categoría producto</span><span class="sxs-lookup"><span data-stu-id="42b53-145">Item Category</span></span>
-   <span data-ttu-id="42b53-146">Precio venta</span><span class="sxs-lookup"><span data-stu-id="42b53-146">Sales Price</span></span>
-   <span data-ttu-id="42b53-147">Precio compra</span><span class="sxs-lookup"><span data-stu-id="42b53-147">Purchase Price</span></span>

## <a name="importing-customer-data"></a><span data-ttu-id="42b53-148">Importar datos de cliente</span><span class="sxs-lookup"><span data-stu-id="42b53-148">Importing Customer Data</span></span>
<span data-ttu-id="42b53-149">Después de que los datos del cliente se hayan introducido en Excel, importe los datos a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="42b53-149">After the customer data has been entered in Excel, you import the data into [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="42b53-150">En la ventana **Paquetes de configuración**, se importan los datos del archivo de Excel y puede validar que los datos sean coherentes con [!INCLUDE[d365fin](includes/d365fin_md.md)] antes de aplicar el paquete.</span><span class="sxs-lookup"><span data-stu-id="42b53-150">In the **Configuration Packages** window, you import the data from the Excel file, and you can validate that the data is consistent with [!INCLUDE[d365fin](includes/d365fin_md.md)] before you apply the package.</span></span>

## <a name="see-also"></a><span data-ttu-id="42b53-151">Consulte también</span><span class="sxs-lookup"><span data-stu-id="42b53-151">See Also</span></span>
[<span data-ttu-id="42b53-152">Importar datos de empresa de otros sistemas financieros</span><span class="sxs-lookup"><span data-stu-id="42b53-152">Importing Business Data from Other Finance Systems</span></span>](upload-data.md)  
[<span data-ttu-id="42b53-153">Migración de datos de QuickBooks</span><span class="sxs-lookup"><span data-stu-id="42b53-153">QuickBooks Data Migration</span></span>](ui-extensions-quickbooks-data-migration.md)  
[<span data-ttu-id="42b53-154">Migración de datos de Dynamics GP</span><span class="sxs-lookup"><span data-stu-id="42b53-154">Dynamics GP Data Migration</span></span>](ui-extensions-dynamicsgp-data-migration.md)

