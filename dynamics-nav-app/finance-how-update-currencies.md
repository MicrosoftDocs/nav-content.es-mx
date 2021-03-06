---
title: Actualizar tipos cambio divisa
description: "Para utilizar varias divisas en su empresa, puede configurar un código para cada divisa y usar un servicio externo para el tipo de cambio, como Yahoo."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: multiple currencies, Yahoo
ms.date: 07/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 50603747629eee61f9bdaed900dcfc0dfc96ab3b
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-update-currency-exchange-rates"></a>Actualizar los tipos de cambio de divisa
Debe configurar un código por cada una de las divisas usadas en caso de que las operaciones de compra y venta se realicen en una divisa que no sea la divisa local (DL), tenga cobros y pagos en otras divisas o registre las transacciones de contabilidad en diferentes divisas.  

Las empresas trabajan cada vez en un mayor número de países o regiones, por lo que es muy importante que puedan crear informes financieros en más de una divisa y revisarlos. El programa admite el uso de varias divisas. En el programa, la contabilidad se configura con la divisa local ($), y se configura otra divisa como divisa adicional, a la que se asigna un tipo de cambio.  

 Mediante la designación de una segunda divisa como información divisa adicional, [!INCLUDE[d365fin](includes/d365fin_md.md)] registrará automáticamente los importes tanto en $ como en la divisa adicional en todos los movimientos de contabilidad y en otros movimientos, por ejemplo los del IVA. Cuando se calculan los importes de un movimiento de contabilidad en una divisa adicional, la información de la ventana **Tipos cambio divisa** se utiliza para buscar el tipo de cambio que corresponda.  

> [!WARNING]  
>  La funcionalidad de divisa adicional NO se debe usar como base de las traducciones de resultados financieros. No es una herramienta que pueda realizar traducciones de resultados financieros de las subsidiarias extranjeras como parte de la consolidación de una empresa. Esta funcionalidad ofrece únicamente la posibilidad de preparar los informes en otra divisa, como si dicha divisa fuera la divisa local de la empresa.

## <a name="adjusting-exchange-rates"></a>Ajustar los tipos de cambio  
Puesto que los tipos de cambio fluctúan constantemente, los equivalentes de la divisa adicional del sistema se deben ajustar regularmente. Si no se llevan a cabo estos ajustes, los importes que se hayan convertido desde divisas extranjeras (o adicionales) y registrado en contabilidad en la divisa local pueden ser erróneos. Además, los movimientos diarios registrados antes de que se introduzca el tipo de cambio del día en el programa se tienen que actualizar una vez que se haya introducido esta información. El proceso Ajustar tipos de cambio se usa para ajustar los tipos de cambio de los movimientos de clientes, proveedores y bancos. También sirve para actualizar los importes en la divisa adicional de los movimientos de contabilidad.  

## <a name="displaying-reports-and-amounts-in-the-additional-reporting-currency"></a>Mostrar los informes y los importes en la divisa adicional  
El uso de una divisa adicional puede servir de ayuda en el proceso de creación de informes de una empresa en los casos siguientes:  

- Empresas de países o regiones que no pertenecen a la Unión Europea y tienen un gran volumen de transacciones con empresas de países o regiones de la Unión Europea. En este caso, la empresa que no pertenece a la Unión Europea puede crear informes en euros para que sus informes financieros resulten más útiles a sus socios de la Unión Europea.  

- Empresas que desean mostrar sus informes en una divisa de mayor difusión internacional, además de en su divisa local.  

Hay varios informes de la aplicación de contabilidad que se basan en movimientos de contabilidad. Para visualizar los datos financieros en el informe en la divisa adicional para informes, solo tiene que seleccionar el campo **Muestra en div. adic.** en la ventana de contabilidad correspondiente.  

## <a name="to-set-up-a-currency-exchange-rate-service"></a>Para configurar un servicio de tipo de cambio de divisa
Puede utilizar un servicio externo para mantener actualizados los tipos de cambio de divisa. El servicio de tipos de cambio de divisa de Yahoo está preinstalado y listo para activarse.

1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Servicios de tipo de cambio de divisas** y, a continuación, elija el vínculo relacionado.
2. Seleccione la acción **Nuevo**.
3. En la ventana **Servicio de tipo de cambio de divisas**, rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Seleccione la casilla de verificación **Activado** para activar el servicio.

## <a name="to-update-currency-exchange-rates-through-a-service"></a>Para actualizar los tipos de cambio de divisa mediante un servicio
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Servicios de tipo de cambio de divisas"), escriba **Divisas** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione la acción **Actualizar tipos de cambio**.

El valor del campo **Tipo cambio** en la ventana **Divisas** se actualiza con el último tipo de cambio de divisa.

## <a name="see-also"></a>Consulte también
[Cerrar años y periodos](year-close-years-periods.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

