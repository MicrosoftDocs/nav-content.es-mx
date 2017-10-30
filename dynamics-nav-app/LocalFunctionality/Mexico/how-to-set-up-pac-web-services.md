---
title: Procedimiento para configurar servicios web de PAC
description: "Para enviar facturas y notas de crédito de forma electrónica, primero debe especificar uno o varios proveedores del sello electrónico que debe incluirse en las facturas de México."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 2d29b1dabbdd42106f52cb198b2b11c031e0536b
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-pac-web-services"></a>Procedimiento: Configurar servicios web de PAC
Para enviar facturas y notas de crédito de forma electrónica, primero debe especificar uno o varios proveedores del sello electrónico que debe incluirse en las facturas de México.  
  
 Al enviar un documento electrónico, este debe contar con un sello digital provisto por un proveedor de servicios autorizado (PAC), antes de que dicho documento pueda enviarse al cliente. La comunicación entre [!INCLUDE[navnow](../../includes/navnow_md.md)] y el PAC se administra a través de servicios web y, por lo tanto, es necesario especificar información técnica sobre los servicios web del PAC que desea usar.  
  
 Para usar servicios web, debe identificar el nombre del método del servicio web que procesa solicitudes de sellos digitales. El PAC puede suministrarle dicha información.  
  
 Si el PAC ofrece el servicio de cancelación de documentos firmados, debe especificar dos métodos web: uno para solicitar el sello digital y otro para cancelar un documento ya firmado.  
  
### <a name="to-set-up-a-pac-web-service"></a>Para configurar el servicio web del PAC  
  
1.  Elija el icono ![Buscar página o informe](media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Servicios web de PAC** y, a continuación, elija el vínculo relacionado.  
  
2.  Rellene los campos tal como se describe en la tabla siguiente.  
  
    |Campo|Descripción|  
    |---
    title: Procedimiento para configurar servicios web de PAC description: Para enviar facturas y notas de crédito de forma electrónica, primero debe especificar uno o varios proveedores del sello electrónico que debe incluirse en las facturas de México.
    
    documentationcenter: '' author: SorenGP

    ms.prod: "dynamics-nav-2017" ms.topic: article ms.devlang: na ms.tgt_pltfrm: na ms.workload: na ms.search.keywords: ms.date: 07/01/2017 ms.author: sgroespe

---------------------------------|---------------------------------------|  
    |**Entorno**|Especifique si el servicio web es para un entorno de prueba o de producción.|  
    |**Tipo**|Especifique si el método web es para solicitar un sello digital o para cancelar un documento firmado.|  
    |**Nombre de método**|Indique el nombre del método web, como **GeneraTimbre** o **CancelaTimbre**.|  
    |**Dirección**|Indique la dirección URL del método web.|  
  
     Contact your PAC for this information.  
  
5.  Repita los pasos para los PAC adicionales que desee definir.  
  
    > [!IMPORTANT]  
    >  El SAT ha certificado a varios PAC en México, por lo que deberá obtener la información pertinente para comunicarse con el PAC que elija.  
  
## <a name="see-also"></a>Consulte también  
 [Facturación electrónica](electronic-invoicing.md)   
 [Procedimiento: Configurar la facturación electrónica](how-to-set-up-electronic-invoicing.md)
