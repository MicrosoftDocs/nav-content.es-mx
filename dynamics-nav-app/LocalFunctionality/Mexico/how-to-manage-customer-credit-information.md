---
title: "Procedimiento para administrar información de crédito de los clientes"
description: "En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede agregar comentarios a la información crediticia de los clientes. También puede retener y bloquear clientes que tengan malos antecedentes crediticios antes de realizar el envío o la facturación."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/11/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 6c64fdb5e8078c91480fffe06caf0340f60cd295
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-manage-customer-credit-information"></a>Procedimiento: Administrar información de crédito de los clientes
En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede agregar comentarios a la información crediticia de los clientes. También puede retener y bloquear clientes que tengan malos antecedentes crediticios antes de realizar el envío o la facturación.  

## <a name="to-add-comments-to-customer-credit-information"></a>Para añadir comentarios a la información de crédito de un cliente  
1.  Elija el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Administración de crédito** y, a continuación, elija el vínculo relacionado.  
2.  En la ventana **Lista de clientes - Gestión créditos**, seleccione un cliente y, a continuación, elija la acción **Comentarios**.  
3.  En la ventana **Hoja comentarios**, llene los campos como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Fecha**|La fecha del comentario.|  
    |**Comentario**|El comentario sobre el cliente. Puede introducir un máximo de 80 caracteres alfanuméricos.|  

4.  Elija el botón **Aceptar**.  

## <a name="to-prevent-an-order-from-shipping-or-invoicing"></a>Para impedir que se envíe o se facture un pedido  
1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione el cliente y, a continuación, elija la acción **Movimientos**.  
3.  En el campo **Esperar**, introduzca las iniciales del cliente.  
4.  Elija el botón **Aceptar**.  

    > [!NOTE]  
    >  Debe contar con el permiso de seguridad adecuado para añadir o eliminar el estado en espera en los pedidos de ventas individuales a través del campo **Esperar**.  

## <a name="to-block-a-sales-order-for-a-customer"></a>Para bloquear un pedido de ventas de un cliente  
1.  Seleccione el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione un cliente y, a continuación, elija la acción **Editar**.  
3.  En la ficha desplegable **General**, en el campo **Bloqueado**, elija una de las siguientes opciones:  

    -   **<Blank>**: se permite la transacción de este cliente.  
    -   **Envío**: no se pueden crear pedidos ni envíos nuevos para este cliente. Los envíos existentes no facturados aún se pueden facturar.  
    -   **Factura**: no se pueden crear pedidos, envíos ni facturas nuevas para este cliente. Los envíos existentes no facturados aún no se pueden facturar.  
    -   **Todo**: no se permite ningún asiento para este cliente, incluso pagos.  
4.  Elija el botón **Aceptar**.  

## <a name="see-also"></a>Consulte también  
[Funcionalidad local de México](mexico-local-functionality.md)  
[Finanzas](../../finance.md)  
[Configurar las finanzas](../../finance.md)

