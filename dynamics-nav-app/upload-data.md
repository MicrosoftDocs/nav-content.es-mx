---
title: Importar los datos empresariales heredados en Dynamics NAV
description: Puede migrar datos para clientes, proveedores e inventario, por ejemplo, desde Excel, QuickBooks o Dynamics GP, a Dynamics NAV.
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: migrate, initialize, implement
ms.date: 09/25/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b19a05fba8a940dad4dcb6c8aebbefdcae67c324
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="importing-business-data-from-other-finance-systems"></a>Importar datos de empresa de otros sistemas financieros
Cuando se registra en [!INCLUDE[d365fin](includes/d365fin_md.md)], puede elegir crear una empresa vacía, de este modo podrá cargar sus datos y probar su nueva empresa de [!INCLUDE[d365fin](includes/d365fin_md.md)]. En función de la solución de finanzas que use su empresa actualmente, puede transferir información sobre clientes, proveedores, inventario y cuentas bancarias.  

Desde la página Inicio, puede iniciar una guía de configuración asistida que le ayudará a transferir los datos de la empresa de un archivo Excel o de otros formatos. El tipo de archivos que puede cargar depende de las extensiones disponibles. Por ejemplo, puede migrar los datos de QuickBooks, ya que [!INCLUDE[d365fin](includes/d365fin_md.md)] incluye una extensión que gestiona la conversión desde QuickBooks. Si desea migrar los datos de otras soluciones de finanzas, debe comprobar si hay una extensión disponible para esa solución o importarlos desde Excel.  

[!INCLUDE[d365fin](includes/d365fin_md.md)] incluye plantillas de cuentas, clientes, proveedores y productos de inventario que puede elegir para que se apliquen al importar sus datos.  

## <a name="importing-data-from-quickbooks-or-dynamics-gp"></a>Importar datos de QuickBooks o Dynamics GP
Si su empresa actualmente usa QuickBooks o Dynamics GP, puede exportar la información pertinente a un archivo. Puede iniciar la guía de configuración asistida para transferir los datos.
Por ejemplo, si su archivo incluye clientes y proveedores, puede elegir transferir solo los datos de cliente. Podrá transferir el resto de la información más adelante.  

La configuración asistida incluye una opción para cambiar la configuración predeterminada de la transferencia, pero le recomendamos que solo introduzca la configuración avanzada si está familiarizado con tablas de bases de datos. En gran la mayoría de las empresas, la asignación predeterminada de QuickBooks o Dynamics GP a [!INCLUDE[d365fin](includes/d365fin_md.md)] transferirá la información que desee.  

Para obtener más información, vea [Migración de datos de QuickBooks Desktop](ui-extensions-quickbooks-data-migration.md), [Migración de datos de QuickBooks Online](ui-extensions-quickbooks-online-data-migration.md) o [Migración de datos de Dynamics GP](ui-extensions-dynamicsgp-data-migration.md).  

## <a name="importing-data-from-configuration-packages"></a>Importar datos desde los paquetes de configuración
[!INCLUDE[d365fin](includes/d365fin_md.md)] incluye un paquete de configuración que puede exportar a Excel y configurar los datos en esa aplicación. A continuación, puede volver a importar los datos desde Excel. El paquete consta de 27 tablas, incluidos datos maestros, como clientes, proveedores, productos y cuentas, otras tablas básicas de configuración, como métodos de envío, y tablas de transacciones, como encabezado y líneas de venta.  

> [!NOTE]  
>   El trabajo con paquetes de configuración es una función avanzada y le recomendamos que se ponga en contacto con el administrador. Para obtener más información, vea [Importar datos del software de contabilidad heredado mediante un paquete de configuración](across-import-data-configuration-packages.md).  

## <a name="see-also"></a>Consulte también
[Finanzas](finance.md)  
[Importar datos del software de contabilidad heredado mediante un paquete de configuración](across-import-data-configuration-packages.md)  
[Migración de datos de QuickBooks Desktop](ui-extensions-quickbooks-data-migration.md)  
[Migración de datos de QuickBooks Online](ui-extensions-quickbooks-online-data-migration.md)  
[Migración de datos de Dynamics GP](ui-extensions-dynamicsgp-data-migration.md)  
[Personalizar [!INCLUDE[d365fin](includes/d365fin_md.md)] con extensiones ](ui-extensions.md)   
[Equipar [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)

## 

