---
title: Registro de clientes nuevos
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
ms.openlocfilehash: 191a9d0b38425c2e36400050afa4fa89ccd2556a
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-register-new-customers"></a>Registro de clientes nuevos
Los clientes son el origen de los ingresos. Cada cliente a quien venda debe estar registrado como ficha de cliente.

Antes de que pueda registrar nuevos clientes, debe configurar varios códigos de ventas que pueda seleccionar al rellenar fichas de cliente. Para obtener más información, consulte [Configurar ventas](sales-setup-sales.md).

Las fichas de cliente contienen la información necesaria para vender productos al cliente. Para obtener más información, consulte [Procedimiento: Facturar ventas](sales-how-invoice-sales.md) y [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

**Nota**: Si existen plantillas de cliente para distintos tipos de cliente, una ventana aparece automáticamente cuando se crea una nueva ficha de cliente en la que puede seleccionar una plantilla de cliente correspondiente. Si solo existe una plantilla de cliente, las nuevas fichas de cliente utilizan siempre esa plantilla.

## <a name="to-create-a-new-customer-card"></a>Para crear una nueva ficha cliente.
1. En la página Inicio, seleccione la acción **Clientes** para abrir la lista de clientes existentes.  
2. En la ventana **Clientes**, seleccione la acción **Nuevo**.

    Si solo existe una plantilla de cliente, una nueva ficha de cliente se abre con algunos campos rellenados con la información de la plantilla.

    Si existe más de una plantilla de cliente, se abre una ventana desde la que puede seleccionar una plantilla de cliente. En ese caso, siga los dos pasos siguientes.
3. En la ventana **Seleccionar una plantilla para un cliente nuevo**, seleccione la plantilla que quiere usar para la nueva ficha de cliente.
4. Elija el botón **Aceptar**. Una nueva ficha de cliente se abre con algunos campos completados con la información de la plantilla.  
5. Empiece a rellenar o cambiar campos en la ficha de cliente según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

En la ficha desplegable **Precios venta y descuentos línea ventas**, puede observar los precios especiales o los descuentos que concede al cliente si se cumplen determinados criterios, como, por ejemplo, el producto, la cantidad de orden mínima o la fecha final. Cada fila representa un precio especial o un descuento de línea. Cada columna representa un criterio aplicable para autorizar el precio especial que se introduzca en el campo **Precio unitario**, o el descuento de línea que se introduzca en el campo **% Descuento línea**. Para más información, vea [Registrar acuerdos de pago, descuentos y precios de venta](sales-how-record-sales-price-discount-payment-agreements.md).

El cliente estará registrado y la ficha de cliente está lista para usarse en los documentos de venta.

Si desea usar esta ficha de cliente como plantilla cuando cree nuevas fichas de cliente, puede guardarla. Para obtener más información, vea la siguiente sección:

## <a name="to-save-the-customer-card-as-a-template"></a>Para guardar la ficha de cliente como una plantilla
1. En la ventana **Ficha de cliente**, seleccione la acción **Guardar como plantilla**. La ventana **Plantilla cliente** se abre mostrando la ficha de cliente como plantilla.
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Para volver a usar dimensiones en las plantillas, seleccione la acción **Dimensiones**. La ventana **Plantilla de dimensiones** se abre mostrando los códigos de dimensión configurados para el cliente.
4. Modifique o introduzca los códigos de dimensión que se aplicarán a nuevas fichas de cliente creadas con la plantilla.  
5. Cuando haya completado la nueva plantilla de cliente, seleccione el botón de **Aceptar**.

La plantilla de cliente se agrega a la lista de plantillas de cliente, de modo que puede usarla para crear nuevas fichas de cliente.

## <a name="see-also"></a>Consulte también  
[Gestionar ventas](sales-manage-sales.md)    
[Configurar ventas](sales-setup-sales.md)    
[Trabajar con Dynamics NAV](ui-work-product.md)

