---
title: Usar abonos de compra para procesar devoluciones o cancelaciones
description: "Explica cómo crear y registrar una nota de crédito de compra cuando se desean devolver productos a un proveedor o cancelar servicios comprados."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: cancel, undo, correct
ms.date: 08/03/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3f0c187e2cd2520854fe69f3896f6d7311cdc2da
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-process-purchase-returns-or-cancellations"></a>Procesamiento de devoluciones de compra o cancelaciones
Si desea devolver productos al proveedor o cancelar servicios comprados, puede crear y registrar una nota de crédito de compras que especifique el cambio solicitado en relación a la factura de compra original. Para incluir la información correcta de la factura de compras, puede crear el abono de compra directamente de la factura de compra contabilizada o puede crear un nuevo abono de compra con información de factura copiada.

Si necesita más control del proceso de devolución de compras, como documentos de almacén para el manejo de artículos o una mejor descripción al recibir elementos de varios documentos de compras con una sola devolución, puede crear órdenes de devolución de compras. Un pedido de devolución de compra emite automáticamente un abono de compra relacionado. Para obtener más información, consulte la sección "Crear un pedido de devolución de compra basado en uno o más documentos de compra registrados".

> [!NOTE]  
>   Si una factura de compra registrada aún no se ha pagado, puede utilizar las funciones **Corregir** o **Cancelar** en la factura de compra registrada para revertir automáticamente las transacciones correspondientes. Estas funciones solo funcionan para las facturas sin pagar y no admiten devoluciones o cancelaciones parciales. Para obtener más información, vea [Procedimiento: Corregir o cancelar las facturas de compra sin abonar](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)

Normalmente, se crea una nota de crédito de compra o un pedido de devolución de compra como resultado de una nota de crédito enviada por un proveedor. El pedido de abono de compra o de devolución de compra funciona como la documentación interna del proceso de abono para fines de estadísticas o control de envíos de los productos relacionados.

El cambio puede relacionarse con todos los productos en la factura de compra original o solo algunos de los productos. Por consiguiente, puede devolver productos parcialmente recibidos o exigir un reembolso parcial de los servicios recibidos. En ese caso, debe editar la información de las líneas del abono de compra o en el pedido de devolución de compras.

Además de la original factura de compra registrada, puede liquidar el abono de compra o el pedido de devolución de compra a otros documentos de compra, por ejemplo otra factura de compra registrada, porque usted también devuelve los productos entregados con dicha factura.

El registro de la nota de crédito también revertirá cualquier cargo de producto que se hubiera asignado al documento registrado, de modo que los movimientos de valor del producto serán los mismos de antes que se asignara el cargo de producto.

## <a name="inventory-costing"></a>Inventario y valoración
Para conservar la correcta valuación de inventarios, normalmente desea tomar los artículos devueltos del inventario al costo unitario en el que fueron comprados, no al costo unitario actual. Esto se denomina reversión de costo exacto.

Existen dos funciones para asignar la reversión de costo exacta automáticamente.  

|Función|Descripción|  
|------------------|---------------------------------------|  
|Función**Revertir líneas documentos registrados** en la ventana **Pedido dev. compra**|Copia una o varias líneas de documentos registrados para revertirlas en el pedido de devolución de compra. Para obtener más información, consulte la sección "Para crear un pedido de devolución de compras y el abono de compra relacionado, para uno o varias facturas de compras registradas".|  
|Función**Copiar líneas** en las ventanas **Abono compra** y **Pedido dev. compra**|Copia la cabecera y las líneas de un documento registrado que se revertirá.<br /><br /> Requiere que se active la casilla de verificación **Coste exacto devol. obligatorio** en la ventana **Configuración compras y pagos**.|

Para asignar manualmente la reversión del costo exacto, debe elegir el campo **Liq. movimiento prod.** en cualquier tipo de línea de documento, y seleccionar el número del movimiento de compra original. De este modo la nota de crédito de compra o el pedido de devolución de compra se vincula al movimiento de compra original y se asegura que el producto se value con el costo unitario original.

