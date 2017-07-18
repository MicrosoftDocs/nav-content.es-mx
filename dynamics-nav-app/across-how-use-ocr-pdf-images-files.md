---
title: "Procedimiento: Utilizar el servicio OCR para convertir archivos PDF y de imagen en documentos electrónicos"
author: SorenGP
ms.custom: na
ms.date: 10/06/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 96b1baf3554d3647e75223bb4cb1ee08dc21eb6d
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-use-ocr-to-turn-pdf-and-image-files-into-electronic-documents"></a>Procedimiento: Utilizar el servicio OCR para convertir archivos PDF y de imagen en documentos electrónicos
A partir de archivos PDF o de imagen que reciba de sus socios comerciales, podrá hacer que un servicio externo de OCR (reconocimiento óptico de caracteres) genere documentos electrónicos que se podrán convertir en registros de documentos en Dynamics NAV. Por ejemplo, cuando recibes una factura de un proveedor en formato PDF, la puedes enviar al servicio de OCR desde la ventana **Documentos entrantes**. Esto se describe en el primer procedimiento.

Como alternativa al envío del archivo desde la ventana **Documentos entrantes** puede enviar el archivo al servicio OCR por correo electrónico. A continuación, cuando vuelve a recibir el documento electrónico, se crea automáticamente un registro de documento entrante relacionado. Esto se describe en el segundo procedimiento.

Después de algunos segundos, recibirá de vuelta el archivo desde el servicio OCR como una factura electrónica que se podrá convertir a una factura de compra para el proveedor. Esto se describe en el tercer procedimiento.

Como el OCR se basa en el reconocimiento óptico, es probable que el servicio de OCR interprete de forma incorrecta algunos caracteres del PDF o de los archivos de imagen la primera vez que procese documentos de un determinado proveedor, por ejemplo. Puede que no interprete el logotipo de la compañía como el nombre del proveedor o que pueda malinterpretar el importe total de una recepción debido a su diseño. Para evitar estos errores en el futuro, puede corregirlos en una versión separada de la ventana **Documentos entrantes**. A continuación, debe enviar las correcciones al servicio OCR para entrenarle para que interprete los caracteres específicos correctamente la próxima vez que procese un documento PDF o de imagen para el mismo proveedor. Para obtener más información, consulte la sección "Para preparar el servicio OCR para evitar errores".

El tráfico de los archivos hacia y desde el servicio OCR se procesa a través de un movimiento de la cola de proyectos dedicado, que se crea automáticamente cuando se activa la conexión del servicio relacionado. Para obtener más información, vea [Procedimiento: Configurar documentos entrantes](across-how-setup-income-documents.md).

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-from-the-incoming-documents-window"></a>Para enviar un archivo PDF o de imagen al servicio OCR desde la ventana **Documentos entrantes**
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Documentos entrantes** y, a continuación, seleccione el enlace relacionado.
2. Cree un nuevo registro de documento entrante y adjunte el archivo. Para obtener más información, vea [Procedimiento: Crear registros de documentos entrantes](across-how-create-income-document-records.md).  
3. En la ventana **Documentos entrantes**, seleccione una o más líneas y, a continuación, seleccione la acción **Enviar a cola de trabajos**.

    El valor del campo **Estado OCR** cambia a **Listo** . El archivo PDF o de imagen adjunto lo envía al servicio OCR la cola de proyectos según la programación, siempre que no haya errores.
5. De forma alternativa, en la ventana **Documentos entrantes**, seleccione una o más líneas y, a continuación, seleccione la acción **Enviar a servicio OCR**.

El valor del campo **Estado OCR** cambia a Enviado siempre que no haya errores.

## <a name="to-send-a-pdf-or-image-file-to-the-ocr-service-by-email"></a>Para enviar un archivo PDF o de imagen al servicio OCR por correo electrónico
Desde su aplicación de correo electrónico, puede enviar un correo electrónico al proveedor del servicio OCR con el archivo PDF o de imagen adjunto. Para obtener información acerca de la dirección de correo electrónico a la que enviar el archivo, consulte el sitio web del proveedor del servicio OCR.

Puesto que no existe ningún registro de documento entrante para el archivo, se creará automáticamente un nuevo registro en la ventana **Documentos entrantes** cuando reciba el documento electrónico resultante desde el servicio OCR. Para obtener más información, vea [Procedimiento: Crear registros de documentos entrantes](across-how-create-income-document-records.md).

**Nota**: Si trabaja con una tableta o un teléfono, puede enviar el archivo al servicio OCR en cuanto haya tomado una foto del documento o puede crear un documento entrante directamente. Para obtener más información, vea la sección "Para crear documentos entrantes a partir de una fotografía" en [Procedimiento: Crear registro de documentos entrantes](across-how-create-income-document-records.md).

