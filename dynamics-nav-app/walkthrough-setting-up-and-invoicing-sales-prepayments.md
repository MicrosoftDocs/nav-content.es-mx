---
title: "Tutorial: Configuración y facturación de anticipos de ventas"
description: "Los anticipos son pagos que se facturan y registran en un pedido de anticipo de ventas o compras antes de la facturación final. Es posible que solicite un depósito antes de fabricar productos del pedido, o que solicite un pago antes de enviar productos al cliente. La funcionalidad de anticipos en [!INCLUDE[d365fin](includes/d365fin_md.md)] se utiliza para facturar y cobrar depósitos de los clientes o remitir depósitos a los proveedores. De este modo, puede asegurar que todos los pagos estén registrados contra una factura."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/07/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3076aca3a3b0ef70da183ec55ee1938926d04702
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="walkthrough-setting-up-and-invoicing-sales-prepayments"></a>Tutorial: Configuración y facturación de prepagos de ventas
Los anticipos son pagos que se facturan y registran en un pedido de anticipo de ventas o compras antes de la facturación final. Es posible que solicite un depósito antes de fabricar productos del pedido, o que solicite un pago antes de enviar productos al cliente. La funcionalidad de anticipos en [!INCLUDE[d365fin](includes/d365fin_md.md)] se utiliza para facturar y cobrar depósitos de los clientes o remitir depósitos a los proveedores. De este modo, puede asegurar que todos los pagos estén registrados contra una factura.  

 Los requisitos de los anticipos se pueden definir para un cliente o proveedor, para todos los productos o para algunos. Una vez realizada la configuración necesaria, puede generar facturas de anticipo a partir de pedidos de compra y venta para el importe calculado del anticipo. Puede cambiar los importes predeterminados en la factura según sea necesario. Por ejemplo, puede enviar facturas de anticipo adicionales si es necesario añadir nuevos productos al pedido.  

## <a name="about-this-walkthrough"></a>Acerca de este tutorial  
 En este tutorial aparecen los siguientes ejemplos:  

-   Configuración de anticipos  
-   Creación de un pedido que requiera un anticipo  
-   Creación de una factura de anticipo  
-   Corrección de los requisitos de anticipo en un pedido  
-   Aplicación de anticipos a un pedido  
-   Facturación del importe final en un pedido con anticipo  

### <a name="roles"></a>Roles  
 En este tutorial se incluyen tareas para las siguientes funciones:  

-   Administradora de contabilidad (Felisa)  
-   Procesadora de pedidos (Susana)  
-   Administrador Cobros (Andrés)  

## <a name="story"></a>Historia  
 Felisa es administradora de contabilidad. Ella decisiones sobre qué clientes deben abonar un depósito antes de que se fabriquen o envíen los productos. Felisa configura [!INCLUDE[d365fin](includes/d365fin_md.md)] para calcular automáticamente los anticipos.  

 Susana es procesadora de pedidos de ventas. Cuando un cliente llama para realizar un pedido, ella lo introduce en el sistema mientras el cliente está en el teléfono. Así, puede verificar los precios y las condiciones de pago con el cliente en el momento, y puede realizar ajustes en el pedido mientras negocia con el cliente.  

 Andrés trabaja en el departamento de Cobros, donde registra facturas y pagos.  

 En este ejemplo, Felisa configura los requisitos de anticipo para el cliente Sellafrio, basándose en su historial crediticio, e imparte instrucciones a Susana sobre el modo de gestionar sus pedidos.  

 Cuando el cliente llama, Susana negocia con el cliente hasta alcanzar un acuerdo. Ella puede elegir calcular el anticipo de varias maneras diferentes.  

 Una vez que Susana envíe la factura de anticipo, el cliente solicita un producto adicional. Susana actualiza el pedido y crea una segunda factura de anticipo.  

 Andrés registra el pago del cliente y lo aplica a las facturas; a continuación, envía la factura final.  

