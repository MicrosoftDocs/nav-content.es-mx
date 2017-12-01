---
title: "Uso de la extensión de la migración de QuickBooks"
description: "Describe cómo utilizar la extensión para importar clientes, proveedores, productos y cuentas desde QuickBooks Desktop a Dynamics NAV."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, import, implement
ms.date: 03/29/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 7b8cf77369a2073f746aebdca5d4cbeba80283ec
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="the-quickbooks-data-migration-extension-for-dynamics-nav"></a>Extensión de la migración de datos de QuickBooks para Dynamics NAV
Esta extensión facilita la migración de clientes, proveedores, productos y cuentas de QuickBooks Desktop a [!INCLUDE[d365fin](includes/d365fin_md.md)]. Si la empresa usa QuickBooks actualmente, puede exportar la información correspondiente y después abrir una guía de instalación asistida para cargar los datos en [!INCLUDE[d365fin](includes/d365fin_md.md)].  
Para obtener más información, vea [Importar datos empresariales desde otros sistemas financieros](upload-data.md).

## <a name="exporting-data-from-quickbooks-desktop"></a>Exportar datos desde QuickBooks Desktop
Debe haber exportado algunos o todos los clientes, proveedores, productos de inventario y cuentas existentes a un archivo IIF (Intuit Interchange Format). La extensión de la migración de datos de QuickBooks incluye una asociación predeterminada de datos de QuickBooks para que pueda usar sus datos existentes para probar su nueva empresa [!INCLUDE[d365fin](includes/d365fin_md.md)]. La asignación predeterminada será suficiente en la gran mayoría de casos, pero puede cambiar la asignación en la guía de configuración asistida.  
En QuickBooks, el menú Archivo incluye una utilidad para exportar listas. Para las finalidades de [!INCLUDE[d365fin](includes/d365fin_md.md)], puede exportar las listas siguientes:

* Lista de clientes  
* Lista de proveedores  
* Lista de productos  
* Lista de cuentas  

Los datos exportados se guardan como un archivo IIF que, a continuación, puede cargar a [!INCLUDE[d365fin](includes/d365fin_md.md)].

## <a name="finding-the-quickbooks-data-migration-extension"></a>Buscar la extensión de la migración de datos de QuickBooks
La extensión de la migración de datos de QuickBooks está instalada y lista como parte integrada de la guía de configuración asistida de la migración de datos. Si está preparado para empezar ahora y ha exportado sus datos de QuickBooks, elija icono ![Buscar por página o informe](media/ui-search/search_small.png "icono Buscar por página o informe"), escriba **Configuración asistida** y, a continuación, haga clic el vínculo relacionado. Seleccione **Migrar los datos empresariales**y, a continuación, siga los pasos en la guía.  

## <a name="see-also"></a>Consulte también
[Importar datos de empresa de otros sistemas financieros](upload-data.md)  
[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] usando extensiones](ui-extensions.md)  

