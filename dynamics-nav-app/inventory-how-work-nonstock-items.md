---
title: 'Procedimiento: Trabajar con productos no inventariables'
author: SorenGP
ms.custom: na
ms.date: 09/29/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2b49d95904732dcf091fd060a96006fdcb477ec1
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-work-with-nonstock-items"></a>Procedimiento: Trabajar con productos no inventariables
Puede ofrecer varios productos a sus clientes para su comodidad que no desea mantener en el inventario hasta que empiece a venderlos. Cuando desee empezar a mantener esos productos en el inventario, puede convertirlos en fichas de productos normales de dos formas.

- Desde una ficha de producto no inventariable, cree una nueva ficha de producto basada en una plantilla.
- Desde una línea de orden de venta que tenga vació el campo **Producto**, seleccione un producto no inventariable. Cuando registra la venta, se crea automáticamente una ficha de producto para el producto no inventariable.

**Nota**: No puede seleccionar un producto no inventariable en la ventana **Factura de venta**. Puede seleccionarlo desde la ventana **Cotización de venta**, pero el producto no inventariable no se convertirá en uno normal cuando utilice la función **Realizar orden**.

Un producto no inventariable normalmente tiene el número del proveedor que lo suministra. Para activar la conversión de una ficha de producto no inventariable a una ficha de producto normal, debe configurar cómo se convertirá la numeración del producto del vendedor a la suya.   

## <a name="to-create-a-nonstock-item"></a>Para crear productos no inventariables
Las fichas de productos no inventariables disponen de mucha menos información que las de productos normales puesto que solo se las utiliza en cotizaciones de ventas y de otras maneras. Por esa razón, se convertirán en fichas de producto normal antes de que pueda registrarles las transacciones de venta.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Productos no inventariables** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

## <a name="to-set-up-how-nonstock-item-numbers-are-converted-to-your-own-numbering"></a>Para configurar cómo se convierten los números de productos no inventariables a la numeración que usted usa  
Para activar la conversión de una ficha de producto no inventariable en una ficha de producto normal, primero debe especificar cómo se convertirá la numeración del producto del proveedor a su formato de número de producto.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Conf. prod. no inventariables** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.

## <a name="to-convert-a-nonstock-item-to-a-normal-item"></a>Para convertir un producto no inventariable en un producto normal
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Productos no inventariables** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un producto no inventariable que desee convertir a uno normal.
3. En la ventana **Ficha prod. no inventariable**, seleccione la acción **Crear producto**.

Se ha creado una nueva ficha de producto con la información del producto no inventariable rellenada previamente y la plantilla de producto correspondiente. Si es necesario, podrá rellenar o editar los campos en la nueva ficha de producto. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

## <a name="to-sell-a-nonstock-item-and-convert-it-to-a-normal-item"></a>Para vender un producto no inventariable y convertirlo en un producto normal
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Órdenes de venta** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**. rellene los campos de la ficha desplegable **General** para cada orden.
3. En una nueva línea de orden, deje el campo **Producto** vacío, seleccione **Línea**, **Funciones** y, a continuación, **Productos no inventariables**.

    El producto no inventariable se ha convertido en un producto normal. Se ha creado una nueva ficha de producto con la información del producto no inventariable rellenada previamente y la plantilla de producto correspondiente.
4. En la ventana **Productos no inventariables**, seleccione el producto no inventariable que desea vender y, a continuación, haga clic en **Aceptar**.
5. Cuando la orden de venta esté completa, seleccione la acción **Registrar**.

Si es necesario, podrá rellenar o editar los campos en la nueva ficha de producto. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

**Nota**: Un informe de referencia cruzada de un producto se crea automáticamente por el proveedor del producto entre el número del producto del proveedor y su nuevo número de producto.

## <a name="see-also"></a>Consulte también
[Registro de productos nuevos](inventory-how-register-new-products.md)  
[Gestionar inventario](inventory-manage-inventory.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)
