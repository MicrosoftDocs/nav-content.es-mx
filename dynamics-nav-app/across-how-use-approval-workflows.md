---
title: Aprobar o rechazar documentos en los flujos de trabajo
description: "Solicite, rechace o delegue una aprobación de, por ejemplo, una compra o venta, como parte de un flujo de trabajo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: reject, delegate, request
ms.date: 08/24/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: b0cd3c6c2465c29d5e4710ae2ef13e3f42522245
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-use-approval-workflows"></a>Procedimiento: Usar flujos de trabajo de aprobación
Cuando un registro, como un documento de compra o una ficha de cliente, necesita ser aprobado por alguien de su organización, enviará una solicitud de aprobación como parte de un flujo de trabajo. En función de la configuración del flujo de trabajo, el aprobador adecuado recibirá notificación sobre que el registro requiere su aprobación.

Los flujos de trabajo de aprobación se crean en la ventana **Flujo de trabajo**. Para obtener más información, consulte [Configurar flujos de trabajo](across-set-up-workflows.md).

Además de los flujos de trabajo de aprobación descritos en este tema, puede realizar otras tareas de flujo de trabajo. Para obtener más información, [Uso de flujos de trabajo](across-use-workflows.md).

Los flujos de trabajo de aprobación más importantes para los documentos de compras y ventas, los diarios de pago y las fichas de clientes y productos están listos para iniciar como configuración asistida. Para obtener más información, vea [[!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]](index.md).

## <a name="to-request-approval-of-a-record"></a>Para solicitar la aprobación de un registro
La siguiente tarea se realizado por un usuario de aprobación.

1. En la ventana que presenta el registro, seleccione la acción **Enviar solicitud de aprobación**.
2. Para ver todas sus solicitudes de aprobación, seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Movs. solic. aprobación** y, a continuación, seleccione el vínculo relacionado.  

El estado del movimiento de aprobación se actualiza de **Creado** a **Abierto**. El estado del registro, por ejemplo una factura de compra, se actualiza de **Abierto** a **Pendiente de aprobación** y permanece bloqueado para el procesamiento hasta que todos los aprobadores hayan aprobado el registro.

Cuando el aprobador autoriza el registro, el estado cambia **Lanzados**. Podrá continuar con el resto de tareas del registro.

## <a name="to-cancel-requests-for-approval"></a>Para cancelar solicitudes de aprobación
La siguiente tarea se realizado por un usuario de aprobación con derechos de aprobación.

Puede que un cliente desee cambiar una orden después de que esta se haya enviado para su aprobación. En tal caso, puede cancelar el proceso de aprobación y realizar los cambios necesarios en la orden antes de volver a solicitar aprobación.

- En la ventana que muestra el registro, seleccione la acción **Cancelar solicitud de aprobación**.

Una vez cancelada la solicitud de aprobación, el estado del movimiento de aprobación relacionado cambia a **Cancelado**. El estado del registro también se actualiza de **Aprobación pendiente** a **Abierto**. El proceso de aprobación puede entonces comenzar de nuevo.

## <a name="to-approve-or-reject-requests-for-approval"></a>Para aprobar o rechazar solicitudes de aprobación
La siguiente tarea se realizado por un usuario de aprobación con derechos de aprobación.

Puede procesar solicitudes de aprobación en la ventana **Solicitudes de aprobación**, por ejemplo aprobar múltiples solicitudes a la vez. Alternativamente, puede procesar cada solicitud en el registro relacionado, como en la ventana **Factura de compra**, seleccionando el enlace en la notificación que recibe.

1. Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Solicitudes para aprobar** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione una o varias líneas para el registro o los registros que desee aprobar o rechazar.
3. Seleccione las acciones **Aprobar**, **Rechazar** o **Delegar**.

Una vez aprobado o rechazado un registro, el estado de aprobación en el campo **Estado** cambia **Aprobado** o **Rechazado**.

Si hay configurada una jerarquía de aprobadores, el estado de registro será **Pendiente de aprobación** hasta que todos los aprobadores hayan aprobado el registro. El estado de registro cambiará a **Lanzados**.

Al mismo tiempo, el estado de aprobación cambia de **Creado** a **Abrir** en cuanto se cree una solicitud de aprobación para el registro. Si se rechaza la solicitud, el estado de aprobación cambia **Rechazado**. El estado permanece en **Abrir** o **Rechazado** hasta que todos los aprobadores hayan aprobado la solicitud.

## <a name="to-delegate-requests-for-approval"></a>Para delegar solicitudes de aprobación
La siguiente tarea se realizado por un usuario de aprobación con derechos de aprobación.

Para evitar que los documentos se acumulen o bloqueen el flujo de trabajo, el aprobador y el administrador de aprobación pueden delegar una solicitud de aprobación a un aprobador sustituto. El sustituto puede ser un sustituto designado, el aprobador directo o el administrador de aprobaciones, en ese orden de prioridad. Esta característica se utiliza normalmente si un aprobador se encuentra fuera de la oficina y no puede aprobar solicitudes antes de la fecha de vencimiento.

1. Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Solicitudes para aprobar** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione una o varias líneas de las solicitudes de aprobación que desea delegar a un aprobador sustituto y, a continuación, seleccione la acción **Delegar**.

Se envía una notificación para aprobar la solicitud al aprobador sustituto.

## <a name="to-manage-overdue-approval-requests"></a>Para gestionar solicitudes de aprobación vencidas
La siguiente tarea se realizado por un usuario de aprobación con derechos de aprobación.

Deberá recordar de forma periódica a los usuarios de flujo de trabajo de aprobación las solicitudes de aprobación vencidas en las que deben realizar alguna acción. Para ello se utiliza la función **Enviar notificaciones de aprobación vencidas**.

La función **Enviar notificaciones de aprobación vencidas** buscará todas las solicitudes de aprobación pendientes que hayan vencido. Cada aprobador que tenga al menos un movimiento de aprobación vencido recibirá una notificación con la lista de todas las solicitudes de aprobación vencidas. Esta notificación también se envía al aprobador y a todos los solicitantes de las aprobaciones vencidas. Esto resulta útil si el movimiento de aprobación vencido se debe delegar a un sustituto.

1. Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Solicitudes de aprobación vencidas** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Solicitudes de aprobación vencidas**, seleccione la acción **Seleccionar solicitudes de aprobación vencidas**.

## <a name="see-also"></a>Consulte también
[Ccial](sales-manage-sales.md)    
[Documentos entrantes](across-income-documents.md)  
[Compras](purchasing-manage-purchasing.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

