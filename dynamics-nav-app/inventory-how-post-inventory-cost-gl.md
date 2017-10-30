---
title: "Cómo registrar costos de inventario en la contabilidad general"
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: 34eec596392e9316e807d3c073c3b8e59dbc12e9
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---

# <a name="how-to-post-inventory-costs-to-the-general-ledger"></a>Cómo registrar costos de inventario en la contabilidad general   
Cuando registra transacciones de inventario, como las remisiones de venta, facturas de compra o ajustes de inventario, las cantidades y los costos cambiados se registran en los movimientos de producto y en los movimientos de valor, respectivamente. Para reflejar este cambio de valor del inventario en sus libros de finanzas, debe registrar los costos de inventario en las cuentas de inventario relacionadas del libro mayor.

Puede registrar los costos de inventario en el libro mayor de dos formas:

- De forma automática, de modo que los costos de inventario se registren en el libro mayor cada vez que registre una transacción de inventario.
- Manualmente, de modo que los costos de inventario solo se registren en el libro mayor cuando ejecute un proceso.


## <a name="to-post-inventory-costs-automatically"></a>Para registrar costos del inventario de forma automática
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de inventario** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Configuración de inventario**, marque la casilla **Variación existencias automát**.

Para cada una de las transacciones de inventario que registre, los valores apropiados se contabilizan en la cuenta de inventario, en la cuenta de ajuste y en la cuenta de CV en el módulo de contabilidad.

Aunque use el registro de costos automático, seguirá siendo necesario ejecutar periódicamente el proceso Valorar stock - movs. producto para asegurarse de que los costos de los bienes se dirigen a las transacciones de salida apropiadas, como son las ventas o las transferencias. Esto es muy importante en aquellas situaciones en las que se venden bienes antes de generar la factura de compra para dichos bienes.

Si se produce un error en la configuración de dimensión durante el registro del costo de inventario en el módulo de contabilidad, el registro finalizará con un error.

## <a name="to-post-inventory-costs-manually"></a>Para registrar los costos de inventario de forma manual
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Reg. var. inventario en cont.** y, a continuación, elija el enlace relacionado.
2. Puede registrar manualmente los costos de inventario en el módulo de contabilidad, si ejecuta el trabajo por lotes. Cuando lo ejecute, se crearán los movimientos de contabilidad según los movimientos de valoración. Es posible registrar los movimientos de forma que estén agrupados por grupos contables.

**Nota**: Cuando lo ejecute, es posible que encuentre errores porque faltan datos en la configuración o porque la configuración de dimensión no es compatible. Si el proceso encuentra errores relacionados con la configuración de dimensión, omitirá dichos errores y utilizará las dimensiones del movimiento de valor. Para el resto de errores, el proceso omitirá registrar los movimientos de valores y mostrará una lista de ellos al final del informe, en una sección llamada "Movimientos omitidos". Para registrar dichos movimientos, deberá primeramente arreglar las causas de los errores.

Para ver una lista con los errores antes de ejecutar el proceso de registro, puede ejecutar el informe **Reg. var. ex. en cont. - Test**. El informe de test muestra un listado con todos los errores encontrados durante un proceso de registro de prueba. A continuación, puede solucionar dichos errores y ejecutar el proceso de registro de costos sin que se omita ningún movimiento.

Si simplemente desea obtener una visión general acerca de qué valores se podrán registrar en el módulo de contabilidad sin que realmente se registren, puede ejecutar el proceso Regis. variación inventario en Cont. sin que se registren los valores en el módulo de contabilidad. Para ello, deberá quitar la marca de verificación del campo Registrar en la página de solicitud. De esta forma, cuando ejecute el trabajo por lotes, se genera un informe que muestra los valores que están preparados para ser registrados en el módulo de contabilidad, pero no se registran.

## <a name="see-also"></a>Consulte también
[Gestionar inventario](inventory-manage-inventory.md)    
[Procedimiento: Ajustar precios de productos](inventory-how-adjust-item-costs.md)  
[Gestionar ventas](sales-manage-sales.md)  
[Gestionar compras](purchasing-manage-purchasing.md)

