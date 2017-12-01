---
title: Tareas administrativas de Dynamics NAV
description: "Algunas tareas en [!INCLUDE[d365fin](includes/d365fin_md.md)] requieren una administración central y configuración. Consulte cuáles son aprenda y qué hacer."
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 873c8e6f9887ef49d8639851bb64013d985e640e
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a>Configuración y administración de Dynamics NAV
Normalmente, un rol de la empresa se encarga de las tareas de la administración central. El alcance de estas tareas puede depender del tamaño de la empresa, así como de las responsabilidades laborales del administrador. Estas tareas pueden incluir la administración de la sincronización de base de datos de las colas de proyectos y de correo electrónico, la configuración de usuarios, la personalización de la interfaz de usuario y la administración de las claves de cifrado.  

Es importante introducir los valores de configuración correctos desde el principio para el éxito de cualquier nuevo software de negocio. [!INCLUDE[d365fin](includes/d365fin_md.md)] incluye varias guías de configuración que le ayudan a configurar datos fundamentales. Para obtener más información, consulte [Configurar Dynamics NAV](setup.md).

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

Un superusuario o un administrador puede configurar el marco de intercambio de datos para que los usuarios puedan exportar e importar los datos de los archivos de banco y de nómina, por ejemplo, para diferentes procesos de tesorería.  

En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.   

|**Para**|**Vea**|  
|------------|-------------|  
|Agregar usuarios, gestionar permisos y gestionar el acceso a los datos, asignar roles.|[Usuarios, perfiles y áreas de tareas de Dynamics NAV](admin-users-profiles-roles.md)|  
|Realizar un seguimiento de todas las modificaciones directas que realicen los usuarios a los datos de la base de datos para identificar el origen de los errores y de las modificaciones en los datos.|[Registrar cambios de Dynamics NAV](across-log-changes.md)|  
|Apoye las decisiones de configuración con recomendaciones para los campos seleccionados que se saben que potencialmente la solución se haga ineficaz si no se configuran correctamente|[Configurar áreas de aplicación complejas mediante procedimientos recomendados](set-up-complex-application-areas-using-best-practices.md)|  
|Exponga las páginas, las unidades de código y las consultas como servicios web.|[Procedimiento: crear y publicar un servicio web](across-how-publish-web-service.md)|  
|Configure un servidor SMTP para habilitar la comunicación de correo electrónico dentro y fuera de Dynamics NAV.| [Configurar el correo electrónico manualmente o con la configuración asistida](madeira-how-setup-email.md)|  
|Introducir solicitudes únicas o periódicas para ejecutar informes o unidades de código.|[Uso de colas de proyectos para programar tareas](admin-job-queues-schedule-tasks.md)|  
|Administre, elimine, o comprima los documentos|[Administración de documentos](admin-manage-documents.md)|  

## <a name="see-also"></a>Consulte también
[Resumen de las funciones empresariales](madeira-business-functionality.md)  
[Funciones empresariales generales](ui-across-business-areas.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[[!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)  

