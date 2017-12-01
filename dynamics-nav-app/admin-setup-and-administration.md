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
ms.sourcegitcommit: 1dfba8b14019991c95f40ffd5f7fbaed5df414eb
ms.openlocfilehash: 3ddb647d28a4065be248a265316b38e8d37d28c2
ms.contentlocale: es-mx
ms.lasthandoff: 12/01/2017

---
# <a name="setup-and-administration-in-dynamics-nav"></a><span data-ttu-id="37f62-104">Configuración y administración de Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="37f62-104">Setup and Administration in Dynamics NAV</span></span>
<span data-ttu-id="37f62-105">Normalmente, un rol de la empresa se encarga de las tareas de la administración central.</span><span class="sxs-lookup"><span data-stu-id="37f62-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="37f62-106">El alcance de estas tareas puede depender del tamaño de la empresa, así como de las responsabilidades laborales del administrador.</span><span class="sxs-lookup"><span data-stu-id="37f62-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="37f62-107">Estas tareas pueden incluir la administración de la sincronización de base de datos de las colas de proyectos y de correo electrónico, la configuración de usuarios, la personalización de la interfaz de usuario y la administración de las claves de cifrado.</span><span class="sxs-lookup"><span data-stu-id="37f62-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="37f62-108">Es importante introducir los valores de configuración correctos desde el principio para el éxito de cualquier nuevo software de negocio.</span><span class="sxs-lookup"><span data-stu-id="37f62-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="37f62-109"> incluye varias guías de configuración que le ayudan a configurar datos fundamentales.</span><span class="sxs-lookup"><span data-stu-id="37f62-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="37f62-110">Para obtener más información, consulte [Configurar Dynamics NAV](setup.md).</span><span class="sxs-lookup"><span data-stu-id="37f62-110">For more information, see [Setting Up Dynamics NAV](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="37f62-111">Un superusuario o un administrador puede configurar el marco de intercambio de datos para que los usuarios puedan exportar e importar los datos de los archivos de banco y de nómina, por ejemplo, para diferentes procesos de tesorería.</span><span class="sxs-lookup"><span data-stu-id="37f62-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="37f62-112">En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.</span><span class="sxs-lookup"><span data-stu-id="37f62-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="37f62-113">**Para**</span><span class="sxs-lookup"><span data-stu-id="37f62-113">**To**</span></span>|<span data-ttu-id="37f62-114">**Vea**</span><span class="sxs-lookup"><span data-stu-id="37f62-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="37f62-115">Agregar usuarios, gestionar permisos y gestionar el acceso a los datos, asignar roles.</span><span class="sxs-lookup"><span data-stu-id="37f62-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="37f62-116">Usuarios, perfiles y áreas de tareas de Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="37f62-116">Users, Profiles, and Role Centers in Dynamics NAV</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="37f62-117">Realizar un seguimiento de todas las modificaciones directas que realicen los usuarios a los datos de la base de datos para identificar el origen de los errores y de las modificaciones en los datos.</span><span class="sxs-lookup"><span data-stu-id="37f62-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="37f62-118">Registrar cambios de Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="37f62-118">Logging Changes in Dynamics NAV</span></span>](across-log-changes.md)|  
|<span data-ttu-id="37f62-119">Apoye las decisiones de configuración con recomendaciones para los campos seleccionados que se saben que potencialmente la solución se haga ineficaz si no se configuran correctamente</span><span class="sxs-lookup"><span data-stu-id="37f62-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="37f62-120">Configurar áreas de aplicación complejas mediante procedimientos recomendados</span><span class="sxs-lookup"><span data-stu-id="37f62-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="37f62-121">Exponga las páginas, las unidades de código y las consultas como servicios web.</span><span class="sxs-lookup"><span data-stu-id="37f62-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="37f62-122">Procedimiento: crear y publicar un servicio web</span><span class="sxs-lookup"><span data-stu-id="37f62-122">How to: Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="37f62-123">Configure un servidor SMTP para habilitar la comunicación de correo electrónico dentro y fuera de Dynamics NAV.</span><span class="sxs-lookup"><span data-stu-id="37f62-123">Set up an SMTP server to enable e-mail communication in and out of Dynamics NAV</span></span>| [<span data-ttu-id="37f62-124">Configurar el correo electrónico manualmente o con la configuración asistida</span><span class="sxs-lookup"><span data-stu-id="37f62-124">How to: Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="37f62-125">Introducir solicitudes únicas o periódicas para ejecutar informes o unidades de código.</span><span class="sxs-lookup"><span data-stu-id="37f62-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="37f62-126">Uso de colas de proyectos para programar tareas</span><span class="sxs-lookup"><span data-stu-id="37f62-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="37f62-127">Administre, elimine, o comprima los documentos</span><span class="sxs-lookup"><span data-stu-id="37f62-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="37f62-128">Administración de documentos</span><span class="sxs-lookup"><span data-stu-id="37f62-128">Manage Documents</span></span>](admin-manage-documents.md)|  

## <a name="see-also"></a><span data-ttu-id="37f62-129">Consulte también</span><span class="sxs-lookup"><span data-stu-id="37f62-129">See Also</span></span>
[<span data-ttu-id="37f62-130">Resumen de las funciones empresariales</span><span class="sxs-lookup"><span data-stu-id="37f62-130">Overview of Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="37f62-131">Funciones empresariales generales</span><span class="sxs-lookup"><span data-stu-id="37f62-131">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="37f62-132">[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="37f62-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="37f62-133">[[!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="37f62-133">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