Para obtener más información, consulte [Detalles de diseño: valoración de inventario](design-details-inventory-costing.md).

## <a name="to-create-a-purchase-credit-memo-from-a-posted-purchase-invoice"></a>Para crear una nota de crédito de compra desde una factura de compra registrada.
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Histórico facturas compra** y, a continuación, seleccione el vínculo relacionado.  
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

## <a name="to-create-a-purchase-credit-memo-by-copying-a-posted-purchase-invoice"></a>Crear un nuevo abono de compra copiando una factura de compra registrada.
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Abonos de compra** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo** para abrir una nota de crédito de compra vacía.
3. En el campo **Proveedor**, escriba el nombre de un proveedor existente.
4. Elija la acción **Copiar documento**.
5. En la ventana **Copiar documento de compra**, en el campo **Tipo de documento**, seleccione el campo **Factura registrada**.
6. Elija el campo **Nº documento** para abrir la ventana **Histórico facturas compra** y seleccione la factura de compra registrada que contiene las líenas que desea revertir.
7. Seleccione la casilla **Recalcular líneas** si desea que las líneas de factura de compra registradas copiadas se actualicen con los cambios en el precio y el costo unitario del producto desde que la factura fue registrada.
8. Elija el botón **Aceptar**. Las líneas de factura copiadas se insertarán en la nota de crédito de compra.
9. Complete la nota de crédito de compra como se explica en la sección "Para crear una nota de crédito de compra a partir de una factura de compra registrada" en este tema.

## <a name="to-create-a-purchase-return-order-based-on-one-or-more-a-posted-purchase-documents"></a>Crear un pedido de devolución de compras basado en uno o más documentos de compras registrados
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de devolución de compra** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione la acción **Nuevo**.  
3. Rellen los campos de la ficha desplegable **General**.
4. En la ficha desplegable **Líneas**, rellene las líneas manualmente o copie la información de otros documentos para rellenar las líneas automáticamente:

    - Utilice la función **Revertir líneas documentos registrados:** para copiar una o más líneas de documentos registrados de uno o varios documentos registrados. Esta función revierte siempre exactamente los costos a partir de la línea de documento registrada. Esta función se describe en los pasos siguientes.    
    - Puede utilizar la función **Copiar documento** para copiar un documento existente al pedido de devolución. Utilice esta función para copiar el documento completo. Puede ser un documento registrado o un documento que todavía no se registró. Esta función solo permite invertir el costo exacto cuando está seleccionada la casilla **Costo exacto devol. obligatorio** en la ventana **Configuración ventas y cobros**.  

4. Elija la acción **Revertir líneas documentos registrados**.
5. En la parte superior de la ventana **Líneas doc. compras contabilizadas**, seleccione el campo **Mostrar sólo líneas reversibles** si solo desea ver las líneas con cantidades que aún no se han devuelto. Por ejemplo, si la cantidad de una factura de compra registrada ya se ha devuelto, puede que no desee incluir esa cantidad en un nuevo documento de devolución de compra.

    > [!NOTE]  
    >  Este campo solo funciona para líneas de facturas, envíos y recepciones registradas, no para líneas de notas de crédito o devoluciones registradas.  

    En la parte izquierda de la ventana, se listan los diferentes tipos de documento y el número que aparece entre corchetes muestra el número de documentos que hay disponible del tipo en concreto.

6. En el campo **Filtro de tipo de documento**, seleccione el tipo de líneas de documento registrado que desea utilizar.  
7. Seleccione las líneas que desea copiar en el nuevo documento.  

    > [!NOTE]  
    >  Si utiliza Ctrl+E para seleccionar todas las líneas, se copiarán todas las líneas incluidas en el filtro definido, pero se ignorará el filtro **Mostrar sólo líneas reversibles**. Por ejemplo, imagine que ha filtrado las líneas en un número de documento determinado con dos líneas, una de las cuales ya se ha devuelto. Aunque el campo **Mostrar sólo líneas reversibles** esté seleccionado, si presiona Ctrl+E para copiar todas las líneas, se copiarán las dos líneas, en lugar de copiar solamente aquella que aún no se ha revertido.  

