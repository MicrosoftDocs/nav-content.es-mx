---
title: Administrar inventario
description: "Describe cómo administrar los productos físicos que comercializa, por ejemplo, manipulación de las existencias en el almacén."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, stock
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 8b79bfd187b04e378180d699aa880e21cf8410c9
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---

# <a name="inventory"></a>Inventario
Por cada producto físico que se comercialice, debe crear una ficha de producto del tipo **Inventario**. Los productos que ofrece a los clientes pero que no mantiene en el inventario, puede registrarlos como productos no inventariables, y puede convertirlos a productos de inventario cuando sea necesario. Puede aumentar o reducir la cantidad de un producto en el inventario registrándolo directamente desde los movimientos de producto, por ejemplo, después de un recuento físico o si no registra compras.

Los aumentos y las disminuciones de inventario también se registran cuando registra documentos de compra y de ventas respectivamente. Para obtener más información, vea [Procedimiento: Registrar](purchasing-how-record-purchases.md), [Procedimiento: Vender productos](sales-how-sell-products.md) y [Procedimiento: Facturar ventas](sales-how-invoice-sales.md). Las transferencias entre almacenes cambian las cantidades de inventario en los almacenes de la empresa.   

Para aumentar la información general de los productos y ayudarle a encontrarlos, puede clasificar los productos y darles atributos para que los pueda ordenar y buscar.

> [!NOTE]
> El control físico de los productos se denomina actividades de almacén. Para obtener más información, consulte [Gestión de almacén](warehouse-manage-warehouse.md).

## <a name="inventory-reconciliation"></a>Conciliación de inventario
Cuando registra transacciones del inventario, como los envíos de ventas, los albaranes de compra o los ajustes de inventario, los costes de producto cambiados se registran en movimientos de valor de productos. Para reflejar este cambio de valor de inventario en sus libros de finanzas, los costes de inventario se registran automáticamente en las cuentas de inventario relacionadas del libro mayor. Para cada una de las transacciones de inventario que registre, los valores apropiados se contabilizan en la cuenta de inventario, en la cuenta de ajuste y en la cuenta de CV en el módulo de contabilidad. Para obtener más información, consulte [Procedimiento: Conciliar costos de inventario con la contabilidad general](finance-how-to-post-inventory-costs-to-the-general-ledger.md).

Aunque se hayan registrado los costes de inventario automáticamente en el libro mayor, seguirá siendo necesario asegurarse de que los costes de los bienes se dirigen a las transacciones de venta de salida relacionadas, especialmente en situaciones donde la venta de bienes se factura antes de la compra de estos bienes. Esto se denomina ajuste de costos. Los costes de los productos se ajustan automáticamente cada vez que registra transacciones de producto, pero también puede ajustar los costes de producto manualmente. Para obtener más información, consulte [Procedimiento: Modificar precios de productos](inventory-how-adjust-item-costs.md).

|Para |Vea |
|---|----|
|Crear fichas de los productos de inventario que comercialice.|[Registro de productos nuevos](inventory-how-register-new-items.md)|
|Estructure los productos principales que vende como kits que constan de los componentes del principal o que ensamble para pedido o para stock.|[Trabajar con listas de materiales](inventory-how-work-BOMs.md)|
|Mantener una visión general de los productos y ayudarle a buscarlos y clasificarlos al organizarlos en categorías.|[Clasificar productos](inventory-how-categorize-items.md)|
|Asignar atributos de producto de distintos tipos de valor a sus productos le ayudará a ordenarlos y encontrarlos.|[Trabajar con atributos de producto](inventory-how-work-item-attributes.md)|
|Crear fichas especiales para los productos que desea ofrecer a los clientes, pero que no desea mantener en el inventario.|[Procedimiento: Trabajar con productos sin stock](inventory-how-work-nonstock-items.md)|
|Realizar recuento físico, hacer ajustes negativos o positivos y cambiar la información, como la ubicación o el número de lote, en los movimientos de productos.|[Recuento, ajuste y reclasificación de inventario](inventory-how-count-adjust-reclassify.md)|
|Ver la disponibilidad de productos por almacén, por periodo, por evento de venta o de compra, o por su uso en las L.M. de ensamblado o producción.|[Consultar la disponibilidad de los productos](inventory-how-availability-overview.md)|
|Transferir productos de inventario entre almacenes con pedidos de transferencia, para administrar las actividades de almacén o con el diario de reclasificación de productos.|[Transferir el inventario entre almacenes](inventory-how-transfer-between-locations.md)|
|Reserve productos de inventario o entrantes para pedidos de venta, pedidos de servicio, pedidos de ensamblado u órdenes de producción.|[Procedimiento: Reservar productos](inventory-how-to-reserve-items.md)|
|Asigne números de serie o números de lote a cualquier documento o línea de diario saliente o entrante, por ejemplo, para el seguimiento de productos en caso de recuperaciones.|[Procedimiento: Trabajar con números de lote y de serie](inventory-how-work-item-tracking.md)|
|Encuentre donde se usó un número de serie o de lote en su cadena de suministro, por ejemplo, en situaciones de recuperación.|[Cómo realizar un seguimiento de productos marcados para seguimiento](inventory-how-to-trace-item-tracked-items.md)|
|Administre las operaciones comerciales en las oficinas de ventas, en los departamentos de compras o en las oficinas de planificación de plantas en múltiples ubicaciones.|[Trabajar con centros de responsabilidad](inventory-responsibility-centers.md)|

## <a name="see-also"></a>Consulte también  
[Compras](purchasing-manage-purchasing.md)  
[Ventas](sales-manage-sales.md)    
[Trabajar con [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](ui-work-product.md)  
[Funciones empresariales generales](ui-across-business-areas.md)

##

