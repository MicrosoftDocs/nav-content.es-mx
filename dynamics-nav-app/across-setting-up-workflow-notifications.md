---
title: "Configuración de notificaciones de flujos de trabajo"
description: "Muchas respuestas del flujo de trabajo corresponden a la notificación al usuario de un evento que se ha producido y en el que deben realizar una acción. Por ejemplo, en un paso del flujo de trabajo, el evento puede ser que el usuario 1 apruebe la solicitud de un registro nuevo y la respuesta que se envíe una notificación al usuario 2, el aprobador. En el siguiente paso del flujo de trabajo, el evento puede ser que el usuario 2 apruebe el registro y la respuesta que se envíe una notificación al usuario 3 para iniciar el procesamiento relacionado del registro aprobado. En el caso de los pasos del flujo de trabajo relacionados con la aprobación, cada notificación está vinculada a un movimiento de aprobación."
documentationcenter: 
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
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2c3e64a5d343bad026ba5417f18861ef6417dae3
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="setting-up-workflow-notifications"></a>Configuración de notificaciones de flujos de trabajo
Muchas respuestas del flujo de trabajo corresponden a la notificación al usuario de un evento que se ha producido y en el que deben realizar una acción. Por ejemplo, en un paso del flujo de trabajo, el evento puede ser que el usuario 1 apruebe la solicitud de un registro nuevo y la respuesta que se envíe una notificación al usuario 2, el aprobador. En el siguiente paso del flujo de trabajo, el evento puede ser que el usuario 2 apruebe el registro y la respuesta que se envíe una notificación al usuario 3 para iniciar el procesamiento relacionado del registro aprobado. En el caso de los pasos del flujo de trabajo relacionados con la aprobación, cada notificación está vinculada a un movimiento de aprobación. Para obtener más información, consulte [Flujo de trabajo](across-workflow.md).  

> [!NOTE]  
>  La versión genérica de [!INCLUDE[d365fin](includes/d365fin_md.md)] utiliza las notificaciones como correo electrónico y como notas internas.  

> [!IMPORTANT]  
>  Todas las notificaciones de flujo de trabajo se envían a través de una cola de proyectos. Asegúrese de que la cola de trabajos esté en su solución. Para obtener más información, consulte [Uso de colas de proyectos para programar tareas](admin-job-queues-schedule-tasks.md).

Se configuran distintos aspectos de las notificaciones de flujo de trabajo en los lugares siguientes:  

1.  Para los flujos de trabajo de aprobación, configure los destinatarios de las notificaciones del flujo de trabajo rellenando una línea en la ventana **Config. usuario aprobación** para cada usuario que participe en el flujo de trabajo. Por ejemplo, si se ha especificado el usuario 2 en el campo **Id. aprobador** en la línea del usuario 1, la notificación de solicitud de aprobación se envía el usuario 1. Para obtener más información, vea . Para obtener más información, vea [Procedimiento: Configurar usuarios de aprobación](across-how-to-set-up-approval-users.md).  
2.  Para definir cuándo y cómo los usuarios reciben notificaciones de flujo de trabajo debe rellenarse la ventana **Programación de notificación** para cada usuario del flujo de trabajo. Para obtener más información, consulte [Procedimiento: Especificar cómo y cuándo recibir notificaciones](across-how-to-specify-when-and-how-to-receive-notifications.md).  
3.  Configure el contenido general y el diseño de las notificaciones, incluidas las notificaciones acerca de respuestas de vencimiento del flujo de trabajo, configurando para ello plantillas de notificación en la ventana **Plantillas notificación**. Puede utilizar las plantillas predeterminadas que se ofrecen con [!INCLUDE[d365fin](includes/d365fin_md.md)].  
4.  Deberá configurarse el contenido específico y las reglas para una notificación de flujo de trabajo al crear el flujo de trabajo en cuestión. Para ello, seleccione las opciones correspondientes en la ventana **Opciones de respuesta de flujo de trabajo** para la respuesta de flujo de trabajo que represente la notificación. Para obtener más información, consulte el paso 9 en [Procedimiento: Crear flujos de trabajo](across-how-to-create-workflows.md).  

## <a name="see-also"></a>Consulte también  
 [Procedimiento: Configurar usuarios de aprobación](across-how-to-set-up-approval-users.md)   
 [Procedimiento: Configurar usuarios de flujo de trabajo](across-how-to-set-up-workflow-users.md)   
 [Procedimiento: Especificar cómo y cuándo recibir notificaciones](across-how-to-specify-when-and-how-to-receive-notifications.md)   
 [Procedimiento: Crear flujos de trabajo](across-how-to-create-workflows.md)   
 [Procedimiento: Administrar las plantillas de notificación](across-how-to-manage-notification-templates.md)   
 [Uso de colas de proyectos para programar tareas](admin-job-queues-schedule-tasks.md)   
 [Configurar el correo electrónico](madeira-how-setup-email.md)   
 [Tutorial: Configuración y uso de un flujo de trabajo de aprobación de compra](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
 [Flujo de trabajo](across-workflow.md)   