8. Seleccione **Aceptar** para copiar las líneas en el documento nuevo.  

    Tendrán lugar los siguientes procesos:  

    -   Para las líneas de documentos registrados del tipo **Producto**, se crea una nueva línea de documento que es una copia de la línea del documento registrado, con la cantidad que aún no se ha revertido. El campo **Liquid. por nº orden producto** se rellena según corresponda con el número de movimiento de producto correspondiente a la línea del documento registrado.  

    -   Para las líneas de documentos registrados que no sean del tipo **Producto**, como los cargos de producto, se crea una nueva línea de documento que es una copia de la línea del documento registrado original.  

    -   Calcula el campo **Costo unitario ($)** de la nueva línea a partir de los costos de los movimientos de producto correspondientes.  

    -   Si el documento copiado es un envío, una recepción, una recepción de devolución o un envío de devolución registrados, el precio unitario se calcula automáticamente a partir de la ficha del producto.  

    -   Si el documento copiado es una factura o una nota de crédito registrada, se copian el precio unitario, los descuentos de factura y los descuentos de línea de la línea del documento registrado.  

    -   Si la línea del documento registrado contiene líneas de seguimiento de productos, el programa rellena el campo **Liq. por nº orden producto** de dichas líneas de seguimiento con los números de movimiento de producto correspondientes de las líneas de seguimiento de productos registradas.  

     Cuando se copia desde una factura o nota de crédito registradas, el sistema copia los descuentos de factura y de línea válidos en el momento de registrar ese documento desde la línea del documento registrado a la nueva línea de documento. Sin embargo, tenga en cuenta que si se activa la opción **Calc. dto. factura** en la ventana **Confi&guración compras y pagos**, el descuento en factura se volverá a calcular cuando registre una línea de documento nueva. Por lo tanto, el importe de la nueva línea puede ser distinto del importe de la línea del documento registrado, dependiendo del nuevo cálculo de descuento de factura.  

    > [!NOTE]  
    >  Si ya se ha revertido, vendido o consumido parte de la cantidad de la línea del documento registrado, se crea una línea sólo para la cantidad que queda en inventario o que no se ha devuelto. Si ya se ha revertido toda la cantidad de la línea del documento registrado, no se crea una nueva línea de documento.  
    >   
    >  Si el flujo de los artículos en el documento registrado coincide con el del nuevo documento, se crea una copia de la línea del documento registrado original en el nuevo documento. El campo **Liq. movimiento prod.** no se rellenó porque, en este caso, la reversión de costo exacto no es posible. Por ejemplo, si utiliza la función **Revertir líneas documentos registrados** para obtener una línea de una nota de crédito de compras registrada para un nueva nota de crédito de compras, solo se copia la línea del Nota crédito regis original en el nuevo abono.  

8. En la ventana **Pedido dev. compra**, en el campo **Cód. auditoría dev.** de cada línea, seleccione el motivo de la devolución.
9. Seleccione la acción **Registrar**.

## <a name="to-create-a-replacement-purchase-order-from-a-purchase-return-order"></a>Para crear un pedido de sustitución a partir de un pedido de devolución de compra
Puede estar de acuerdo con el proveedor en que compense un producto comprado, sustituyendo el producto. El producto de sustitución puede ser el mismo u otro distinto. Esta situación se puede dar si el proveedor le envió por error un producto equivocado.  
1.  En la ventana **Pedido dev. compra** para un proceso de devolución activo, en una línea vacía, haga un movimiento negativo para el producto de reposición insertando un importe negativo en el campo **Cantidad** .  
2. Seleccione la acción **Mover líneas negativas**.  
3. En la ventana **Mover líneas compra negativas**, rellene los campos en una línea según sea necesario.
4. Elija el botón **Aceptar**. La línea negativa se elimina del pedido de devolución de compra y se crea un nuevo pedido de compra. Para obtener más información, consulte [Procedimiento: Registrar compras](purchasing-how-record-purchases.md).  