## <a name="to-receive-the-resulting-electronic-document-from-the-ocr-service"></a>Para recibir el documento electrónico resultante desde el servicio de OCR.
El documento electrónico que se crea por el servicio de OCR desde un archivo PDF o de imagen, se recibe automáticamente en la ventana **Documentos entrantes** por el movimiento de cola de proyectos que se configura cuando activa el servicio de OCR.

Si no utiliza una cola de proyectos o desea recibir el documento final de OCR más pronto de lo acordado, puede elegir el botón **Recibir desde el servicio de OCR**. Esto obtendrá los documentos que el servicio de OCR haya completado.

**Nota**: Si el servicio de OCR está configurado para requerir la verificación manual de los documentos procesados, el campo **Estado OCR** contendrá **Esperando verificación**. En ese caso, ejecute los pasos siguientes para iniciar sesión en el sitio web del servicio de OCR para comprobar manualmente un documento de OCR.

1. En el campo **Estado OCR**, seleccione el hipervínculo **Esperando verificación**. De forma alternativa, seleccione **Esperando verificación** en la página Inicio.
2. En el sitio web del servicio de OCR, inicie sesión con las credenciales de su cuenta de OCR. Estas son las credenciales que también usó al configurar el servicio. Para obtener más información, vea la sección "Configurar un servicio de OCR" en [Procedimiento: Configurar documentos entrantes](across-how-setup-income-documents.md).

    Si accede al sitio web desde el campo **Estado OCR**, el documento en cuestión se muestra inmediatamente después de que firme. Si accede al sitio web y selecciona el mosaico en la página Inicio, en la primera página que se abre, debe elegir el botón **Empezar** en la pestaña **Verificar** o hacer doble clic en el documento que desea entrar.

    La información del documento de OCR muestra tanto el contenido original del archivo PDF o de imagen como los valores del archivo de OCR resultantes.
3. Revise los distintos valores de campo y edite o introduzca valores manualmente en los campos donde el servicio de OCR se ha marcado como no seguro.
4. Elija el botón **Aceptar**. El proceso de OCR se ha completado y el documento electrónico resultante se ha enviado a la ventana de **Documentos entrantes** en Dynamics NAV, de acuerdo con la programación de las colas de proyecto.

    Si accede al sitio web y escoge el mosaico en la página Inicio, cualquier otro documento de OCR que deba verificarse se mostrará automáticamente en el sitio web.
5. Repita el paso 4 para que se verifique cualquier otro documento de OCR.

Ahora puede empezar a crear los documentos de registro para los documentos electrónicos recibidos en Dynamics NAV, de forma manual o automática. Para obtener más información, consulte la sección "Para crear un registro de documentos en Dynamics NAV desde un documento recibido de OCR". También puede conectar el registro de documento entrante al documento registrado o no registrado existente de forma que el archivo de origen sea fácil de acceder desde Dynamics NAV. Para obtener más información, vea [Procesar documentos entrantes](across-process-income-documents.md).

## <a name="to-create-a-purchase-invoice-from-an-electronic-document-received-from-the-ocr-service"></a>Para crear una factura de compra desde un documento electrónico recibido del servicio de OCR
El procedimiento siguiente describe cómo crear un registro de la factura de compra desde una factura recibida de un proveedor como un documento electrónico del servicio OCR. El procedimiento es el mismo que cuando crea, por ejemplo, una línea del diario general a partir de un recibo de gastos.

**Nota**: Los campos **Descripción** y **N.°** de las líneas creadas del documento se completarán solo si primero ha asignado el texto encontrado en el documento de OCR a los campos de Dynamics NAV. Puede realizar esta acción como referencias cruzadas de producto, para las líneas de documentos del tipo Producto, o como asignaciones de texto a cuenta, para las líneas de documentos o diarios del tipo Cuenta de contabilidad. Para obtener más información, consulte la herramienta para la acción **Referencias cruzadas** en las fichas de productos y el procedimiento relacionado, [Procedimiento: Asignar texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md)

Para los documentos entrantes, normalmente usa la acción **Asignar texto a cuenta** para indicar que un determinado texto en una factura de proveedor recibida desde el servicio de OCR se ha asignado a una cuenta de un proveedor determinado. Si va más adelante, cualquier parte de la descripción de un documento entrante que existe como texto de asignación implica que el campo **N.º** resultante de las líneas de documento o diario del tipo Cuenta de contabilidad se han rellenado con el proveedor en cuestión.

Además de asignarlo a una cuenta de proveedor o a cuentas de contabilidad, también puede asignarlo a una cuenta bancaria. Esto resulta práctico, por ejemplo, en los documentos electrónicos para los gastos que ya se han pagado, donde desea crear una línea de diario general que esté lista para registrarse en una cuenta bancaria.

