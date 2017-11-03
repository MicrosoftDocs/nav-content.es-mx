---
title: "Procedimiento para generar facturas electrónicas"
description: "Después de registrar una factura de venta en [!INCLUDE[navnow](../../includes/navnow_md.md)], debe generar una factura electrónica que se enviará al cliente. Asimismo, puede exportar dicha factura electrónica como un archivo XML, que puede guardar en una ubicación especificada."
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
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 990b7116cbced09f2c1d6d777dcda82df1c7f5bf
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-generate-electronic-invoices"></a>Procedimiento: Generar facturas electrónicas
Después de registrar una factura de venta en [!INCLUDE[navnow](../../includes/navnow_md.md)], debe generar una factura electrónica que se enviará al cliente. Asimismo, puede exportar dicha factura electrónica como un archivo XML, que puede guardar en una ubicación especificada.  

En el procedimiento siguiente se describe cómo generar facturas electrónicas para facturas de venta, aunque los mismos pasos también se aplican a facturas y notas de crédito de servicios.  

## <a name="to-generate-electronic-invoices-for-sales-invoices"></a>Para generar facturas electrónicas de facturas de ventas  

1.  Elija el icono ![Buscar página o informe](../../media/ui-search/search_small.png "icono de Buscar página o informe"), escriba **Factura venta reg.** y, a continuación, elija el vínculo relacionado.  
2.  Seleccione la factura registrada.  
3.  Elija la acción **Send Electronic Document**. De este modo, se enviará un correo electrónico al cliente con la factura electrónica adjuntada como archivo XML. Si seleccionó el campo **Enviar informe PDF** de la ventana **Configuración de contabilidad**, también se incluirá un documento PDF con el archivo XML.  
4.  Como alternativa, elija la acción **Exportar documento electrónico como XML**. Seleccione la ubicación donde desea guardar la factura electrónica como archivo XML.  

    Para comprobar la actividad de facturas electrónicas, en la ventana **Factura venta reg.**, en la ficha desplegable **Facturación**, se actualizarán los campos **Documento electrónico enviado** y **No. of E-Document Submissions**.  

> [!NOTE]  
>  ADD INCLUDE<!--[!INCLUDE[bp_refimplementation](../../includes/bp_refimplementation_md.md)]-->  

## <a name="see-also"></a>Consulte también  
 [Procedimiento: Configurar la facturación electrónica](how-to-set-up-electronic-invoicing.md)   
  [Facturación electrónica](electronic-invoicing.md)  
  [Funcionalidad local de México](mexico-local-functionality.md)

