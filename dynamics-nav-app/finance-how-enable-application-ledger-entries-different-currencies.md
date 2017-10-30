---
title: Liquidar movimientos en distintas divisas
description: Puede liquidar movimientos en varias divisas, por ejemplo, si vende a un cliente en una divisa y cobra en otra.
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, payment, reconcile
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: f323b98472f3e2ef0f28000f8a9140b066206945
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-enable-application-of-ledger-entries-in-different-currencies"></a>Procedimiento: Permitir la liquidación de movimientos de cliente en distintas divisas
Si se realiza una compra a un proveedor en una divisa y se emite el pago en otra divisa, es posible liquidar la compra con el pago.

De igual modo, si vende a un cliente en una divisa y cobra en otra, puede liquidar el pago con la factura de venta.

El procedimiento siguiente describe cómo configurarlo para movimientos de proveedor en la ventana **Configuración de compras y pagos**. La configuración es similar para los movimientos de cliente en la ventana **Configuración de ventas y cobros**.

## <a name="to-enable-application-of-vendor-ledger-entries-in-different-currencies"></a>Para permitir la liquidación de movimientos de proveedor en divisas distintas
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Configuración de compras y pagos** y, a continuación, seleccione el vínculo relacionado.
2. En el campo **Liquidación entre divisas**, seleccione una de las siguientes opciones.

| Opción | Descripción |
| --- | --- |
| Ninguno |No se permite la liquidación entre divisas. |
| UME |Se permite la liquidación entre divisas de la UME. |
| Todo |Se permite la liquidación entre todas las divisas. |

## <a name="to-set-up-gl-accounts-for-currency-application-rounding-differences"></a>Para configurar cuentas para liquidar diferencias de redondeo en divisa  
Si liquida movimientos en varias divisas distintas, debe configurar las cuentas en las que se registrarán las diferencias de redondeo.  

> [!NOTE]  
>  Primero debe configurar las cuentas contables antes de completar la tarea. Para obtener más información, consulte [Descripción del libro mayor y plan de cuentas](finance-general-ledger.md).

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Grupos contables clientes** y, a continuación, seleccione el vínculo relacionado.  
2. En los campos **Cta. neg. red. liquids. divisa** y **Cta. pos. red. liquids. divisa**, especifique el número de cuentas contables para registrar las diferencias de redondeo.  
3. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Grupos de registro del proveedor** y, a continuación, seleccione el vínculo relacionado.  
4. En los campos **Cta. neg. red. liquids. divisa** y **Cta. pos. red. liquids. divisa**, especifique el número de cuentas contables para registrar las diferencias de redondeo.  

## <a name="see-also"></a>Consulte también
[Administrar pagos](payables-manage-payables.md)  
[Administrar cobros](receivables-manage-receivables.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

