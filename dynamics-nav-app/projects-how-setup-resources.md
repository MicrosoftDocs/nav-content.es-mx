---
title: "Configuración de recursos"
author: SorenGP
ms.custom: na
ms.date: 12/14/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 72f5304e6a69a736c9df2cbb9ca64c5f3c5261a2
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-resources"></a>Configuración de recursos
Para administrar correctamente las actividades de recursos, debe configurar los recursos, y los costos y los precios relacionados. Las reglas de precios, descuentos y factores de costo relacionadas con el proyecto se configuran en la tarjeta respectiva. Puede especificar los costos y los precios de recursos individuales, de grupos de recursos o de todos los recursos disponibles de la empresa.

Si se utilizan o venden recursos en un proyecto, los precios y costes asociados con ellos se recuperan de la información que haya configurado.

Debe especificar el importe predeterminado por hora cuando se crea el recurso. Por ejemplo, si utiliza un equipo específico en un proyecto durante cinco horas, el proyecto se calcularía en función del importe por hora.

## <a name="to-set-up-a-resource"></a>Para configurar un recurso
Cree una ficha por cada recurso que desee utilizar en los proyectos.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Recursos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.  

## <a name="to-set-up-a-resource-group"></a>Para configurar una familia de recursos
En una familia de recursos se pueden combinar varios recursos. En ellas se agrupan todas las capacidades y presupuestos cada uno de los recursos. Las capacidades de las familias de recursos pueden introducirse también independientemente de los valores acumulados o bien sumándolas a estos.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Familias de recursos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. Rellene los campos según sea necesario.

## <a name="to-set-capacity-for-a-resource"></a>Para configurar la capacidad de un recurso 
Para calcular cuánto tiempo puede dedicar un recurso a los trabajos, su capacidad debe definirse primero como tiempo disponible por periodo en el calendario de trabajo. Utilice esta configuración para rellenar las líneas de planificación del proyecto que contienen el recurso. Para obtener más información, vea [Creación de proyectos](projects-how-create-jobs.md).

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Recursos** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de recurso correspondiente y, a continuación, elija la acción **Capacidad recurso**.
3. En la ventana **Capacidad del recurso**, en el campo **Ver**, especifique la duración del periodo, por ejemplo **Día**, que se muestra en columnas en la ficha desplegable **Matriz capacidad recurso**.
4. Para cada recurso de una línea, especifique por cada periodo de las columnas el número de horas que el recurso está disponible.
5. Opcionalmente, para detallar la capacidad semanal de recursos en una fecha inicial y final, elija la acción **Establecer capacidad**.
6. En la ventana **Config. capacidad recurso**, rellene los campos según sea necesario.
7. Elija la acción **Actualizar capacidad**. La ventana **Capacidad recurso** se actualiza con la capacidad introducida.
8. Cierre la ventana.

## <a name="to-set-up-alternate-resource-costs"></a>Para configurar precio costos recursos alternativos
Además del costo especificado en la ficha de recurso, puede configurar costos alternativos para cada recurso. Por ejemplo, si paga a un empleado un sueldo por horas superior por el trabajo en horas extraordinarias, puede configurar un precio costos recursos para el sueldo por horas extraordinarias. El costo alternativo que configuró para el recurso anulará el costo que consta en la ficha de recurso cuando use el recurso en el diario de recursos.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Recursos** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione el recurso para el que desee configurar varios costes alternativos y, a continuación, elija la acción **Costes**.  
3. En la ventana **Precio de coste del recurso**, rellene los campos en una línea según sea necesario.  
4. Repita el paso 3 para el precio costos recursos alternativo que desee configurar.

**Nota**. Para configurar precios de coste de recursos aplicables a todos los recursos y familias de recursos, abra la ventana **Precio de coste del recurso** y rellene los campos.

## <a name="to-set-up-alternate-resource-prices"></a>Para configurar precios de recursos alternativos  
Además del precio especificado en la tarjeta de recurso, puede configurar precios alternativos para cada recurso. Estos precios alternativos pueden ser condicionales. Pueden depender de si el recurso se consume con un proyecto o tipo de trabajo determinado.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Recursos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el recurso para el que desee configurar varios precios alternativos y, a continuación, elija la acción **Precios**.
3. En la ventana **Precio de venta del recurso**, rellene los campos en una línea según sea necesario.
4. Repita el paso 3 para cada precio de venta de recurso alternativo que desee configurar.

## <a name="see-also"></a>Consulte también
[Configuración de la administración de proyectos](projects-setup-projects.md)  
[Administrar proyectos](projects-manage-projects.md)  
[Finanzas](finance-setup.md)  
[Gestionar compras](purchasing-manage-purchasing.md)         
[Gestionar ventas](sales-manage-sales.md)      
[Trabajar con Dynamics NAV](ui-work-product.md)  

