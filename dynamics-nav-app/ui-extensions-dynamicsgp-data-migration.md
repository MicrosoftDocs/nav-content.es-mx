---
title: "Migrar datos de Dynamics GP con la extensión de la migración de datos"
description: "Utilice la extensión de migración de datos de Dynamics GP para migrar clientes, proveedores, productos de inventario y cuentas desde Dynamics GP a Dynamics NAV."
documentationcenter: 
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
ms.openlocfilehash: 0156ec040b96f007674161361e4368b81f7c42d9
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="the-dynamics-gp-data-migration-extension-for-dynamics-nav"></a>Extensión de la migración de datos de Dynamics GP para Dynamics NAV
Esta extensión facilita la migración de clientes, proveedores, productos de inventario y cuentas de Dynamics GP a [!INCLUDE[d365fin](includes/d365fin_md.md)]. Si la empresa usa Dynamics GP actualmente, puede exportar los registros maestros correspondientes y después abrir una guía de instalación asistida para agregar los datos a [!INCLUDE[d365fin](includes/d365fin_md.md)]. Para obtener más información, vea [Migrar datos empresariales desde otros sistemas financieros](upload-data.md).

## <a name="exporting-data-from-dynamics-gp"></a>Exportar datos desde Dynamics GP
Deberá haber exportado todos los clientes, proveedores, productos de inventario y cuentas existentes, o parte de ellos, mediante la funcionalidad de exportación de datos de Dynamics GP. Para las finalidades de [!INCLUDE[d365fin](includes/d365fin_md.md)], puede exportar los tipos de datos siguientes:

* Cuenta  
* Cliente  
* Elemento  
* Proveedor  

La extensión de la migración de datos de Dynamics GP asigna automáticamente los datos exportados para que estén a su disposición rápidamente en la nueva empresa de [!INCLUDE[d365fin](includes/d365fin_md.md)]. Durante el proceso, se crea información de configuración auxiliar, por ejemplo grupos contables. Los productos de existencias se incorporarán al sistema con el método de valoración de costo FIFO. Las cuentas se configurarán como el segmento de cuenta principal desde Dynamics GP con dimensiones, porque [!INCLUDE[d365fin](includes/d365fin_long_md.md)] no tiene segmentos de cuentas.

## <a name="see-also"></a>Consulte también
[Importar datos de empresa de otros sistemas financieros](upload-data.md)  
[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] usando extensiones](ui-extensions.md)  