## <a name="to-create-a-purchase-allowance"></a>Para crear una deducción de compra  
Si los productos que recibe del proveedor no son satisfactorios, como cuando están dañados o son del color o tamaño incorrecto, es posible que el proveedor le ofrezca una deducción de compra.  

Puede registrar este costo reducido de compra como un cargo de producto en una nota de crédito o pedido de devolución, y vincularlo a la remisión registrada. A continuación se describe esto para un pedido de devolución de compra, pero los mismos pasos se aplican a un abono de copra.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Abonos de compra** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo** para abrir una nota de crédito de compra vacía.  
3.  Rellene la cabecera de nota de crédito con información acerca del proveedor que le envió la deducción de compra.  
4. Seleccione **Cargo (prod.)** en el campo **Tipo** de la ficha desplegable **Líneas**.  
5.  En el campo **N.º**, seleccione el valor de cargo apropiado de producto.  

    Puede que desee crear un número de costo de producto especial para cubrir las deducciones de compra.  
6.  En el campo **Cantidad**, introduzca **1**.  
7.  En el campo **Precio compra**, introduzca el importe de la deducción de compra.  
8.  Asigne la deducción de compra como un cargo de producto a los productos de la remisión registrada. Para obtener más información, consulte [Procedimiento: Utilizar los cargos de producto a cuenta para los costos comerciales adicionales](payables-how-assign-item-charges.md). Una vez asignada la deducción, vuelva a la ventana **Abono de compra**.

Cuando registre el pedido de devolución de compra, la deducción de compra se añadirá al importe del movimiento de compra correspondiente. De este modo podrá mantener la precisión de la valuación de inventarios.  

## <a name="to-combine-return-shipments"></a>Para combinar envíos devueltos  
Si desea devolver los productos cubiertos por distintos pedidos de devolución de compra al mismo vendedor, entonces puede utilizar la función **Combinar envíos devueltos**.  

Cuando envíe los productos, registre los pedidos de devolución de compras relacionados como enviados para crear envíos de devolución de compra registrados.  

Cuando vaya a facturar estos productos, en lugar de facturar cada pedido de devolución de compra por separado, cree una nota de crédito de compras y copie automáticamente las líneas de envío de devolución de compra registradas en este documento. Luego registre la nota de crédito de compra y facture con comodidad todos los pedidos de devolución de compra pendientes al mismo tiempo.  

Cuando se combinan envíos devueltos en una nota de crédito y se registran, se crea una nota de crédito de compras registrada para las líneas facturadas. El campo **Cantidad facturada** del pedido de devolución de compra de origen se actualiza en función de la cantidad facturada. Sin embargo, este pedido de devolución de compra original no se elimina, aunque se haya recibido y facturado por completo, por lo que debe eliminar el pedido de devolución de compra manualmente.

> [!NOTE]  
> El procedimiento siguiente supone que hay varios pedidos de devolución de compra para el proveedor y que están registrados como enviados.     

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Abonos de compra** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**.  
3. En la ficha desplegable **General**, rellene los campos como sea necesario.  
4. Elija la acción **Tomar líns. envío dev.**.  
5.  Seleccione las diversas líneas de envío de devolución que desee incluir en la factura.  

    Si ha seleccionado una línea de envío de devolución incorrecta o desea comenzar desde el principio, solo elimine las líneas de la nota de crédito de compras y vuelva a usar la función **Tomar líns. envío devol.**  
6.  Seleccione la acción **Registrar**.  

### <a name="to-remove-open-purchase-return-orders-after-combined-return-shipment-posting"></a>Para eliminar pedidos de devolución de compra abiertos después del registro del envío de devolución  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Eliminar dev. compras fact...** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene los campos según sea necesario y, a continuación, haga clic en el botón **Aceptar**.  
3.  También puede eliminar los pedidos de devolución de compra individuales manualmente.

## <a name="see-also"></a>Consulte también
[Compras](purchasing-manage-purchasing.md)  
[Registro de compras](purchasing-how-record-purchases.md)  
[Corregir o cancelar las facturas de compra sin abonar](purchasing-how-correct-cancel-unpaid-purchase-invoices.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