## <a name="setting-up-prepayments"></a>Configuración de anticipos  
 Felisa configura el sistema para gestionar los anticipos de los clientes.  

-   Felisa decide utilizar la misma serie numérica para los anticipos que las usadas para la facturación de venta.  
-   Felisa configura el programa para que compruebe si se requieren anticipos antes de la facturación final de los pedidos.  
-   Felisa configura valores predeterminados para un porcentaje de anticipo requerido para ciertos productos y clientes.  

En los siguientes procedimientos, se describe cómo realizar las tareas de Felisa:  

#### <a name="to-set-up-number-series-for-prepayments"></a>Para configurar series numéricas para anticipos  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Conf. ventas y cobros** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ventana **Conf. ventas y cobros**, amplíe la ficha desplegable **Numeración**.  
3.  Verifique que la serie numérica de las facturas de anticipo registradas en el campo **Nº fact. anticipo registrada** sea la misma que para las facturas de venta registradas (**Nº serie fact. registrada**) y que la serie numérica para notas de crédito de anticipo registradas (**Nº nota de crédito anticipo registrada**) sea la misma que para las notas de crédito registradas (**Nº serie nota de crédito registrada**).  

#### <a name="to-block-shipments-for-unpaid-prepayment"></a>Para bloquear envíos por anticipos sin abonar  
1.  En la ventana **Conf. ventas y cobros**, en la ficha desplegable **General**, seleccione la casilla **Comprobar prepago al registrar**.

    Ahora no se puede enviar ni facturar un pedido que tenga un importe de anticipo sin abonar.  

Felisa exige que al cliente 20000 se le facture un prepago del 30% en todos los pedidos, de manera predeterminada. Por lo tanto, escribirá un porcentaje de anticipo predeterminado en la ficha cliente.  

Felisa requiere que a todos los clientes se les facture un depósito del 20% para el producto 1100. El cliente 20000 tiene un mal historial de prepagos, Por lo que requiere un anticipo del 40 % para el cliente 20000 para el producto 1100. En el procedimiento siguiente se ilustra el modo de configurar los porcentajes de anticipo predeterminados.  

#### <a name="to-assign-default-prepayment-percentages-to-customers-and-items"></a>Para asignar porcentajes de anticipo predeterminados a clientes y productos  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.  
2.  Abra la ventana de la ficha del cliente 20000 (Sellafrio).
3.  En el campo **% anticipo**, escriba **30**.  
4.  Elija el botón **Aceptar** para cerrar la ficha de cliente.  
5.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos** y, a continuación, seleccione el vínculo relacionado.  
6.  Abrir la ficha para el cliente 1100.
7.  Seleccione la acción **Porcentajes anticipo**.  
8.  Rellene dos líneas en la ventana **Porcentajes anticipo ventas** como sigue.  

    |**Tipo venta**|**Código ventas**|**Nº producto**|**% anticipo**|  
    |--------------------|--------------------|------------------|----------------------|  
    |**Cliente**|**20000**|**1100**|**40**|  
    |**Todos clientes**||**1100**|**20**|  

    > [!IMPORTANT]  
    >  Dependiendo de su país o región, también debe especificar un código de grupo de impuesto en la ficha desplegable **Facturación** para los productos 1000 y 1100.  

9. Cierre todas las ventanas.  

#### <a name="to-specify-an-account-for-sales-prepayments-in-general-posting-setup"></a>Para especificar una cuenta para los anticipos de ventas en la configuración del registro general  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), introduzca **Configuración grupos contables** y, a continuación, elija el vínculo relacionado.  
2.  Seleccione la línea donde el campo de **General neg. grupo contable** se establece en **EXPORTAR**, y el campo **General producción. grupo contable** se establece en **MERCADERÍA** y, a continuación, seleccione **Editar**.  
3.  En la ventana de **Ficha grupos contabilización**, en el campo **Cuenta anticipo ventas**, especifique la cuenta correspondiente.  
4.  Elija el botón **Aceptar**.  

