---
title: Registrar ventas
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 0ce8b5d9e77d40a5f10c9242e7368add5b75b12a
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="posting-sales"></a>Registrar ventas
En **Grupo contable** en un documento de ventas, puede elegir entre las funciones de registro siguientes:

- **Registrar**
- **Informe de prueba**
- **Registrar y enviar**
- **Registrar e imprimir**
- **Registrar y enviar por correo electrónico**
- **Registrar por lotes**
- **Vista previa de registro**

Una vez completadas todas las líneas e introducida toda la información en la orden de venta, puede registrarla. Esto crea una remisión y una factura.

Cuando se registra una orden de venta, se actualiza la cuenta del cliente, la contabilidad y los movimientos de producto.

Por cada orden de venta, se crea un movimiento de venta en la tabla **Mov. contabilidad**. Se crea también un movimiento en la cuenta de cliente de la tabla **Mov. cliente** y un movimiento de contabilidad en la cuenta de cliente correspondiente. Además, el registro de la orden puede dar como resultado un movimiento de IVA y uno de contabilidad para el importe de descuento. El registro de un movimiento para el descuento depende del contenido del campo **Registro dto.** de la ventana **Conf. ventas y cobros**.

Por cada línea de orden de venta, se creará un movimiento de producto en la tabla **Mov. producto** (si las líneas de venta contienen números de producto) o un movimiento de contabilidad en la tabla **Mov. contabilidad** (si las líneas de venta contienen una cuenta de contabilidad). Además, las órdenes de venta siempre se registran en las tablas **Histórico cab. remisión venta** y **Histórico cab. factura venta**.

**Importante**: Cuando registre una orden, puede crear una remisión y una factura. Esto se puede realizar al mismo tiempo o de manera independiente. También puede crear una remisión y una factura parciales completando los campos **Cantidad a enviar** y **Cantidad a facturar** en las líneas individuales de la orden de venta antes de registrar. Tenga en cuenta que no puede crear una factura de algo no se ha enviado. Es decir, antes de poder facturar, tiene que haber registrado una remisión de venta o haber seleccionado, al mismo tiempo, entregar y facturar. 

Una vez completado el registro, las líneas de venta registradas se quitan de la orden. Al terminar el registro aparece un mensaje de aviso. Después de esto, podrá ver los movimientos registrados en las diferentes ventanas que los contienen, como **Movs. cliente**, **Movs. contabilidad**, **Movs. producto**, **Histórico albaranes ventas** y **Histórico facturas venta**.

## <a name="see-also"></a>Consulte también
[Enviar documentos por correo electrónico](ui-how-send-documents-email.md)
