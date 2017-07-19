---
title: Procesamiento de devoluciones de compra o cancelaciones
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 94067fb3d10975c1db29d2e3f1d5d6373fcbf9f2
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-process-purchase-returns-or-cancellations"></a>Procesamiento de devoluciones de compra o cancelaciones
Si desea devolver productos al proveedor o cancelar servicios comprados, puede crear y registrar una nota de crédito de compras que especifique el cambio solicitado en relación a la factura de compra original. Para incluir la información correcta de la factura de compra, puede crear la nota de crédito de compra de la factura de compra registrada o usar una función de copia.

Normalmente, se crea una nota de crédito de compras como resultado de una nota de crédito enviada por un proveedor. La nota de crédito de compras funciona como la documentación interna del proceso de nota de crédito para fines contables.

El cambio puede relacionarse con todos los productos en la factura de compra original o solo algunos de los productos. Por consiguiente, puede devolver productos parcialmente recibidos o exigir un reembolso parcial de los servicios recibidos. En ese caso, debe modificar la información copiada de la factura de compra.

Además de la original factura de compra registrada, puede liquidar la nota de crédito de compra en otros documentos de compra, por ejemplo, otra factura de compra registrada, porque usted también devuelve los productos entregados con dicha factura.

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Para crear una nota de crédito de compra desde una factura de compra registrada.
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Notas de crédito de compra** y, a continuación, elija el enlace relacionado.  
2. En la ventana **Facturas de compra registradas**, seleccione la factura de compra que desea revertir y, a continuación, seleccione la acción **Crear nota de crédito correctiva**.

    La mayoría de los campos de la cabecera de nota de crédito de compra se rellenan con la información de la factura de compra registrada. Puede modificar todos los campos, por ejemplo, mediante la nueva información que indica el contrato de devolución.
3. Edite la información de las líneas según el contrato, como por ejemplo el número de productos devueltos o el importe que se reembolsará.
4. Seleccione la acción **Liquidar movs.**.
5. En la ventana **Liquidar movimientos proveedor**, seleccione la línea con el documento de compra registrado en el que desee liquidar la nota de crédito de compra y, a continuación, seleccione la acción **Liq. por id.**. El número de la nota de crédito de compra se inserta en el campo **Liq. por id**.
6. En la línea del campo **Importe a liquidar**, introduzca el importe que desea liquidar si es menor que el importe original.

    En la parte inferior de la ventana **Liq. movs. proveedor**, puede observar el importe total a liquidar para revertir todos los movimientos correspondientes, concretamente cuando el valor en el campo **Balanza** es cero.
7. Elija el botón **Aceptar**. Cuando registra la nota de crédito de compra, esta se aplica a los documentos de compra registrados especificados.

    Cuando ha creado o editado las líneas de nota de crédito de compra necesarias y se han especificado una o varias aplicaciones, puede empezar a registrar la nota de crédito de compra.
8. Seleccione la acción **Registrar**.

Las facturas de compra registradas a las que se aplica la nota de crédito ahora están revertidas. Si ya ha pagado la factura original, el proveedor ahora deberá reembolsarle el pago a usted. Si la nota de crédito es solo para parte del producto en la factura original, puede pagar solo el importe pendiente en la factura de compra original para cerrarla.

La nota de crédito de compra se ha eliminado y remplazado por un nuevo documento en la lista de notas de crédito compras registradas.

## <a name="to-create-a-purchase-credit-memo-from-scratch"></a>Para crear una nota de crédito de compra desde cero
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Facturas de compra registradas** y, a continuación, elija el enlace relacionado.
2. Seleccione la acción **Nuevo** para abrir una nota de crédito de compra vacía.
3. En el campo **Proveedor**, escriba el nombre de un proveedor existente.
4. Elija la acción **Copiar documento**.
5. En la ventana **Copiar documento de compra**, en el campo **Tipo de documento**, seleccione el campo **Factura registrada**
6. Seleccione el **N.º documento**. para abrir la ventana **Facturas de compra registradas** y, a continuación, seleccione la factura de compra registrada que contiene las líneas que desea revertir.
7. Seleccione la casilla **Recalcular líneas** si desea que las líneas de factura de compra registradas copiadas se actualicen con los cambios en el precio y el costo unitario del producto desde que la factura fue registrada.
8. Elija el botón **Aceptar**. Las líneas de factura copiadas se insertarán en la nota de crédito de compra.
9. Complete la nota de crédito de compra como se explica en la sección "Para crear una nota de crédito de compra a partir de una factura de compra registrada" en este tema.

## <a name="see-also"></a>Consulte también
[Gestionar compras](purchasing-manage-purchasing.md)  
[Registro de compras](purchasing-how-record-purchases.md)  