## <a name="creating-an-order-that-requires-a-prepayment"></a>Creación de un pedido que requiera un anticipo  
 En el siguiente ejemplo, Susana, la procesadora de pedidos, crea un pedido cuando habla con un cliente. Los productos que solicita del cliente requieren un anticipo, y el cliente ha realizado en el pasado algunos pagos con retraso. Por tanto, se ha indicado a Susana para requerir un importe fijo de 2.000 como anticipo en el pedido.  

El cliente solicita poder pagar el 35%, con lo que Susana está de acuerdo. Por tanto, ella cambia el pedido.  

Susana crea la factura de anticipo y la envía al cliente.  

#### <a name="to-create-a-sales-order-with-a-prepayment"></a>Para crear un pedido de venta con anticipo  
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Pedidos de venta** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**.  
3.  En el campo **Venta a-N.º cliente**, seleccione **20000**.  
5.  Acepte el la advertencia de saldo pendiente que se muestra.  
6.  Rellene dos líneas de venta con la siguiente información.  

    |**Escriba**|**Nº**|**Cantidad**|  
    |--------------|-------------|------------------|  
    |**Producto**|**1000**|**1**|  
    |**Producto**|**1100**|**1**|

    Los campos de anticipo de la línea de ventas están ocultos de manera predeterminada, por lo que deberá mostrarlos.  

7. Compruebe que el campo **% anticipo** de la línea con el producto **1000** contiene **30**. El valor predeterminado se ha tomado de la cabecera de venta, que se ha rellenado de la ficha cliente.  

    El campo **% anticipo** de la línea con el producto **1100** contiene **40**. Es el porcentaje que especificó en la ventana **Porcentajes anticipo ventas** para el producto **1100** y el cliente **20000**.  

    Para obtener más información, vea [Procedimiento: configurar anticipos](finance-set-up-prepayments.md).  
8. Seleccione la acción **Estadísticas**.  
9. En la ficha desplegable **Anticipo**, el campo de **Importe línea anticipo sin IVA** contiene **1.560**. Si ahora crea una factura de anticipo para el pedido, ésta será el importe que figura en la factura.  

    En este ejemplo, se ha indicado a Susana que sugiera un anticipo total de 2000 para el pedido.  

    > [!IMPORTANT]  
    >  Dependiendo de su país o región, el paso siguiente puede que no se aplique.  
10. Cambie el importe que aparece en el campo **Importe línea anticipo sin IVA** a **2000** y cierre la ventana.  
11. Consulte el campo **% anticipo** de la líneas de ventas, y verá que se ha calculado de nuevo el valor hasta **40,81625**.  

    El nuevo cálculo incluye todas las líneas con un porcentaje de anticipo superior a 0.  

    Ahora, el cliente pregunta si el porcentaje de anticipo se puede ajustar en 35%. El supervisor de Susana aprueba el cambio.  

12. En la ventana **Pedido venta**, campo **% de anticipo**, introduzca **35**.  
13. En la advertencia que aparece, seleccione el botón de **Sí**. Un índice del 35% será aplicado como el porcentaje de pago para todo el pedido.  
14. Verifique que se han actualizado las líneas en consecuencia.  

## <a name="creating-a-prepayment-invoice"></a>Creación de una factura de anticipo  
Después de escribir los valores de anticipo correctos en el pedido, Susana crea la factura de anticipo y la envía al cliente.  

#### <a name="to-create-a-prepayment-invoice"></a>Para crear una factura de anticipo  

1.  En la ventana **Pedido de ventas**, elija la acción **Registrar factura anticipo**.  

> [!NOTE]  
>  Susana debería seleccionar **Registrar e imprimir factura anticipo** y enviar por correo la factura al cliente.  

