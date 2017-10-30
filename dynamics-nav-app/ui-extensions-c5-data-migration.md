---
title: "Uso de la extensión de migración de datos de C5"
description: "Utilice esta extensión para migrar clientes, proveedores, productos y las cuentas de contabilidad de Microsoft Dynamics C5 2012 a Dynamics NAV."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: extension, migrate, data, C5, import
ms.date: 09/26/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2307849566a44bb49a5db6965ec3056b1a39684b
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---

# <a name="the-c5-data-migration-extension-for-dynamics-nav"></a><span data-ttu-id="70284-103">Extensión de migración de datos de C5 para Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="70284-103">The C5 Data Migration Extension for Dynamics NAV</span></span>
<span data-ttu-id="70284-104">Esta extensión facilita la migración de clientes, proveedores, productos y las cuentas de contabilidad de Microsoft Dynamics C5 2012 a [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="70284-104">This extension makes it easy to migrate customers, vendors, items, and your general ledger accounts from Microsoft Dynamcis C5 2012 to [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> 

> [!Note] 
> <span data-ttu-id="70284-105">La empresa en [!INCLUDE[d365fin](includes/d365fin_md.md)] no debe contener ningún dato.</span><span class="sxs-lookup"><span data-stu-id="70284-105">The company in [!INCLUDE[d365fin](includes/d365fin_md.md)] must not contain any data.</span></span> <span data-ttu-id="70284-106">Además, después de iniciar una migración, no debe crear clientes, proveedores, artículos ni cuentas hasta que la finalice.</span><span class="sxs-lookup"><span data-stu-id="70284-106">Additionally, after you start a migration, do not create customers, vendors, items, or accounts until the migration finishes.</span></span>

## <a name="to-migrate-data"></a><span data-ttu-id="70284-107">Para migrar datos</span><span class="sxs-lookup"><span data-stu-id="70284-107">To migrate data</span></span>
<span data-ttu-id="70284-108">Deben realizarse algunos para exportar datos de la C5 e importarlos a [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span><span class="sxs-lookup"><span data-stu-id="70284-108">There are just a few steps to export data from C5, and import it in [!INCLUDE[d365fin](includes/d365fin_md.md)]:</span></span> 

1. <span data-ttu-id="70284-109">En la C5, utilice la función **Base de datos de exportación** para exportar los datos.</span><span class="sxs-lookup"><span data-stu-id="70284-109">In C5, use the **Export Database** feature to export the data.</span></span> <span data-ttu-id="70284-110">Envíe la carpeta de exportación a una carpeta comprimida.</span><span class="sxs-lookup"><span data-stu-id="70284-110">Then send the export folder to a compressed (zipped) folder.</span></span>  
2. <span data-ttu-id="70284-111">En [!INCLUDE[d365fin](includes/d365fin_md.md)], seleccione el ícono ![Buscar página o informe](media/ui-search/search_small.png "Buscar página o informe"), introduzca **Migración de datos** y, a continuación, seleccione **Migración de datos**.</span><span class="sxs-lookup"><span data-stu-id="70284-111">In [!INCLUDE[d365fin](includes/d365fin_md.md)], choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Data Migration**, and then choose **Data Migration**.</span></span>
3. <span data-ttu-id="70284-112">Complete los pasos de la guía de configuración asistida.</span><span class="sxs-lookup"><span data-stu-id="70284-112">Complete the steps in the assisted setup guide.</span></span> <span data-ttu-id="70284-113">Asegúrese de elegir **Importar de Microsoft Dynamcis C5 2012** como origen de datos.</span><span class="sxs-lookup"><span data-stu-id="70284-113">Make sure to choose **Import from Microsoft Dynamcis C5 2012** as the data source.</span></span>  

> [!Note] 
> <span data-ttu-id="70284-114">Las empresas a menudo agregan campos para personalizar la C5 para su línea de negocio específica.</span><span class="sxs-lookup"><span data-stu-id="70284-114">Companies often add fields to customize C5 for their specific line of business.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="70284-115"> no migra datos de campos personalizados.</span><span class="sxs-lookup"><span data-stu-id="70284-115"> does not migrate data from custom fields.</span></span> <span data-ttu-id="70284-116">Además, la migración dará error si tiene más de 10 campos personalizados.</span><span class="sxs-lookup"><span data-stu-id="70284-116">Also, migration will fail if you have more than 10 custom fields.</span></span> 

## <a name="viewing-the-status-of-the-migration"></a><span data-ttu-id="70284-117">Ver el estado de la migración</span><span class="sxs-lookup"><span data-stu-id="70284-117">Viewing the Status of the Migration</span></span>
<span data-ttu-id="70284-118">Utilice la página **Información general sobre migración de datos** para controlar el éxito de la migración.</span><span class="sxs-lookup"><span data-stu-id="70284-118">Use the **Data Migration Overview** page to monitor the success of the migration.</span></span> <span data-ttu-id="70284-119">La página muestra información como el número de entidades que la migración incluirá, el estado de la migración, el número de elementos que se han migrado y si lo han hecho correctamente.</span><span class="sxs-lookup"><span data-stu-id="70284-119">The page shows information such as the number of entities that the migration will include, the status of the migration, and the number of items that have been migrated and whether they were successfull.</span></span> <span data-ttu-id="70284-120">También muestra la cantidad de errores, lo que le permite investigar qué salió mal y, cuando es posible, facilita ir a la entidad para solucionar los problemas.</span><span class="sxs-lookup"><span data-stu-id="70284-120">It also shows the number of errors, lets you investigate what went wrong and, when possible, makes it easy to go to the entity to fix the issues.</span></span> <span data-ttu-id="70284-121">Para obtener más información, consulte la siguiente sección de este tema.</span><span class="sxs-lookup"><span data-stu-id="70284-121">For more information, see the next section in this topic.</span></span> 

> [!Note] 
> <span data-ttu-id="70284-122">Mientras espera los resultados de la migración, debe actualizar la página para mostrarlos.</span><span class="sxs-lookup"><span data-stu-id="70284-122">While you are waiting for the results of the migration, you must refresh the page to display the results.</span></span>

## <a name="correcting-errors"></a><span data-ttu-id="70284-123">Corrección de errores</span><span class="sxs-lookup"><span data-stu-id="70284-123">Correcting Errors</span></span>
<span data-ttu-id="70284-124">Si algo sale mal y se produce un error, el campo **Estado** mostrará **Completado con errores** y el campo **Recuento de errores** mostrará cuántos.</span><span class="sxs-lookup"><span data-stu-id="70284-124">If something goes wrong and an error occurs, the **Status** field will show **Completed with Errors**, and the **Error Count** field will show how many.</span></span> <span data-ttu-id="70284-125">Para ver una lista de los errores, puede abrir la página **Errores de migración de datos** si elige:</span><span class="sxs-lookup"><span data-stu-id="70284-125">To view a list of the errors, you can open the **Data Migration Errors** page by choosing:</span></span>

* <span data-ttu-id="70284-126">El número en el campo **Recuento de errores** de la entidad.</span><span class="sxs-lookup"><span data-stu-id="70284-126">The number in the **Error Count** field for the entity.</span></span> 
* <span data-ttu-id="70284-127">La entidad y la acción **Mostrar errores**.</span><span class="sxs-lookup"><span data-stu-id="70284-127">The entity, and then the **Show Errors** action.</span></span> 

<span data-ttu-id="70284-128">En la página **Errores de migración de datos**, para corregir un error puede elegir un mensaje de error y seleccionar **Editar registro** para abrir una página que muestre los datos migrados de la entidad.</span><span class="sxs-lookup"><span data-stu-id="70284-128">On the **Data Migration Errors** page, to fix an error you can choose an error message, then choose **Edit Record** to open a page that shows the migrated data for the entity.</span></span> <span data-ttu-id="70284-129">Después de corregir uno o más errores, puede elegir **Migrar** para migrar solo las entidades que corrigió, sin necesidad de reiniciar por completo la migración.</span><span class="sxs-lookup"><span data-stu-id="70284-129">After you fix one or more errors, you can choose **Migrate** to migrate only the entities you fixed, without having to completely restart the migration.</span></span>  

> [!Tip]
> <span data-ttu-id="70284-130">Si ha solucionado más de un error, puede usar la función **Seleccionar más** para seleccionar varias líneas para migrar.</span><span class="sxs-lookup"><span data-stu-id="70284-130">If you have fixed more than one error, you can use the **Select More** feature to select multiple lines to migrate.</span></span> <span data-ttu-id="70284-131">De forma alternativa, si hay errores que no son importantes para solucionar, puede elegirlos y seleccionar **Omitir selecciones**.</span><span class="sxs-lookup"><span data-stu-id="70284-131">Alternatively, if there are errors that are not important to fix, you can choose them and then choose **Skip Selections**.</span></span>

> [!Note]
> <span data-ttu-id="70284-132">Si tiene elementos que se incluyen en una lista de materiales, es posible que tenga que migrar más de una vez si el elemento original no se crea antes de las variantes que le hacen referencia.</span><span class="sxs-lookup"><span data-stu-id="70284-132">If you have items that are included in a BOM, you might need to migrate more than once if the original item is not created before the variants that reference it.</span></span> <span data-ttu-id="70284-133">Si primero se crea una variante del elemento, la referencia al elemento original puede provocar un mensaje de error.</span><span class="sxs-lookup"><span data-stu-id="70284-133">If an item variant is created first, the reference to the original item can cause an error message.</span></span>  

## <a name="verifying-data-after-migrating"></a><span data-ttu-id="70284-134">Comprobar datos después de migrar</span><span class="sxs-lookup"><span data-stu-id="70284-134">Verifying Data After Migrating</span></span> 
<span data-ttu-id="70284-135">Si desea comprobar que los datos se han migrado correctamente, puede ver las páginas siguientes en la C5 y [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="70284-135">If you want to verify that your data migrated correctly, you can look at the following pages in C5 and [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>

|<span data-ttu-id="70284-136">Microsoft Dynamics C5 2012</span><span class="sxs-lookup"><span data-stu-id="70284-136">Microsoft Dynamcis C5 2012</span></span> | [!INCLUDE[d365fin](includes/d365fin_md.md)]|
|-----|-----|
|<span data-ttu-id="70284-137">Movimientos de cliente</span><span class="sxs-lookup"><span data-stu-id="70284-137">Customer Entries</span></span>| <span data-ttu-id="70284-138">Diarios generales</span><span class="sxs-lookup"><span data-stu-id="70284-138">General Journals</span></span>|
|<span data-ttu-id="70284-139">Movimientos de proveedor</span><span class="sxs-lookup"><span data-stu-id="70284-139">Vendor Entries</span></span>| <span data-ttu-id="70284-140">Diarios generales</span><span class="sxs-lookup"><span data-stu-id="70284-140">General Journals</span></span>|
|<span data-ttu-id="70284-141">Movs. prods.</span><span class="sxs-lookup"><span data-stu-id="70284-141">Item Entries</span></span>| <span data-ttu-id="70284-142">Diarios de productos</span><span class="sxs-lookup"><span data-stu-id="70284-142">Item Journals</span></span>|

<span data-ttu-id="70284-143">En [!INCLUDE[d365fin](includes/d365fin_md.md)], el proceso de los datos migrados se denomina **C5MIGRATE**.</span><span class="sxs-lookup"><span data-stu-id="70284-143">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the batch for the migrated data is named **C5MIGRATE**.</span></span> 

> [!Note]
> <span data-ttu-id="70284-144">No olvide que migramos solamente los movimientos abiertos.</span><span class="sxs-lookup"><span data-stu-id="70284-144">Remember that we migrate only open entries.</span></span> <span data-ttu-id="70284-145">No encontrará datos históricos.</span><span class="sxs-lookup"><span data-stu-id="70284-145">You will not find any historical data.</span></span>

## <a name="stopping-data-migration"></a><span data-ttu-id="70284-146">Detener la migración de datos</span><span class="sxs-lookup"><span data-stu-id="70284-146">Stopping Data Migration</span></span>
<span data-ttu-id="70284-147">Puede detener la migración de datos con la opción **Detener todas las migraciones**.</span><span class="sxs-lookup"><span data-stu-id="70284-147">You can stop migrating data by choosing **Stop All Migrations**.</span></span> <span data-ttu-id="70284-148">Si utiliza esta opción, todas las migraciones pendientes también se detendrán.</span><span class="sxs-lookup"><span data-stu-id="70284-148">If you do, all pending migrations are also stopped.</span></span>

## <a name="see-also"></a><span data-ttu-id="70284-149">Consulte también</span><span class="sxs-lookup"><span data-stu-id="70284-149">See Also</span></span>
<span data-ttu-id="70284-150">[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] usando extensiones](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="70284-150">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="70284-151">[[!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="70284-151">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

