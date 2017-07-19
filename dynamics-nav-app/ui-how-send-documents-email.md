---
title: "Procedimiento: Enviar documentos por correo electrónico."
author: SorenGP
ms.custom: na
ms.date: 11/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: e4476c2ab903001017dcd6c8bdaa84892ba79c9e
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-send-documents-by-email"></a>Procedimiento: Enviar documentos por correo electrónico.
Para comunicar el contenido de documentos empresariales rápidamente a sus socios, por ejemplo, la información de pagos en los documentos de venta a los clientes, puede usar la función de Informe personalizado para definir el contenido específico de un documento que se insertará en el cuerpo del correo electrónico automáticamente.

Para activar los correos electrónicos en Dynamics NAV, inicie la guía de configuración **Configurar correo electrónico** en la página Inicio.

Puede enviar por correo electrónico prácticamente todos los tipos de documento como archivos adjuntos en el mensaje directamente desde la ventana que muestra el documento. Además del archivo adjunto, puede configurar contenido específico de un documento en el cuerpo del correo electrónico con la información principal de ése documento, precedida por el texto estándar que saluda al destinatario del correo e introduce el documento en cuestión. Para ofrecer a sus clientes el pago de las ventas de forma electrónica usando un servicio de pago, como por ejemplo PayPal, puede disponer también de su información y su hipervínculo en el cuerpo del correo.

A partir de todos los documentos soportados, se inicia el envío del correo seleccionando la acción **Enviar** en los documentos registrados, o la acción **Registrar y enviar** en los documentos no registrados.

Si el campo **Correo electrónico** en la ventana **Enviar documento a** se establece en **Sí (Mensaje para configuración)**, se abre la ventana **Enviar correo electrónico** rellenada previamente con el contacto en el campo **Para:** y el documento adjunto es un archivo PDF. En el campo **Cuerpo**, puede introducir tanto el texto manualmente como disponer del campo rellenado con un contenido específico de un documento en el cuerpo del correo electrónico que ha configurado.

El procedimiento siguiente describe cómo configurar el informe **Ventas - Factura** para usarlo como contenido específico en el cuerpo del correo cuando envíe las facturas de venta registradas.

## <a name="to-set-up-a-document-specific-email-body-for-sales-invoices"></a>Para configurar un documento específico en el cuerpo de un correo electrónico para las facturas de venta
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Selección informes ventas** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Informe selección - ventas**, en el campo **Uso**, seleccione **Facturar**.
3. En una línea nueva, en el campo **Id. informe**, seleccione, por ejemplo, informe estándar 1306.
4. Seleccione la casilla **Usar para el cuerpo del correo electrónico**.
5. Seleccione el campo **Id. de diseño del cuerpo del correo electrónico** y, a continuación, seleccione uno de los diseños disponibles de la ventana **Diseños de informe personalizados**.
6. Las plantillas de informes definen tanto el estilo como el contenido del cuerpo del correo, incluyendo el texto estándar que precede la información principal del documento.
7. Para ver o editar el diseño en el que se basa el cuerpo del correo electrónico, en la ventana **Diseños de informe personalizados**, elija la acción **Editar diseño**.
8. Si desea ofrecer a sus clientes el pago de las ventas de forma electrónica puede configurar el servicio de pago relacionado, como por ejemplo PayPal y, a continuación, puede disponer también de su información y su hipervínculo en el cuerpo del correo. Para obtener más información, consulte [Procedimiento: Permitir pagos de cliente a través de PayPal](sales-how-enable-customer-payments-paypal.md).
9. Elija el botón **Aceptar**.

Ahora bien, cuando selecciona, por ejemplo, la acción Enviar en la ventana **Factura venta reg.**, el cuerpo del correo electrónico contendrá la información del documento del informe 1306 precedida por el texto estándar siguiendo el diseño de informe que seleccionó en el paso 5.

El procedimiento siguiente describe cómo enviar una factura de ventas registrada como un mensaje de correo electrónico con un documento adjunto en formato PDF y con un contenido específico en el cuerpo del correo.
## <a name="to-send-documents-by-email"></a>Para enviar documentos por correo electrónico
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Facturas de ventas registradas** y, a continuación, elija el enlace relacionado.
2. Seleccione la factura de ventas relevante y elija la acción **Enviar**. Se abre la ventana **Enviar documento a**.
3. en el campo **Correo electrónico** seleccione **Sí (Mensaje para configuración)**. Para obtener más información, vea [Procedimiento: Configurar los perfiles de envío de documentos](sales-how-setup-document-send-profiles.md).
4. Elija el botón **Aceptar**. Se abre la ventana **Enviar correo electrónico**.
5. En el campo **Para:** introduzca una dirección de correo electrónico válida. El valor predeterminado es la dirección de correo electrónico del cliente.
6. En el campo **Cc:**, especifique una dirección de correo electrónico para que se envíe una copia del correo electrónico a otro destinatario.
7. En el campo **CCo:**, especifique una dirección de correo electrónico para que se envíe una copia del correo electrónico a otro destinatario sin que su dirección y nombre aparezcan a los demás destinatarios.
8. En el campo **Asunto**, escriba un texto descriptivo del asunto. El valor predeterminado es el nombre del cliente y el número de factura.
9. En el campo **Archivo adjunto**, se adjunta la factura generada de forma predeterminada como un archivo PDF. Seleccione el botón de búsqueda para abrir el archivo o para adjuntar otro.
10. En el campo **Cuerpo**, escriba un mensaje breve al destinatario.

    Si se configura el contenido específico de un documento en el cuerpo del correo electrónico en la ventana **Informe selección - ventas**, el campo **Cuerpo** se rellena automáticamente. Para obtener más información, vea "Para configurar un contenido específico de un documento en el cuerpo del correo electrónico para las facturas de venta" en este tema.
11. Seleccione la casilla **Editar en la aplicación de Outlook** para abrir el mensaje en la aplicación de correo electrónico para Office 365.
12. Haga clic en el botón **Aceptar** para enviar el correo electrónico.

**Nota**: Si no necesita especificar la configuración del correo electrónico cada vez que envíe un documento, puede seleccionar la opción **Sí (Usar configuración predeterminada)** en el campo Correo electrónico en la ventana **Enviar documento a**. En ese caso, la ventana **Enviar correo electrónico** no se abrirá. Consulte el paso 4. Para obtener más información, vea [Procedimiento: Configurar los perfiles de envío de documentos](sales-how-setup-document-send-profiles.md).

## <a name="see-also"></a>Consulte también  
[Trabajar con Dynamics NAV](ui-work-product.md)  
[Facturación de ventas](sales-how-invoice-sales.md)

