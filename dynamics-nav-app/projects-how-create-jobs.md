---
title: "Creación de proyectos"
author: SorenGP
ms.custom: na
ms.date: 11/01/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: df34c435d07e9526cb4d93e2bfc30162258ba957
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-create-jobs"></a>Creación de proyectos
Cuando inicie un proyecto nuevo, debe crear una ficha de proyecto con tareas de proyecto integradas y líneas de planificación de proyecto, estructuradas en dos niveles.  

La primera capa consta de tareas de proyecto. Debe crear al menos una tarea de proyecto por cada proyecto porque todos los registros hacen referencia a una tarea de proyecto. Tener al menos una tarea de proyecto en su proyecto le permite configurar líneas de planificación de proyecto y registrar el consumo en el proyecto.

La segunda capa consta de líneas de planificación de proyecto, que especifican el uso detallado de los recursos, productos y diversos gastos de contabilidad general.

La estructura de capas permite dividir el proyecto en tareas más pequeñas y usar detalles más específicos en el presupuesto, las ofertas y el registro. Además, le ofrece información de cómo está progresando un proyecto. Por ejemplo, puede hacer un seguimiento de si está alcanzando los hitos señalados o si va encaminado a cumplir las expectativas de presupuesto.

**Nota**: La acción **Proyecto nuevo** en el área de trabajo **Administrador del proyecto** inicia una configuración asistida que le guía por los pasos para crear un proyecto con tareas integradas y líneas de planificación. El procedimiento siguiente describe cómo realizar los pasos manualmente.

## <a name="to-create-a-job-card"></a>Para crear una ficha de proyecto
Cree una ficha de proyecto y, a continuación, cree las líneas de tarea de proyecto y las líneas de planificación de proyecto para el mismo.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proyectos** y, a continuación, seleccione el vínculo relacionado.  
2. Elija la acción **Nuevo** y, a continuación, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Para especificar el proyecto con la información sobre otros proyectos, elija la acción **Copiar proyecto**, rellene los campos según sea necesario y, a continuación, elija el botón **Aceptar**.

**NOTA**: Si utiliza las hojas de horas con su proyecto, también debe designar una persona responsable. Esta persona puede aprobar las hojas de horas para las tareas de empleados asociadas con el proyecto. Para obtener más información, vea [Configuración de hojas de horas](projects-how-setup-time-sheets.md).

## <a name="to-create-tasks-for-a-job"></a>Para crear tareas para un proyecto  
Una parte clave de la creación de un proyecto es especificar las diversas tareas que conlleva. Para ello, debe agregar líneas nuevas en la ficha desplegable **Tareas** de la ventana **Ficha de proyecto**, con una tarea por línea. Cada proyecto debe tener al menos una tarea.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proyectos** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de un proyecto relevante.
3. En la ficha desplegable **Tareas**, rellene los campos según sea necesario en una nueva línea.
4. Para indentar las tareas y crear una jerarquía, elija la acción **Tareas** y, a continuación, elija la acción **Indentar tareas proyecto**.
5. Repita los pasos 3 y 4 para todas las tareas que necesite para el proyecto.
6. Para especificar las tareas de proyecto con la información sobre otras tareas de proyecto, elija la acción **Copiar tareas de proyecto desde**, rellene los campos según sea necesario y, a continuación, elija el botón **Aceptar**.

## <a name="to-create-planning-lines-for-a-job"></a>Para crear líneas de planificación de un proyecto  
Puede redefinir las nuevas tareas de proyecto como líneas de planificación de proyecto. Una línea de planificación puede utilizarse para capturar cualquier información de un proyecto que desee supervisar. Puede utilizar líneas de planificación para agregar información como qué recursos son necesarios o para capturar productos que sean necesarios para realizar el proyecto. Por ejemplo, si tiene una tarea para obtener la aprobación de clientes para un proyecto, puede asociar esa tarea con líneas de planificación para productos como reuniones con clientes y asignar un recurso.  

Una línea de planificación de un proyecto puede ser de uno de los siguientes tipos.  

|Tipo|Descripción|
|----|-----------|
|**Ppto**|Proporciona consumo y costes del proyecto estimados, habitualmente en un contrato de tiempo y tipo de proyecto. Las líneas de planificación de este tipo no pueden facturarse.|
|**Facturable**|Proporciona una facturación estimada al cliente, habitualmente en un proyecto de precio fijo.|
|**Presupuesto y facturable**|Proporciona el uso presupuestado igual a lo que se desea facturar.|  

**Nota**. A medida que especifique información en las líneas de planificación del proyecto, la información de costos se completará automáticamente. Por ejemplo, el costo, el precio y el descuento de los recursos y productos se basan inicialmente en la información que se haya definido en las ficha de recurso y la ficha de producto.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proyectos** y, a continuación, seleccione el vínculo relacionado.
2. Abra una ficha de un proyecto relevante.
3. Seleccione una tarea de proyecto cuyos campo **Tipo tarea proyecto** contenga **Registrar** y seleccione la acción **Líneas planificación proyecto**.  
4. En la ventana **Líneas planificación proyecto**, en una línea nueva, rellene los campos según sea necesario.
5. Repita los pasos 3 y 4 para todas líneas de planificación que necesita para la tarea de proyecto.

## <a name="see-also"></a>Consulte también
[Administrar proyectos](projects-manage-projects.md)  
[Finanzas](finance-setup.md)  
[Gestionar compras](purchasing-manage-purchasing.md)         
[Gestionar ventas](sales-manage-sales.md)      
[Trabajar con Dynamics NAV](ui-work-product.md)  
