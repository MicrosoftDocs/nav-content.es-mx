---
title: "Cómo configurar impuesto sobre servicios e impuesto a las compras"
description: "La definición de impuesto de las ventas comprende los impuestos que pagan las empresas por usar productos"
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: c1e8aba3c1732fe4eef7031c5488af520aebf0bd
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-use-tax-and-purchase-tax"></a>Cómo: configurar impuesto sobre servicios e impuesto a las compras
La definición de impuesto de las ventas comprende los impuestos que pagan las empresas por usar productos:  

- Impuesto sobre servicios (Estados Unidos): el impuesto sobre servicios es un impuesto de las ventas de los Estados Unidos que se paga sobre los productos que compra y usa una empresa para sí misma en lugar de venderlos a un tercero. La empresa debe pagar el impuesto de las ventas correspondiente a tales productos al gobierno, como impuesto sobre servicios.  
- Impuesto a las compras (Canadá): el impuesto a las compras es un impuesto de las ventas de Canadá que debe pagar una empresa sobre los productos que compra a los proveedores. Cuando una empresa compra productos que usará para sí misma, el proveedor cobra el impuesto de las ventas apropiado correspondiente a los productos.  

## <a name="to-set-up-use-tax-for-a-purchase-order"></a>Para configurar el impuesto sobre servicios para un pedido de compra  
1.  Seleccione ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos compra** y, a continuación, elija el vínculo relacionado en **Procesamiento de pedidos**.  
2.  En la ventana **Pedidos compra**, de la pestaña **Inicio**, del grupo **Nuevo**, elija **Nuevo**.  
3.  En la ficha desplegable **Líneas**, rellene los campos como sea necesario. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
4.  En la ficha desplegable **Facturación**, llene los campos como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Sujeto a impuesto**|Seleccione este campo para configurar los impuestos a los que está sujeto. **Importante:** Este campo está disponible en la ventana **Cab. compra**, pero no se muestra de forma predeterminada. Para seleccionar este campo, primero debe agregar la columna que lo muestra. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |**Cód. área impuesto**|El código de área de impuesto del proveedor. **Importante:** Este campo está disponible en la ventana **Cab. compra**, pero no se muestra de forma predeterminada. Para seleccionar este campo, primero debe agregar la columna que lo muestra. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |**Nº exención fisc.**|El número de exención fiscal de la empresa. Puede introducir un máximo de 30 caracteres alfanuméricos. **Importante:** Este campo está disponible en la ventana **Cab. compra**, pero no se muestra de forma predeterminada. Para seleccionar este campo, primero debe agregar la columna que lo muestra. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
    |**Cód. área impuesto provincial**|El código de impuesto de la provincia. **Importante:** Este campo está disponible en la ventana **Cab. compra**, pero no se muestra de forma predeterminada. Para seleccionar este campo, primero debe agregar la columna que lo muestra. [!INCLUDE[bp_customize](../../includes/bp_customize_md.md)]|  
5.  Elija el botón **Aceptar**.  

## <a name="to-set-up-use-tax-details"></a>Para configurar detalles del impuesto sobre servicios  
1.  Elija el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Detalles de impuesto** y, a continuación, elija el vínculo relacionado.  
2.  En la ventana **Detalles impuesto**, elija la acción **Nuevo**.  
3.  En la ventana **Nuevo - Detalles impuesto**, llene los campos como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Cód. jurisdicción impuesto**|El código de jurisdicción de impuesto correspondiente al movimiento del detalle de impuesto.|  
    |**Cód. grupo impuesto**|El código de grupo de impuesto correspondiente al movimiento del detalle de impuesto.|  
    |**Tipo impto.**|**Impuestos de las ventas y sobre servicios**: para aplicar ambos impuestos a las ventas y al uso al movimiento del detalle de impuesto.<br /><br /> –o–<br /><br /> **Impto. consumo**: para aplicar el impuesto al consumo al movimiento del detalle de impuesto.<br /><br /> –o–<br /><br /> **Sólo impto. ventas**: para aplicar el impuesto de las ventas solamente al movimiento del detalle de impuesto.<br /><br /> –o–<br /><br /> **Sólo impto. sobre servicios**: para aplicar el impuesto sobre servicios solamente al movimiento del detalle de impuesto.|  
4.  Elija el botón **Aceptar**.  

## <a name="to-set-up-purchase-tax-for-a-company"></a>Para configurar el impuesto a las compras para una empresa  
1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Información de la empresa** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ventana **Información de empresa**, en la ficha desplegable **Impuesto**, rellene los campos tal como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Cód. área impuesto**|El código de área de impuestos de la empresa. Este código se usa junto con el campo de código de grupo de impuestos y el campo **Sujeto a impuesto** para buscar la información necesaria para calcular el impuesto de las ventas.|  
    |**Nº exención fisc.**|El número de exención fiscal de la empresa. Puede introducir un máximo de 30 caracteres alfanuméricos.|  
    |**Cód. área impuesto provincial**|El código de impuesto de la provincia.|  
3.  Elija el botón **Aceptar**.  

## <a name="to-set-up-purchase-tax-for-a-location"></a>Para configurar el impuesto a las compras para un almacén  
1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Almacenes** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ventana **Ubicaciones**, seleccione la ubicación necesaria y, a continuación, elija el botón **Editar**.  
3.  En la ficha desplegable **General**, llene los campos como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**No usar para cálculo de impuestos**|Seleccione este campo para especificar si la información de impuesto incluida en este registro de almacén se usará para calcular el impuesto de las ventas sobre los documentos de compra.|  
    |**Cód. área impuesto**|El código de área de impuestos del almacén. Este código se usa junto con el campo de código de grupo de impuestos y el campo **Sujeto a impuesto** para buscar la información necesaria para calcular el impuesto de las ventas.|  
    |**Nº exención fisc.**|El número de exención fiscal de la empresa. Puede introducir un máximo de 30 caracteres alfanuméricos.|  
    |**Cód. área impuesto provincial**|El código de impuesto de la provincia.|  
4.  Elija el botón **Aceptar**.  

## <a name="to-set-up-purchase-tax-for-non-recoverable-tax"></a>Para configurar el impuesto a las compras para impuestos irrecuperables  
1.  Elija el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Detalles de impuesto** y, a continuación, elija el vínculo relacionado.  
2.  En la ventana **Detalles impuesto**, elija la acción **Nuevo**.  
3.  Active la casilla de verificación **Gastar/Capitalizar**.  

    > [!NOTE]  
    >  Se debe activar esta casilla de verificación si el impuesto pagado es irrecuperable.  
4.  Elija el botón **Aceptar**.  

## <a name="see-also"></a>Consulte también
[Funcionalidad local de México](mexico-local-functionality.md)  
[Informes del impuesto de venta en México](mexico-sales-tax.md)  
[Finanzas](../../finance.md)  
[Configurar las finanzas](../../finance.md)  

