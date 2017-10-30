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

# <a name="the-c5-data-migration-extension-for-dynamics-nav"></a>Extensión de migración de datos de C5 para Dynamics NAV
Esta extensión facilita la migración de clientes, proveedores, productos y las cuentas de contabilidad de Microsoft Dynamics C5 2012 a [!INCLUDE[d365fin](includes/d365fin_md.md)]. 

> [!Note] 
> La empresa en [!INCLUDE[d365fin](includes/d365fin_md.md)] no debe contener ningún dato. Además, después de iniciar una migración, no debe crear clientes, proveedores, artículos ni cuentas hasta que la finalice.

## <a name="to-migrate-data"></a>Para migrar datos
Deben realizarse algunos para exportar datos de la C5 e importarlos a [!INCLUDE[d365fin](includes/d365fin_md.md)]: 

1. En la C5, utilice la función **Base de datos de exportación** para exportar los datos. Envíe la carpeta de exportación a una carpeta comprimida.  
2. En [!INCLUDE[d365fin](includes/d365fin_md.md)], seleccione el ícono ![Buscar página o informe](media/ui-search/search_small.png "Buscar página o informe"), introduzca **Migración de datos** y, a continuación, seleccione **Migración de datos**.
3. Complete los pasos de la guía de configuración asistida. Asegúrese de elegir **Importar de Microsoft Dynamcis C5 2012** como origen de datos.  

> [!Note] 
> Las empresas a menudo agregan campos para personalizar la C5 para su línea de negocio específica. [!INCLUDE[d365fin](includes/d365fin_md.md)] no migra datos de campos personalizados. Además, la migración dará error si tiene más de 10 campos personalizados. 

## <a name="viewing-the-status-of-the-migration"></a>Ver el estado de la migración
Utilice la página **Información general sobre migración de datos** para controlar el éxito de la migración. La página muestra información como el número de entidades que la migración incluirá, el estado de la migración, el número de elementos que se han migrado y si lo han hecho correctamente. También muestra la cantidad de errores, lo que le permite investigar qué salió mal y, cuando es posible, facilita ir a la entidad para solucionar los problemas. Para obtener más información, consulte la siguiente sección de este tema. 

> [!Note] 
> Mientras espera los resultados de la migración, debe actualizar la página para mostrarlos.

## <a name="correcting-errors"></a>Corrección de errores
Si algo sale mal y se produce un error, el campo **Estado** mostrará **Completado con errores** y el campo **Recuento de errores** mostrará cuántos. Para ver una lista de los errores, puede abrir la página **Errores de migración de datos** si elige:

* El número en el campo **Recuento de errores** de la entidad. 
* La entidad y la acción **Mostrar errores**. 

En la página **Errores de migración de datos**, para corregir un error puede elegir un mensaje de error y seleccionar **Editar registro** para abrir una página que muestre los datos migrados de la entidad. Después de corregir uno o más errores, puede elegir **Migrar** para migrar solo las entidades que corrigió, sin necesidad de reiniciar por completo la migración.  

> [!Tip]
> Si ha solucionado más de un error, puede usar la función **Seleccionar más** para seleccionar varias líneas para migrar. De forma alternativa, si hay errores que no son importantes para solucionar, puede elegirlos y seleccionar **Omitir selecciones**.

> [!Note]
> Si tiene elementos que se incluyen en una lista de materiales, es posible que tenga que migrar más de una vez si el elemento original no se crea antes de las variantes que le hacen referencia. Si primero se crea una variante del elemento, la referencia al elemento original puede provocar un mensaje de error.  

## <a name="verifying-data-after-migrating"></a>Comprobar datos después de migrar 
Si desea comprobar que los datos se han migrado correctamente, puede ver las páginas siguientes en la C5 y [!INCLUDE[d365fin](includes/d365fin_md.md)].

|Microsoft Dynamics C5 2012 | [!INCLUDE[d365fin](includes/d365fin_md.md)]|
|-----|-----|
|Movimientos de cliente| Diarios generales|
|Movimientos de proveedor| Diarios generales|
|Movs. prods.| Diarios de productos|

En [!INCLUDE[d365fin](includes/d365fin_md.md)], el proceso de los datos migrados se denomina **C5MIGRATE**. 

> [!Note]
> No olvide que migramos solamente los movimientos abiertos. No encontrará datos históricos.

## <a name="stopping-data-migration"></a>Detener la migración de datos
Puede detener la migración de datos con la opción **Detener todas las migraciones**. Si utiliza esta opción, todas las migraciones pendientes también se detendrán.

## <a name="see-also"></a>Consulte también
[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] usando extensiones](ui-extensions.md)  
[[!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)  

