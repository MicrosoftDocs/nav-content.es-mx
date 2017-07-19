---
title: 'Procedimiento: Registrar precios y descuentos de ventas'
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
ms.openlocfilehash: 2d6438108fb2c36bb6f0d44efddc053bd628d068
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-record-sales-prices-and-discounts"></a>Procedimiento: Registrar precios y descuentos de ventas
Es necesario definir los diferentes acuerdos de precios y descuentos que se aplican al vender a distintos clientes de modo que se apliquen las reglas y los valores acordados a los documentos de venta que se crean para los clientes.

Respecto a los precios, puede tener una precio especial de venta insertado en las líneas de venta si existe una cierta combinación de cliente, producto, cantidad mínima, unidad de medida o fecha de inicio o de fin.

Respecto a los descuentos, puede configurar y usar dos tipos de descuentos de ventas:

|Tipo de descuento |Descripción |
|--------------|------------|
|**Descuento línea venta**|Un importe de descuento que está insertado en las líneas de venta si existe una cierta combinación de cliente, producto, cantidad mínima, unidad de medida o fecha de inicio o de fin. Funciona igual que para los precios de venta.|
|**Descuento en factura**|Un porcentaje de descuento que se resta del total del documento si el importe de todas las líneas de un documento de venta supera cierto límite.|

Dado que los descuentos de línea de venta y los precios de venta se basan en una combinación de producto y cliente, también puede basar esta configuración en la ficha del producto al que se aplican las reglas y valores.

## <a name="to-set-up-a-sales-price-for-a-customer"></a>Para configurar un precio de venta para un cliente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Clientes** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de cliente correspondiente y, a continuación, elija la acción **Precios**.

    El campo **Tipo venta** se rellena con **Cliente**y el campo **Código ventas** se rellena con el número de cliente.
3. Rellene los campos de la línea como sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
4. Rellene una línea para cada combinación que aplicará un precio de venta especial al cliente.

## <a name="to-set-up-a-sales-line-discount-for-a-customer"></a>Para configurar un descuento de línea de venta para un cliente
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Clientes** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de cliente correspondiente y, a continuación, elija la acción **Dto. línea**.

    El campo **Tipo venta** se rellena con **Cliente**y el campo **Código ventas** se rellena con el número de cliente.
3.  Rellene los campos de la línea como sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
4. Rellene una línea para cada combinación que aplicará un descuento de línea de venta al cliente.

## <a name="to-set-up-an-invoice-discount-for-a-customer"></a>Para configurar un descuento en factura para un cliente
Una vez que haya determinado los clientes que pueden obtener descuentos en factura, introduzca el código de descuento en factura en las fichas de cliente y especifique los términos de cada código.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Clientes** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de un cliente que pueda obtener descuentos en factura.
3. En el campo **Código descuento factura**, seleccione un código para los términos relevantes de la factura con descuentos que usará para calcular los descuentos en facturas para el cliente.

    **Nota**: Los códigos de descuento en factura se representan por las fichas existentes del cliente. Lo que permite asignar rápidamente las condiciones de descuento en factura a clientes realizando el picking del nombre de otros clientes con los mismos términos.

    Configure de nuevo los términos de descuento en factura para ventas.
4. En la ventana **Ficha de cliente**, seleccione la acción **Descuento factura**. Aparecerá la ventana **Dtos. factura cliente**.
5. En el campo **Código divisa**, introduzca el código de una divisa que se aplique a los términos de descuento en factura en la línea. Deje el campo en blanco para establecer condiciones de descuento de factura en USD.
6. En el campo **Importe mínimo**, escriba el importe mínimo que deba tener una factura para optar al descuento.
7. En el campo **% descuento**, introduzca el descuento en la factura como un porcentaje del importe de la factura.
8. Repita los pasos del 5 al 7 para cada divisa que el cliente reciba un descuento diferente de factura.

El descuento en factura ahora está configurado y asignado al cliente en cuestión. Al seleccionar el código del cliente en el campo **Cód. dto. factura** en otras fichas de cliente, se asigna el mismo descuento en factura a estos clientes.

## <a name="see-also"></a>Consulte también  
[Configurar ventas](sales-setup-sales.md)  
[Gestionar ventas](sales-manage-sales.md)

