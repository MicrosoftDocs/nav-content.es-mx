---
title: "Configuración de centros de trabajo y centros de máquinas"
description: "Una ficha **Centro de trabajo**, organiza los valores fijos y los requisitos del recurso de producción y, por consiguiente, esta ficha rige la salida de la producción realizada en dicho centro de trabajo."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/19/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: ba71815bc7d099b7f600ab828dec579ddbf2265a
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-work-centers-and-machine-centers"></a>Procedimiento: Configuración de centros de trabajo y centros de máquinas
El sistema distingue entre tres tipos de capacidad. Éstas se organizan de manera jerárquica. Cada nivel contiene los niveles subordinados.  

El nivel superior es el grupo de centro de trabajo. Los centros de trabajo se asignan a los grupos de centros de trabajo. Cada centro de trabajo sólo puede pertenecer a un grupo de centros de trabajo.

Puede asignar distintos centros de máquina a cada centro de trabajo. Un centro de máquina sólo puede pertenecer a un centro de trabajo.  

La capacidad planificada de un centro de trabajo se compone de la disponibilidad de los centros de máquina correspondientes y la disponibilidad planificada adicional del centro de trabajo. La disponibilidad planificada del grupo de centros de trabajo es, por tanto, la suma de todas las disponibilidades correspondientes de los centros de máquina y de trabajo.  

La disponibilidad se almacena en los movimientos de calendario. Para configurar centros de trabajo o de máquina, primero debe configurar calendarios de planta. Para obtener más información, consulte [Procedimiento: Crear calendarios de planta](production-how-to-create-work-center-calendars.md).  

## <a name="to-set-up-a-work-center"></a>Para definir centros de trabajo
A continuación se describe principalmente cómo configurar un centro de trabajo. Los pasos para configurar un calendario de centro de máquina son parecidos excepto por la ficha desplegable **Configurar ruta**.  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Centros de trabajo** y, a continuación, seleccione el vínculo relacionado.  
2.  Seleccione la acción **Nuevo**.  
3. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4.  En el campo **Grupo de centro de trabajo**, seleccione el grupo de recursos de nivel superior bajo el que está organizado el centro de trabajo, si es relevante. En la ventana Clientes, seleccione la acción la lista desplegable **Nuevo**.  
5.  Seleccione el campo **Bloqueado** si desea evitar que el centro de trabajo se utilice en cualquier procesamiento. Esto significa que la salida no se puede registrar por un artículo producido en el centro de trabajo. Para obtener más información, consulte [Registro de salida de producción](production-how-to-post-output-quantity.md).
6.  En el campo **Costo unitario directo**, especifique el costo de producir una unidad de medida en este centro de trabajo, sin tener en cuenta los demás elementos de costo. Este costo se suele denominar *costo directo de mano de obra*.  
7.  En el campo **% Costo indirecto**, especifique los costos generales de operación de uso del centro de trabajo como un porcentaje del costo unitario directo. Este importe porcentual se agrega al costo directo al calcular el costo unitario.  
8.  En el campo **Tasa costos generales**, especifique todos los costos del centro de trabajo que no sean de explotación, como los gastos de mantenimiento, como una cantidad absoluta.  

    El campo **Costo unitario** contiene el costo unitario calculado de producir una unidad de medida en este centro de trabajo, incluidos todos los elementos de costo, como se indica a continuación:  

    Costo unitario = Costo unitario directo + (Costo unitario directo x % Costo indirecto) + Tasa de costos generales.  

9.  En el campo **Cálculo costo unitario**, indique si el cálculo anterior debe basarse en la cantidad de tiempo empleado: **Tiempo** o en el número de unidades producidas: **Unidades**.  
10.  Seleccione el campo **Costo unitario específico** si desea definir el costo unitario del centro de trabajo en la línea de ruta donde se va a utilizar. Esto se aplica a las operaciones con unos costos de capacidad radicalmente diferentes de los procesados normalmente en el centro de trabajo.  
11.  En el campo **Método de baja**, seleccione si el registro de salida de este centro de trabajo se debe calcular y registrar manualmente o automáticamente con alguno de los métodos siguientes.  

    |Opción|Descripción|  
    |----------------------------------|---------------------------------------|  
    |**Manual**|El consumo se registra manualmente en el diario de salida o en el diario de producción.|
    |**Anticipada**|El consumo se calcula y se registra automáticamente al lanzar la orden de producción.|  
    |**Atrás**|El consumo se calcula y se registra automáticamente cuando se finaliza la orden de producción.|  

    > [!NOTE]  
    >  Si es necesario, se puede reemplazar el método de baja seleccionado aquí y en la ficha **Producto** para operaciones individuales; para ello, deberá cambiar la configuración en las líneas de ruta.

12.  En el campo **Cód. unidad de medida**, especifique la unidad de tiempo en la que se efectúa el cálculo de costos y la planificación de capacidad del centro de trabajo.
    Para poder controlar el consumo constantemente, primero debe configurar un método de medida. Las unidades que se especifican son unidades básicas. Por ejemplo, el tiempo de proceso se mide en horas y minutos.

    > [!NOTE]  
    > Si decide utilizar Días, recuerde que 1 día = 24 horas, y no 8 (jornada laboral).

