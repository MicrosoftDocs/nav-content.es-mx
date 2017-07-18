---
title: 'Procedimiento: Registrar precios y descuentos de compra'
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
ms.openlocfilehash: f99bb0aeef2c25048b0da3e0476ae2d612bff562
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-record-purchase-prices-and-discounts"></a>Procedimiento: Registrar precios y descuentos de compra
Es necesario definir los diferentes acuerdos de precios y descuentos que se aplican al comprar a distintos proveedores de modo que se apliquen las reglas y los valores acordados a los documentos de compra que se crean para los proveedores.

Respecto a los precios, puede tener una precio especial de compra insertado en las líneas de compra si existe una cierta combinación de proveedor, producto, cantidad mínima, unidad de medida o fecha de inicio o de fin.

Respecto a los descuentos, puede configurar y usar dos tipos de descuentos de compra:

|Tipo de descuento |Descripción |
|--------------|------------|
|**Descuento línea compra**|Un importe de descuento que está insertado en las líneas de compra si existe una cierta combinación de proveedor, producto, cantidad mínima, unidad de medida o fecha de inicio o de fin. Funciona igual que para los precios de compra.|
|**Descuento en factura**|Un porcentaje de descuento que se resta del total del documento si el importe de todas las líneas de un documento de compra supera cierto límite.|

Puesto que los descuentos de línea y los precios de compra se basan en una combinación de producto y proveedor, también se puede introducir esta combinación desde la ficha de producto en la que se definen las reglas y los valores. Para obtener más información, vea [Procedimiento: Registrar nuevos productos](inventory-how-register-new-products.md).

## <a name="to-set-up-a-special-purchase-price-for-a-vendor"></a>Para configurar un precio de compra especial para un proveedor
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proveedores** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de proveedor correspondiente y, a continuación, elija la acción **Precios**.

    El campo **Tipo de compras** se rellena previamente con el campo **Proveedor** y el campo **Código de compre** se rellena con el número del proveedor.
3. Rellene los campos de la línea como sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
4. Rellene una línea para cada combinación por la que el proveedor le garantiza un descuento de compra.

## <a name="to-set-up-a-line-discount-for-a-vendor"></a>Para configurar un descuento de línea para un proveedor
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proveedores** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de proveedor correspondiente y, a continuación, elija la acción **Dto. línea**.

    El campo **Tipo de compras** se rellena previamente con el campo **Proveedor** y el campo **Código de compre** se rellena con el número del proveedor.
3. Rellene los campos de la línea como sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
4. Rellene una línea para cada combinación por la que el proveedor le garantiza un descuento de compra.

## <a name="to-set-up-an-invoice-discount-for-a-vendor"></a>Para configurar términos de descuento en factura para un proveedor:
Una vez su proveedor le haya informado de que descuentos en factura garantizan, introduzca el código de descuento en las fichas de cliente y especifique los términos de cada código.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proveedores** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de un proveedor que pueda obtener descuentos en factura.
3. En el campo **Código descuento factura**, seleccione un código para los términos relevantes de la factura con descuentos que usará para calcular los descuentos en facturas para el proveedor.

    **Nota**: Los códigos de descuento en factura se representan por las fichas existentes del proveedor. Lo que permite asignar rápidamente las condiciones de descuento en factura a proveedores realizando el picking del nombre de otros proveedores con los mismos términos.

    Configure de nuevo los términos de descuento en factura para compras.
4. En la ventana **Ficha de proveedor**, seleccione la acción **Descuento factura**. Aparecerá la ventana **Dtos. factura proveedor**.
5. En el campo **Código divisa**, introduzca el código de una divisa que se aplique a los términos de descuento en factura en la línea. Deje el campo en blanco para establecer condiciones de descuento de factura en USD.
6. En el campo **Importe mínimo**, escriba el importe mínimo que deba tener una factura para optar al descuento.
7. En el campo **% descuento**, introduzca el descuento en la factura como un porcentaje del importe de la factura.
8. Repita los pasos 5 a 7 para cada divisa para la que el proveedor va a recibir un descuento diferente de factura.

El descuento en factura está configurado y asignado el proveedor en cuestión. En el momento que selecciona el código de proveedor en el campo **Código de descuento de factura** en las fichas de proveedores, se asigna el mismo descuento en factura a ese proveedor.

## <a name="see-also"></a>Consulte también  
[Configurar compra](purchasing-setup-purchasing.md)  
[Gestionar compras](purchasing-manage-purchasing.md)

