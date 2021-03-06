---
title: Procedimiento para configurar y publicar servicios web de KPI basados en estructuras de cuentas
description: "En la ventana **Configuración de servicio web KPI de estructura de cuentas**, se configura cómo mostrar los datos de KPI de la estructura de cuentas y en qué estructuras de cuentas específicas se deben basar los KPI."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/08/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: b45fe6e1e5d4e5be00a6e8a34b7b4fea39b5d75b
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-and-publish-kpi-web-services-based-on-account-schedules"></a>Procedimiento: configurar y publicar un servicio web KPI que se basa en estructuras de cuentas
En la ventana**Configuración de servicio web KPI de estructura de cuentas**, se configura cómo mostrar los datos de KPI de la estructura de cuentas y en qué estructuras de cuentas específicas se deben basar los KPI. Cuando elige el botón **Publicar servicio Web**, los datos especificados KPI de esquema de cuentas se agregan a la lista de servicios Web publicados en la ventana **Servicios Web**.  

## <a name="to-set-up-and-publish-a-kpi-web-service-that-is-based-on-account-schedules"></a>Para configurar y publicar un servicio web KPI que se basa en estructuras de cuentas  

1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Configuración de servicio web KPI de estructura de cuentas** y, a continuación, seleccione el vínculo relacionado.  
2.  En la ficha desplegable **General**, llene los campos como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Inicio de valores previstos**|Especifique en qué momento se muestran los valores previstos en el gráfico KPI del esquema de cuentas.<br /><br /> Los valores previstos se recuperan del presupuesto de contabilidad general que seleccione en el campo **Nombre presupuesto contable**. **Nota**: Para obtener KPI que muestren cifras previstas tras una fecha determinada y cifras reales antes de la fecha, puede cambiar el campo **Permitir registro desde** en la ventana **Configuración de contabilidad**. Para obtener más información, consulte Permitir registrar desde.|  
    |**Nombres pptos. contabilidad**|Especifique el nombre del presupuesto de contabilidad que proporciona los valores previstos en el servicio web KPI de esquema de cuentas.|  
    |**Periodo**|Especifique el periodo en el que se basa el servicio web KPI de esquema de cuentas.|  
    |**Ver por**|Especifiqué en qué intervalo de tiempo se muestra el KPI de esquema de cuentas.|  
    |**Nombre del servicio web**|Especifique el nombre del servicio web KPI de esquema de cuentas.<br /><br /> Este nombre aparecerá en el campo **Nombre servicio** de la ventana **Servicios web**.|  

    Continúe especificando una o varias estructuras de cuentas que desee publicar como servicio web de KPI según la configuración que ha realizado en la tabla anterior.  

3.  En la ficha desplegable **Estructuras de cuentas**, rellene los campos tal como se describe en la tabla siguiente.  

    |Campo|Descripción|  
    |---------------------------------|---------------------------------------|  
    |**Nombre Estructura de Cuentas**|Especifique la estructura de cuentas en el que se basa el servicio web KPI.|  
    |**Descripción esq. cuentas**|Especifique la descripción de la estructura de cuentas en la que se basa el servicio web KPI.|  

4.  Repita el paso 3 para todas las estructuras de cuentas en las que desea basar el servicio web KPI de estructura de cuentas.  
5.  Para ver o editar la estructura de cuentas seleccionada, en la ficha desplegable **Estructura de cuentas**, elija **Editar estructura de cuentas**.  
6.  Para ver los datos de KPI de la estructura de cuentas que ha configurado, elija la acción **Servicio web KPI de estructura de cuentas**.  
7.  Para publicar el servicio Web KPI de esquema de cuentas, elija la acción **Publicar servicio Web**. El servicio web se agrega a la lista de servicios web publicados en la ventana **Servicios web**.  

    > [!NOTE]  
    >  También puede publicar el servicio web KPI seleccionando el objeto de la página **Configuración de servicio web KPI de estructura de cuentas** de la ventana **Servicios web**. Para obtener más información, consulte [Cómo publicar un servicio Web](https://msdn.microsoft.com/en-us/library/dd338978.aspx) en MSDN.  

## <a name="see-also"></a>Consulte también  
[Inteligencia empresarial](bi.md)  
[Finanzas](finance.md)  
[Configurar las finanzas](finance-setup-finance.md)  
[Libro mayor y plan de cuentas](finance-general-ledger.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

