---
title: "Gestionar diseños de informe"
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
ms.openlocfilehash: 57cd575c1f72841dae162b077d1f676720ee24e7
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
    
# <a name="manage-report-layouts"></a>Gestionar diseños de informe
Un diseño de informe controla el contenido y el formato del informe, incluidos los campos de datos de un conjunto de datos de informe que aparecen en el informe y la forma en que se organizan, el estilo del texto, las imágenes, etc. Desde los clientes de Dynamics NAV, puede cambiar el diseño que se usa en un informe, crear uno nuevo o modificar los existentes. 

En concreto, un diseño de informe configura lo siguiente:

- Los campos de etiqueta y de datos que incluir desde el conjunto de datos del informe de Dynamics NAV.
- El formato de texto, como el tipo de fuente, el tamaño y el color.
- El logotipo de la empresa y su posición.
- Configuración de página general, como márgenes e imágenes de fondo. 

Dynamics NAV se puede configurar con varios diseños de informe que puede cambiar según sea necesario. Puede utilizar uno de los diseños de informe integrados o puede crear diseños de informe personalizados y asignarlos a sus informes según sea necesario.

Se pueden usar dos tipos de diseños de informe: Word y RDLC.

## <a name="word-report-layout-overview"></a>Descripción del diseño de informes de Word
Un diseño de informe de Word está basado en un documento de Word (tipo de archivo .docx). Los diseños de informes de Word permiten diseñar diseños de informes con Microsoft Word 2013 o versiones posteriores. Un diseño de informes de Word determina el contenido del informe, controlando la forma en que se organizan estos elementos del contenido y su aspecto. Un documento de diseño de informe de Word normalmente usa tablas para organizar el contenido, donde las celdas pueden incluir campos de datos, texto o imágenes.

## <a name="rdlc-layout-overview"></a>Descripción del diseño de RDLC
Los diseños de RDLC se basan en los diseños de definición de informe de cliente (tipos de archivo .rdlc o .rdl). Estos diseños se crean y modifican con el generador de informes de SQL Server. El concepto del diseño de RDLC es similar al de Word, donde el diseño define el formato general del informe y determina qué campos del conjunto de datos incluir. La elaboración de diseños de RDLC es más avanzada que la de diseños de Word.

## <a name="built-in-and-custom-report-layouts"></a>Diseños de informe personalizados e integrados
Dynamics NAV incluye varios diseños integrados. Los diseños integrados son diseños predefinidos diseñados para informes específicos. Los informes de Dynamics NAV tendrán un diseño integrado, como un diseño de informes de RDLC, de Word o, en algunos casos, ambos. No puede modificar un diseño de informe integrado desde Dynamics NAV, pero sí se pueden usar como punto de inicio para crear sus propios diseños de informe personalizados. 

Los diseños personalizados son diseños de informe que se crean para modificar el aspecto de un informe. Normalmente se crea un diseño personalizado basado en un diseño integrado, si bien se pueden crear desde cero o desde una copia de un diseño personalizado existente. Los diseños personalizados permiten tener varios diseños para el mismo informe, con posibilidad de pasar de uno a otro según sea necesario. Por ejemplo, puede tener distintos diseños para cada empresa de Dynamics NAV, o puede tener diseños diferentes para la misma empresa para determinadas ocasiones o eventos, como una campaña especial o la temporada de vacaciones.

## <a name="deciding-whether-to-use-a-word-or-rdlc-report-layout"></a>Usar un diseño de informe de Word o uno de RDLC 
Un diseño de informe puede basarse en un documento de Word o en un archivo de RDLC. La decisión de si se usará un diseño de informe de Word o de RDLC dependerá del modo en que desea que aparezca el informe generado y de su conocimiento de Word y del generador de informes de SQL Server. 

Los conceptos de diseño generales son muy parecidos en Word y RDLC. Sin embargo, cada tipo tiene determinadas características de diseño que afectan a la forma en que el informe generado aparece en Dynamics NAV. Esto significa que el mismo informe puede tener un aspecto diferente cuando se utiliza el diseño de informe de Word en comparación con el diseño de informe de RDLC.

El proceso para configurar diseños de informe de Word y de RDLC en informes es el mismo. La diferencia principal es la forma en la que se modifican los diseños. Los diseños de informe Word suelen ser más fáciles de crear y modificar que los diseños de informe de RDLC, ya que se puede utilizar Word para ello. Los diseños de informe de RDLC se modifican mediante el generador de informes de SQL Server, que está dirigido a usuarios más avanzados.

Para obtener información acerca de cómo cambiar el diseño que desea usar, consulte [Procedimiento: Cambiar el diseño que se usa actualmente en un informe](ui-how-change-layout-currently-used-report.md)

## <a name="see-also"></a>Consulte también
[Trabajar con Dynamics NAV](ui-work-product.md)  
[Creación de un diseño de informe personalizado](ui-how-create-custom-report-layout.md)  
[Enviar documentos por correo electrónico](ui-how-send-documents-email.md)