13.  En el campo **Capacidad**, puede definir si en el centro de trabajo hay más de una máquina o persona trabajando a la vez. Si la instalación de [!INCLUDE[d365fin](includes/d365fin_md.md)] no tiene la funcionalidad del centro de máquina, el valor de este campo debe ser **1**.  
14.  En el campo **Eficiencia**, especifique el porcentaje de la salida estándar esperada que este centro de trabajo produce realmente. Si especifica **100**, estará indicando que el centro de trabajo tiene una salida real igual que la salida estándar.  
15. Seleccione la casilla verificación **Calendario consolidado** si también utiliza centros de máquina. Esto asegura que los movimientos de calendario se traspasan desde los calendarios de centro de máquina.  
16.  En el campo **Cód. calen. planta**, seleccione un calendario de planta. Para obtener más información, consulte [Procedimiento: Crear calendarios de planta](production-how-to-create-work-center-calendars.md).  
17.  En el campo **Tiempo espera en cola**, puede especificar el intervalo de tiempo fijo que debe transcurrir antes de que se inicie el trabajo asignado en este centro de trabajo. Tenga en cuenta que el tiempo de espera en cola se agrega a otros elementos de tiempo no productivos, como el tiempo de espera y el tiempo de movimiento, que haya definido en las líneas de ruta que utilizan este centro de trabajo.  

## <a name="example---different-machine-centers-assigned-to-a-work-center"></a>Ejemplo: distintos centros de máquina asignados a un centro de trabajo.
Es importante planificar qué capacidades van a componer la capacidad total al configurar los centros de máquina y los centros de trabajo.

Si se asignan distintos centros de máquina (como 210 Mesa de empaquetado 1, 310 Cabina de pintura ...) a un centro de trabajo, resulta significativa la consideración de las capacidades únicas del centro de máquina ya que un fallo en el mismo puede interrumpir todo el proceso. Se pueden introducir los grupos de máquina según su capacidad, pero podrían no incluirse en la planificación. A desactivar el campo **Calendario consolidado**, sólo se asigna la capacidad del centro de trabajo en la planificación y no la del centro de máquina.

Si, no obstante, se combinan centros de máquina idénticos (como 210 Mesa de empaquetado 1 y 220 Mesa de empaquetado 2) en un centro de trabajo, resulta interesante la consideración del centro de trabajo como la suma de los centros de máquina asignados. Por tanto, el centro de trabajo se mostrará con capacidad cero. Al activar el campo **Calendario consolidado**, se asigna la capacidad común al centro de trabajo.

Si las capacidades de los centros de trabajo no van a contribuir a la capacidad total, puede conseguir que lo hagan mediante un factor de eficiencia igual a cero.

## <a name="to-set-up-a-capacity-constrained-machine-or-work-center"></a>Para configurar una capacidad efectiva de una máquina o de un centro de trabajo
Debe configurar los recursos de producción que considera críticos y señalarlos para aceptar una carga finita en lugar de la carga infinita predeterminada que aceptan otros recursos de producción. Un recurso de capacidad restringida puede ser un centro de trabajo o de máquina que ha identificado como cuello de botella y para el que le gustaría establecer una carga limitada y finita.

[!INCLUDE[d365fin](includes/d365fin_md.md)] no admite el control detallado de la planta. Planea una utilización factible de los recursos al proporcionar una programación preliminar, pero no crea ni mantiene automáticamente las programaciones detalladas basadas en prioridades o reglas de optimización.

En la ventana **Recursos de capacidad limitada**, puede establecer una configuración que evite la sobrecarga de los recursos específicos y garantizar que no se deje ninguna capacidad sin asignar si pudiera aumentar el plazo de producción de una orden de producción. En el campo **Amortiguador (% capdad. total)**, puede agregar tiempo de amortiguación a recursos para minimizar la división de operaciones. De este modo, el sistema puede programar la carga en el último día posible superando el porcentaje de carga crítica ligeramente si esto puede reducir el número de operaciones divididas.

Al planificar con recursos de capacidad limitada, el sistema se asegura de que no se cargue ningún recurso por encima de su capacidad definida (carga crítica). Esto se realiza mediante la asignación de cada operación a la franja temporal disponible más próxima. Si la franja temporal no es lo suficientemente amplia para completar toda la operación, la operación se dividirá en dos o más partes que se colocarán en las franjas temporales más próximas disponibles.

1. Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), especifique **Recursos capacidad restringida** y elija el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. Rellene los campos según sea necesario.

> [!NOTE]
> Las operaciones de los centros de máquina o de trabajo que se configuran como recursos restringidos se planificarán siempre de serie. Esto significa que si un recurso restringido tiene varias capacidades, tales capacidades solo se pueden planificar en secuencia, no en paralelo, como sería el caso si el centro de trabajo o de máquina no estuviera configurado como recurso restringido. En un recurso limitado, el campo Capacidad en el centro de trabajo o el centro de máquina es mayor que 1.

> En el caso de división de la operación, el tiempo de configuración se asigna solo una vez, pues se presupone que se realiza algún ajuste manual para optimizar la programación.

## <a name="see-also"></a>Consulte también  
[Cómo crear calendarios de planta](production-how-to-create-work-center-calendars.md)  
[Configuración de fabricación](production-configure-production-processes.md)  
[Fabricación](production-manage-manufacturing.md)    
[Planificación](production-planning.md)   
[Grupos contables inventario](inventory-manage-inventory.md)  
[Compras](purchasing-manage-purchasing.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

