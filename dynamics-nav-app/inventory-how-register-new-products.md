---
title: Registro de productos nuevos
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df84a4d3e15035cd956c7612a12069844f5601d2
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-products"></a>Registro de productos nuevos

Los productos son la base de su empresa, las mercancías o servicios con las que comercializa. Cada producto se debe registrar como una ficha de producto.

**Nota**: En Dynamics NAV, se usa el término "producto" para denominar los artículos.

Las fichas de producto contienen la información necesaria para comprar, almacenas, vender, entregar y contabilizar productos.

La ficha de producto puede ser de tipo Inventario o Servicio para especificar si el producto es una unidad física o una unidad de tiempo de mano de obra. Aparte de algunos campos relacionados con los aspectos físicos de un producto, todos los campos de un producto funcionan de la misma forma para los productos de inventario y los servicios. Para obtener más información acerca de la venta de un producto, vea [Procedimiento: Vender productos](sales-how-sell-products.md) o [Procedimiento: Facturar ventas](sales-how-invoice-sales.md)

**Nota**: Si existen plantillas para distintos tipos de producto, aparece una ventana automáticamente cuando se crea una nueva ficha de producto en la que puede seleccionar una plantilla de producto apropiada. Si solo existe una plantilla de producto, las nuevas fichas de producto utilizan siempre esa plantilla.

## <a name="to-create-a-new-item-card"></a>Para crear una nueva ficha de producto.
1. En la página Inicio, elija la acción **Productos** para abrir la lista de productos existentes.  
2. En la ventana **Productos**, seleccione la acción **Nuevo**.

    Si solo existe una plantilla de producto, se abre una nueva ficha de producto con algunos de los campos rellenados con la información de la plantilla.
3. En la ventana **Seleccionar una plantilla para un producto nuevo**, seleccione la plantilla que quiere usar para la nueva ficha de producto.
4. Elija el botón **Aceptar**. Se abre una nueva ficha de producto con algunos de los campos rellenados con la información de la plantilla.
5. Empiece a rellenar o cambiar campos en la ficha de producto según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

En la ficha desplegable **Precios de ventas**, puede observar los precios especiales o los descuentos que concede al cliente por el producto si se cumplen determinados criterios, como, por ejemplo, el cliente, la cantidad de orden mínima o la fecha final. Cada fila representa un precio especial o un descuento de línea. Cada columna representa un criterio aplicable para autorizar el precio especial que se introduzca en el campo **Precio unitario**, o el descuento de línea que se introduzca en el campo **% Descuento línea**. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).

El producto quedará registrado y la ficha de producto está lista para usarse en los documentos de compra y venta.

Si desea usar esta ficha de producto como plantilla cuando cree nuevas fichas de producto, puede guardarla. Para obtener más información, vea la siguiente sección:

## <a name="to-save-the-item-card-as-a-template"></a>Para guardar la ficha de producto como plantilla
1. En la ventana **Ficha de producto**, seleccione la acción **Guardar como plantilla**. La ventana **Plantilla de producto** se abre mostrando la ficha de producto como plantilla.
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Para volver a usar dimensiones en las plantillas, seleccione la acción **Dimensiones**. La ventana **Plantilla de dimensiones** se abre mostrando los códigos de dimensión configurados para el producto.
4. Modifique o introduzca los códigos de dimensión que se aplicarán a nuevas fichas de producto creadas con la plantilla.
5. Cuando haya completado la nueva plantilla de producto, haga clic en el botón **Aceptar**.

La plantilla de producto se agrega a la lista de plantillas de producto, de modo que puede usarla para crear nuevas fichas de producto.

## <a name="see-also"></a>Consulte también
  [Gestionar inventario](inventory-manage-inventory.md)  
  [Gestionar compras](purchasing-manage-purchasing.md)  
  [Gestionar ventas](sales-manage-sales.md)

