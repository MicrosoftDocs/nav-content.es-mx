---
title: "Factura electrónica"
description: "Las empresas mexicanas deben tener la posibilidad de enviar facturas de forma electrónica como archivos de Comprobante Fiscal Digital por Internet (CFDI). [!INCLUDE[navnow](../../includes/navnow_md.md)] admite CFDI para que pueda exportar facturas de ventas y servicios, así como notas de crédito con formato de documentos electrónicos que cuenten con la firma digital requerida."
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
ms.openlocfilehash: e5b0811565f6475784b4a5d2d2b1ef67b3483b9d
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="electronic-invoicing"></a>Factura electrónica
Las empresas mexicanas deben tener la posibilidad de enviar facturas de forma electrónica como archivos de Comprobante Fiscal Digital por Internet (CFDI). [!INCLUDE[navnow](../../includes/navnow_md.md)] admite CFDI para que pueda exportar facturas de ventas y servicios, así como notas de crédito con formato de documentos electrónicos que cuenten con la firma digital requerida.  
  
 El archivo de CFDI es un archivo XML que incluye lo siguiente:  
  
-   Nombre de la empresa emisora.  
  
-   Domicilio fiscal de la empresa emisora.  
  
-   Régimen tributario de la empresa emisora.  
  
-   Número de registro federal de contribuyente (RFC) de la empresa emisora.  
  
-   RFC de la empresa receptora.  
  
-   Cantidad y descripción de los bienes o servicios.  
  
-   Precio unitario.  
  
-   Importes de impuestos enumerados por tipo de impuesto.  
  
-   Código de divisa.  
  
-   Ubicación de aduana, que ../../incluye la fecha y el número del documento de la aduana, si la transacción es una importación.  
  
-   Sello digital de la empresa emisora, asignado por las autoridades fiscales (SAT).  
  
-   Sello digital de un proveedor de servicios autorizado (PAC), que usted elija.  
  
> [!IMPORTANT]  
>  Deberá enviar las facturas electrónicas a un PAC, que es un proveedor de servicios autorizado designado por las autoridades fiscales de México (SAT).  
  
## <a name="getting-started"></a>Introducción  
 Antes de poder utilizar ADD INCLUDE<!--[!INCLUDE[navnow](how-to-set-up-electronic-invoicing.md). Para obtener información sobre los certificados y las claves de SAT, consulte el sitio web del [Servicio de Administración Tributaria](http://go.microsoft.com/fwlink/?LinkId=242772).  
  
 Además, debe especificar los servicios web que utilizará para comunicarse con el PAC con el fin de obtener los sellos digitales correspondientes. Para obtener más información, consulte [Procedimiento: Configurar servicios web de PAC](how-to-set-up-pac-web-services.md).  
  
> [!IMPORTANT]  
>  Tenga en cuenta que SAT ha certificado a varios PAC en México, por lo que deberá obtener la información pertinente para comunicarse con el PAC que elija.  
  
## <a name="sending-electronic-invoices"></a>Envío de facturas electrónicas  
 Una vez que haya registrado una factura o una nota de crédito, podrá enviarla al cliente. Pero antes debe obtener el sello digital de un PAC. [!INCLUDE[navnow](../../includes/navnow_md.md)] se comunica con el PAC a través de servicios web para solicitar un sello y, de este modo, su empresa y el PAC firman digitalmente el documento de forma automática.  
  
 Al enviar una factura o una nota de crédito al cliente, [!INCLUDE[navnow](../../includes/navnow_md.md)] utiliza la dirección de correo electrónico que se ha especificado en la ventana **Información de empresa**. El documento se envía a la dirección de correo electrónico que se ha especificado en la ventana **Ficha cliente** del cliente de facturación que consta en la factura o la nota de crédito. En la ventana **Configuración de contabilidad**, también puede elegir si desea incluir documentos como archivos PDF en el mensaje de correo electrónico que se envía.  
  
> [!IMPORTANT]  
>  Los usuarios encargados de enviar las facturas electrónicas deben ser capaces de enviar correo a través del Protocolo simple de transferencia de correo (SMTP). En función de la configuración de la empresa, puede que deba conceder permisos explícitos a cada usuario y equipo correspondiente.  
  
 Asimismo, si desea imprimir los documentos, estos incluirán un código de barras de respuesta rápida (QR) y otra información identificatoria de la factura electrónica relacionada. Dicha información permite que un equipo informático pueda leer el documento impreso y proporciona un vínculo entre el documento electrónico y el documento impreso.  
  
 Para obtener más información, consulte [Procedimiento: Generar facturas electrónicas](how-to-generate-electronic-invoices.md).  
  
## <a name="communication-component"></a>Componentes de comunicación  
 El ADD INCLUDE<!--[!INCLUDE[navnow](../../includes/nav_windows_md.md)]-->. El componente gestiona la comunicación con los servicios web del PAC y también genera los códigos QR que se incluyen en los documentos impresos. Para consultar ejemplos sobre cómo utilizar el ensamblado Microsoft.Dynamics.NAV.MX.dll, consulte la codeunit 10145 **Admin. de facturas elect.** y la codeunit 10147 **Generador de objetos de factura electrónica**.  
  
 Al generar un documento electrónico para solicitar un sello, [!INCLUDE[navnow](../../includes/navnow_md.md)] crea un documento XML y lo envía al PAC para su procesamiento. El documento XML original incluye la misma información que el campo de cadena original que se muestra en el documento impreso. La cadena original ../../incluye la información siguiente:  
  
-   Fecha de documento  
  
-   Tipo de documento  
  
-   Condiciones de pago  
  
-   Nombre, dirección y número de registro federal de su empresa  
  
-   Nombre, dirección y número de registro federal del cliente  
  
-   Importes y cantidades de línea  
  
 El PAC devuelve un documento XML que incluye la cadena original y, también, ../../una sección para el sello digital. En [!INCLUDE[navnow](../../includes/navnow_md.md)], puede exportar los archivos XML de los documentos que tienen una firma digital y obtener así más detalles sobre los datos que se incluyen en cada elemento XML.  
  
## <a name="see-also"></a>Consulte también  
 [Procedimiento: Configurar la facturación electrónica](how-to-set-up-electronic-invoicing.md)   
 [Procedimiento: Configurar servicios web de PAC](how-to-set-up-pac-web-services.md)   
 [Procedimiento: Generar facturas electrónicas](how-to-generate-electronic-invoices.md)
