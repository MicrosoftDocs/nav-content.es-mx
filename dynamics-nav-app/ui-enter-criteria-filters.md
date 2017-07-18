---
title: Introducir criterios en los filtros
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 8eab393a0a77f9f1595ca1247c7549e68b491cb2
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="entering-criteria-in-filters"></a>Introducir criterios en los filtros
Cuando quiera buscar datos, como nombres de cliente, direcciones o grupos de productos, puede introducir los criterios. En los criterios de búsqueda puede usar todos los números y las letras que normalmente se emplean en un campo específico. También puede usar símbolos especiales o expresiones matemáticas para filtrar aún más los resultados.

## <a name="searching-using-the-quick-filter"></a>Búsqueda mediante el filtro rápido
Puede agregar filtros a todas las páginas con el filtro rápido. El filtro rápido se activa al elegir el icono de la lupa que se encuentra en la esquina superior derecha de una página. Este tipo de filtro se utiliza para una rápida introducción de criterios.

**Importante**: El filtro rápido proporciona un acceso sencillo a los datos de filtro mediante la especificación de texto simple, pero también proporciona muchas opciones de criterios de búsqueda. El filtro rápido actúa de distinta forma dependiendo de si introduce texto sin formato o texto con símbolos.  
- Si se introduce texto sin formato en los criterios de búsqueda, estos se interpretan como una búsqueda que tendrá en cuenta mayúsculas y minúsculas y que contendrá un determinado texto.  
- Si se introduce texto con símbolos en los criterios de búsqueda, estos se interpretan exactamente como se haya introducido este texto y teniendo en cuenta mayúsculas y minúsculas.

### <a name="quick-filter-criteria"></a>Criterios del filtro rápido
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH>Criterios de búsqueda</TH>
    <TH>Interpretado como…</TH>
    <TH>Devoluciones...</TH>
  </TR>
  <TR>
    <TD>>man</TD>
    <TD>@*man*</TD>
    <TD>Todos los registros que contienen el texto man y respetando mayúsculas y minúsculas.</TD>
  </TR>
  <TR>
    <TD>>se</TD>
    <TD>@*se*</TD>
    <TD>Todos los registros que contienen el texto se y respetando mayúsculas y minúsculas.</TD>
  </TR>
  <TR>
    <TD>>Man*</TD>
    <TD>Empieza por Man y distingue mayúsculas de minúsculas.</TD>
    <TD>Todos los registros que empiecen por el texto Man.</TD>
  </TR>
  <TR>
    <TD>'man'</TD>
    <TD>Un texto exacto respetando mayúsculas y minúsculas.</TD>
    <TD>Todos los registros que coincidan exactamente con man.</TD>
  </TR>
  <TR>
    <TD>@*man</TD>
    <TD>Termina en y distingue mayúsculas de minúsculas.</TD>
    <TD>Todos los registros que terminen en man.</TD>
  </TR>
  <TR>
    <TD>@man*</TD>
    <TD>Empieza por y distingue mayúsculas de minúsculas.</TD>
    <TD>Todos los registros que empiecen por man.</TD>
  </TR>
</TABLE>

**Nota**: No puede usar un carácter comodín al filtrar en los campos de enumeración, como el campo **Estado** en las órdenes de venta. Para especificar un filtro para este tipo de campo, puede especificar el valor numérico como parámetro de filtrado. Por ejemplo, en el campo **Estado** de una orden de venta que tenga los valores **Abierto**, **Lanzado**, **Aprobación pendiente** y **Anticipo pendiente**, utilice los valores **0**, **1**, **2** y **3** para filtrar para estas opciones.  

## <a name="see-also"></a>Consulte también
[Trabajar con Dynamics NAV](ui-work-product.md)

