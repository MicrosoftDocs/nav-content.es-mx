---
title: Configurar bancos
description: Puede conciliar cuentas bancarias en Dynamics NAV con los estados de cuenta del banco.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: feed, stream
ms.date: 09/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3581615fe94006aa9245f5e66fe6cf475b22acfb
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-bank-accounts"></a>Procedimiento para configurar las cuentas de bancos
Las cuentas bancarias se utilizan en [!INCLUDE[d365fin](includes/d365fin_md.md)] para hacer un seguimiento de las transacciones bancarias. Los bancos pueden expresarse en la divisa local ($) o en una extranjera. Cuando haya configurado todos los bancos, puede utilizar también la opción de impresión de cheques.

## <a name="to-set-up-bank-accounts"></a>Para configurar bancos
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cuentas bancarias** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Cuentas bancarias**, elija la acción **Nuevo**.
3. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]
> Para completar el campo **Saldo** con un saldo inicial, debe publicar un movimiento de cuenta bancaria con el importe en cuestión. Puede hacerlo si realiza una conciliación de bancos. Para obtener más información, vea [Procedimiento: Conciliar cuentas bancarias por separado](bank-how-reconcile-bank-accounts-separately.md). De forma alternativa, puede implementar el saldo inicial como parte de la creación de datos generales en nuevas compañías mediante la configuración asistida **Migrar datos empresariales**. Para obtener más información, vea [[!INCLUDE[d365fin](includes/d365fin_md.md)](index.md).

## <a name="to-set-up-your-bank-account-for-import-or-export-of-bank-files"></a>Para configurar la cuenta para la importación o exportación de archivos bancarios
Los campos de la ficha desplegable **Transferencia** en la ventana **Ficha banco** están relacionados con la importación y exportación de archivos o fuentes de banco. Para obtener más información, vea [Procedimiento: Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md).

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Cuentas bancarias** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un banco del que exportará archivos de banco, o al que los importará.
3. En la ficha desplegable **Transferencia**, rellene los campos como sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!NOTE]  
>   Distintos servicios de exportación de archivos y sus formatos requieren valores de configuración diferentes en la ventana **Ficha banco**. Estará informado sobre valores de configuración incorrectos o que faltan al intentar exportar el archivo. Leer las descripciones breves de los campos atentamente o consulte los temas relacionados del procedimiento. Por ejemplo, exportar un archivo de pago para la transferencia electrónica de fondos (EFT) de Norteamérica requiere que tanto el campo **Nº último aviso pago** como el campo **Nº tránsito** estén rellenados. Para obtener más información, vea [Procedimiento: Exportar pagos a un archivo bancario](payables-how-export-payments-bank-file.md).

## <a name="to-set-up-vendor-bank-accounts-for-export-of-bank-files"></a>Para configurar cuentas bancarias de proveedor para exportar archivos bancarios
Los campos de la ficha desplegable **Transferencia** en la ventana **Ficha banco proveedor** están relacionados con la exportación de archivos o fuentes de banco. Para obtener más información, vea [Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md) y [Exportar pagos a un archivo bancario](payables-how-export-payments-bank-file.md).

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Proveedores** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un proveedor a cuya cuenta bancaria exportará los archivos bancarios de pagos.
3. Elija la acción **Cuentas bancarias**.
3. En la ficha desplegable **Ficha banco proveedor** de la ventana **Transferencia**, complete los campos como sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-the-opening-balance-on-new-bank-accounts"></a>Para establecer el saldo inicial en nuevas cuentas bancarias


## <a name="see-also"></a>Consulte también
[Configurar banca](bank-setup-banking.md)  
[Administrar cuentas bancarias](bank-manage-bank-accounts.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

