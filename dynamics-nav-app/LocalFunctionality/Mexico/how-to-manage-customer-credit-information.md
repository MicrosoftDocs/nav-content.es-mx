---
title: "Procedimiento para administrar información de crédito de los clientes"
description: "En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede agregar comentarios a la información crediticia de los clientes. También puede retener y bloquear clientes que tengan malos antecedentes crediticios antes de realizar el envío o la facturación."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 3c810f54d2788d6465cd76e70548989f9b6651fc
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-manage-customer-credit-information"></a>Procedimiento: Administrar información de crédito de los clientes
En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede agregar comentarios a la información crediticia de los clientes. También puede retener y bloquear clientes que tengan malos antecedentes crediticios antes de realizar el envío o la facturación.  
  
### <a name="to-add-comments-to-customer-credit-information"></a>Para añadir comentarios a la información de crédito de un cliente  
  
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Administración de crédito** y, a continuación, elija el vínculo relacionado.  
  
2.  En el campo **Lista de clientes - Gestión créditos**, seleccione un cliente. En la pestaña **Navegar**, en el grupo **Cliente**, elija **Comentarios**.  
  
3.  En la ventana **Hoja comentarios**, llene los campos como se describe en la tabla siguiente.  
  
    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Fecha**|La fecha del comentario.|  
    |**Comentario**|El comentario sobre el cliente. Puede introducir un máximo de 80 caracteres alfanuméricos.|  
  
4.  Elija el botón **Aceptar**.  
  
### <a name="to-prevent-an-order-from-shipping-or-invoicing"></a>Para impedir que se envíe o se facture un pedido  
  
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Clientes** y, a continuación, elija el vínculo relacionado en **Cobros**.  
  
2.  Seleccione el cliente. En la pestaña **Navegar**, en el grupo **Historial**, elija **Movimientos contables**.  
  
3.  En el campo **Esperar**, introduzca las iniciales del cliente.  
  
4.  Elija el botón **Aceptar**.  
  
    > [!NOTE]  
    >  Debe contar con el permiso de seguridad adecuado para añadir o eliminar el estado en espera en los pedidos de ventas individuales a través del campo **Esperar**.  
  
### <a name="to-block-a-sales-order-for-a-customer"></a>Para bloquear un pedido de ventas de un cliente  
  
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Clientes** y, a continuación, elija el vínculo relacionado en **Cobros**.  
  
2.  Seleccione un cliente. En la pestaña **Inicio**, en el grupo **Administrar**, elija **Editar**.  
  
3.  En la ficha desplegable **General**, en el campo **Bloqueado**, elija una de las siguientes opciones:  
  
    -   **<Blank>**: se permite la transacción de este cliente.  
  
    -   **Envío**: no se pueden crear pedidos ni envíos nuevos para este cliente. Los envíos existentes no facturados aún se pueden facturar.  
  
    -   **Factura**: no se pueden crear pedidos, envíos ni facturas nuevas para este cliente. Los envíos existentes no facturados aún no se pueden facturar.  
  
    -   **Todo**: no se permite ningún asiento para este cliente, incluso pagos.  
  
4.  Elija el botón **Aceptar**.  
  
## <a name="see-also"></a>Consulte también  
 Cliente - Total pedidos   
 [Funcionalidad local de Estados Unidos](../UnitedStates/united-states-local-functionality.md)   
 [Funcionalidad local de Canadá](../Canada/canada-local-functionality.md)   
 [Funcionalidad local de México](mexico-local-functionality.md)
