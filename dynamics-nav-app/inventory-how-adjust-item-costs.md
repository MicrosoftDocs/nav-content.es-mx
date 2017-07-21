---
title: 'Procedimiento: Ajustar precios de productos'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 59db38c159dd2810656edc668ee431c6414b9d90
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-adjust-item-costs"></a>Procedimiento: Ajustar precios de productos   
El precio de un producto (valor de inventario) que compre y más tarde venda puede cambiar durante su vida útil, por ejemplo, debido a que se agregue un costo de flete a su precio de compra después de que haya vendido el producto. Para conocer siempre el valor de inventario correcto, los costos de productos se deben ajustar con frecuencia.
Esto garantiza que las estadísticas relativas a ventas y beneficios estén actualizadas y que los KPI financieros sean correctos.

**Nota**: Los costes del producto solo se ajustan por el método de valoración de costes FICO. Esto significa que el costo unitario de un producto es el valor real de cualquier recepción del producto y que el inventario se valora suponiendo que el primer producto del inventario se vende primero.

La función de ajuste de costos solo procesa los movimientos de valores que aún no se hayan ajustado. Si la función encuentra una situación en que es necesario transferir los precios de entrada cambiados a movimientos de salida asociados, se crean nuevos movimientos de valor de ajuste, que se basan en la información de los movimientos de valor de ajuste, pero contienen el importe de ajuste. La función de ajuste de costos usa la fecha de registro del movimiento de valor original en el movimiento de ajuste, a menos que dicha fecha se encuentre dentro de un periodo del inventario que esté cerrado. En ese caso, el programa utilizará la fecha de inicio como el siguiente periodo del inventario abierto. Si no se usan periodos de inventario, la fecha del campo **Permitir registro desde** de la ventana **Configuración contabilidad** definirá cuándo se registra el movimiento de ajuste.

**Nota**: Cuando se hayan ajustado los costos de los productos, el costo de inventario se debe registrar en el libro mayor, ya sea manual o automáticamente. Para obtener más información, consulte [Procedimiento: Registrar costos de inventario en el libro mayor](inventory-how-post-inventory-cost-gl.md).

Puede ajustar los precios de los productos de dos formas:
 - Automáticamente, al configurar el sistema para ajustar los cambios de costo cada vez que se registren transacciones de inventario.
 - Manualmente, al ejecutar el proceso **Valorar stock - movs. producto** para uno o más productos cuando sepa que hayan cambiado sus costos.  

## <a name="to-adjust-item-costs-automatically"></a>Para ajustar los precios de producto automáticamente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de inventario** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Configuración de inventario**, en el campo **Ajuste automático de costo**, seleccione uno de los valores siguientes.

|Opción |Comportamiento |
|-------|---------|
|Nunca|Los costos no se ajustan al registrarlos.|
|DÍA|Los costos se ajustan si el registro se produce en el plazo de un día a partir de la fecha de trabajo.|
|Semana|Los costos se ajustan si el registro se realiza dentro de una semana a partir de la fecha de trabajo.|
|Mes|Los costos se ajustan si el registro se realiza en el plazo de un mes a partir de la fecha de trabajo.|
|Trimestre|Los costos se ajustan si el registro se lleva a cabo en el plazo de un trimestre a partir de la fecha de trabajo.|
|Año|Los costos se ajustan si el registro se realiza en el plazo de un año a partir de la fecha de trabajo.|
|Siempre|Los costos siempre se ajustan al registrarlos, independientemente de la fecha de registro.|

## <a name="to-adjust-item-costs-manually"></a>Para ajustar manualmente precios de productos
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Valorar stock - movs. producto** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Valorar stock - movs. producto**, especifique para qué productos quiere ajustar los costos y si los costos ajustados se registrarán en el libro mayor al mismo tiempo.

## <a name="see-also"></a>Consulte también
[Gestionar inventario](inventory-manage-inventory.md)  
[Cómo registrar costes de inventario en la contabilidad general](inventory-how-post-inventory-cost-gl.md)  
[Gestionar ventas](sales-manage-sales.md)  
[Gestionar compras](purchasing-manage-purchasing.md)