## <a name="creating-an-additional-prepayment-invoice"></a>Creación de una factura de anticipo adicional  
Al día siguiente, el cliente llama a Susana y realiza cambios en el pedido. El cliente desea dos unidades del producto 1100. Susana vuelve a abrir y actualiza el pedido y, a continuación, crea una segunda factura de anticipo en el pedido y la envía al cliente.  

#### <a name="to-create-an-additional-prepayment-invoice"></a>Para crear una factura de anticipo adicional  

1.  En la ventana **Pedido de ventas**, elija la acción **Volver a abrir**.  
2.  En la línea del producto **1100**, en el campo **Cantidad**, escriba **2**.  

    Desplácese para ver los campos de anticipo. El campo de **Anticipo Excl de la línea importe. IVA** contiene ahora **630** y el campo **Importe anticipo facturado sin IVA** contiene **315**. Este campo muestra que hay un importe de anticipo adicional que aún no se ha facturado.  
3.  Para registrar una factura para el importe de anticipo adicional, en la pestaña **Acciones**, en el grupo **Registro**, elija **Anticipo** y seleccione **Registrar factura de anticipo**.  

## <a name="applying-the-prepayments"></a>Aplicación de los anticipos  
El cliente paga el importe de anticipo y Andrés, que trabaja en el departamento contable, registra el pago y lo aplica a las facturas de anticipo.  

#### <a name="to-apply-a-payment-to-the-prepayment-invoices"></a>Para aplicar un pago a las facturas de anticipo  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios de recibos de efectivo** y, a continuación, seleccione el vínculo relacionado.  
2.  Rellene una línea de diario con la siguiente información.  

    |Nombre del campo|Escriba|  
    |----------------|-----------|  
    |**Tipo documento**|**Pago**|  
    |**Tipo mov.**|**Cliente**|  
    |**Nº cuenta**|**20000**|  
3. Seleccione la acción **Liquidar movs.**.  
4.  En la ventana **Movs. pendientes cliente**, seleccione la primera factura de anticipo y, a continuación, elija **Marcar id. de liquidación**.  
5.  Repita el paso anterior para el segundo anticipo.  
6.  Elija el botón **Aceptar**.  

    El campo de importe se habrá rellenado ahora con la suma de las dos facturas de anticipo.  

7.  Registre el diario.  

## <a name="invoicing-the-remaining-amount"></a>Facturación del importe restante  
Se ha notificado a Andrés que los productos del pedido se han enviado y que el pedido está listo para su facturación. Andrés crea la factura para el pedido.  

#### <a name="to-invoice-the-remaining-amount"></a>Para facturar el importe restante  
1. Abra el pedido de venta.  
2. Seleccione **Entregar y facturar** y, a continuación, **Aceptar**.  

> [!NOTE]  
>  Normalmente, el departamento de envíos ya habrá registrado el envío.  

Andrés puede ver el historial para verificar que la factura de venta fue creada tal como se previó.  

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Facturas de ventas registradas** y, a continuación, elija el vínculo relacionado.  

## <a name="next-steps"></a>Pasos siguientes  
En este tutorial, ha visto los pasos necesarios para configurar [!INCLUDE[d365fin](includes/d365fin_md.md)] para gestionar anticipos. Ha configurado los porcentajes de anticipo predeterminados en clientes y productos, y también ha utilizado distintos métodos para calcular los anticipos de un pedido. Ha tratado de asignar un importe de anticipo total al pedido y ha calculado el importe de anticipo como un porcentaje del pedido completo.  

También ha registrado una factura de anticipo, creado una segunda factura de anticipo cuando se modificó el pedido y registrado la factura final por el importe restante.  

La función de anticipos en [!INCLUDE[d365fin](includes/d365fin_md.md)] facilita la configuración y la imposición de reglas de anticipo para clientes y productos; además, permite registrar cada pago contra una factura.  

## <a name="see-also"></a>Consulte también  
[Facturación de anticipos](finance-invoice-prepayments.md)  
[Finanzas](finance.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Tutorial de procesos empresariales](walkthrough-business-process-walkthroughs.md)