1. Seleccione la línea del documento entrante para el documento electrónico del proveedor que ha recibido del servicio OCR.
2. Para asignar un texto a un documento en la cuenta del proveedor, una cuenta de débito, seleccione la acción **Asignar texto a cuenta** y, a continuación, rellene la ventana **Asignación de texto a cuenta** con la información que se aplicará al proveedor más adelante. Para más información, consulte [Procedimiento: Asignación de texto en pagos periódicos a cuentas para conciliación automática](receivables-how-map-text-recurring-payments-accounts-auto-reconcilliation.md).
3. Para asignar los números de producto del documento a las descripciones de los productos del proveedor, abra la ficha de cada producto y, a continuación, elija la acción **Referencias cruzadas** para configurar las referencias cruzadas entre su descripción de los artículos y la del vendedor.
4. En la ventana **Documentos entrantes**, seleccione la acción **Crear documento**.

Se creará una factura de compra en Dynamics NAV según la información del documento electrónico del proveedor que recibió del servicio OCR.

Los errores de validación, normalmente relacionados con datos maestros incorrectos o no presentes en Dynamics NAV, se mostrarán en la ficha desplegable **Errores y advertencias**. Para obtener más información, consulte la sección "Para gestionar errores al recibir documentos electrónicos".

## <a name="to-handle-errors-when-receiving-electronic-documents"></a>Para gestionar errores al recibir documentos electrónicos
1. En la ventana **Documentos entrantes**, seleccione la línea de un documento entrante recibido del servicio OCR que contenga errores. Está indicado en el Valor de error del campo **Estado OCR**.
2. Seleccione la acción **Editar** para abrir la ventana de **Documento entrante**.
3. En la ficha desplegable **Errores y advertencias**, seleccione el mensaje y, a continuación, elija la acción **Abrir registro relacionado**.
4. Se abrirá la ventana que contiene los datos incorrectos o que faltan, como una ficha de proveedor en la que falte un valor de campo.
5. Corrija el error o los errores tal como se describe en cada mensaje de error.
6. Continúe para procesar el documento electrónico entrante volviendo a seleccionar la acción **Crear manualmente**.
7. Repita los pasos del 5 al 6 para los errores pendientes hasta que el documento electrónico se pueda recibir correctamente.

## <a name="to-train-the-ocr-service-to-avoid-errors"></a>Para preparar al servicio OCR para evitar errores
Como el OCR se basa en el reconocimiento óptico, es probable que el servicio de OCR interprete de forma incorrecta algunos caracteres del PDF o de los archivos de imagen la primera vez que procese documentos de un determinado proveedor, por ejemplo. Puede que no interprete el logotipo de la compañía como el nombre del proveedor o que pueda malinterpretar el importe total de un recibo de gastos debido a su diseño. Para evitar que sigan ocurriendo este tipo de errores, puedes corregir los datos recibidos por el servicio de OCR y después enviar comentarios al servicio.

La ventana **Corrección de datos de OCR** que abrió desde la ventana **Documentos entrantes**, muestra los campos de la ficha desplegable **Información financiera** en dos columnas, una con los datos editables del OCR y la otra con los datos de solo lectura. Cuando selecciona el botón **Enviar comentarios sobre OCR** se envía el contenido de la ventana **Corrección de datos de OCR** al servicio de OCR. La próxima vez que el servicio procese PDF o archivos de imagen que contengan los datos en cuestión, se incorporarán tus correcciones para evitar los mismos errores.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Documentos entrantes** y, a continuación, seleccione el enlace relacionado.
2. Abra un registro de documentos entrantes que contenga los datos recibidos del servicio OCR que desea corregir.
3. En la ventana **Documentos entrantes**, seleccione la acción **Corregir datos de OCR**.
4. En la ventana **Corrección de datos de OCR**, sobrescriba los datos en la columna editable para cada campo que tenga un valor incorrecto.
5. Para deshacer las correcciones que se hayan realizado desde que se abrió la ventana **Corrección de datos de OCR**, seleccione la acción **Restablecer datos de OCR**.
6. Para enviar las correcciones al servicio OCR, seleccione la acción **Enviar comentarios sobre OCR**.
7. Para guardar las correcciones, cierre la ventana **Corrección de datos de OCR**.

Los campos de la ficha desplegable **Información financiera** en la ventana **Documento entrante** se actualizan con los valores nuevos que introdujo en el paso 4.

## <a name="see-also"></a>Consulte también  
[Procesar documentos entrantes](across-process-income-documents.md)  
[Documentos entrantes](across-income-documents.md)  
[Gestionar compras](purchasing-manage-purchasing.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)
