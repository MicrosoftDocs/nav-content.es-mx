---
title: Gestionar documentos entrantes
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 49acc3549180b73dada6415f3ea40f17c1dd9e4c
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="manage-incoming-documents"></a>Gestionar documentos entrantes
Algunas transacciones empresariales no se registran en Dynamics NAV desde el principio. En su lugar, un documento empresarial externo llega a la empresa como datos adjuntos de correo electrónico o una copia en papel que se digitaliza para archivarla. Esto es habitual en las compras, donde dichos archivos de documentos entrantes representan los recibos de pago de gastos o pequeñas compras.

Desde los archivos PDF o de imagen que representan a los documentos entrantes podrá hacer que un servicio externo del OCR (reconocimiento óptico de caracteres) genere documentos electrónicos que se podrán convertir a registros de documento en Dynamics NAV.

En la ventana **Documentos entrantes**, puede usar distintas funciones para revisar recibos de gastos, gestionar tareas de OCR y convertir archivos de documentos entrantes, manual o automáticamente en los documentos pertinentes o en líneas de diario. Los archivos externos se pueden adjuntar en cualquier etapa del proceso, incluidos los documentos registrados y los movimientos de proveedor, cliente y de contabilidad resultantes.

El proceso de documento entrante puede constar de las principales actividades siguientes:

* Registrar los documentos externos en Dynamics NAV creando líneas en la ventana **Documentos entrantes** de cualquiera de las siguientes formas:
    * Manualmente, usando funciones simples, desde un PC o un dispositivo móvil, de una de las siguientes formas:
        * Use el botón **Crear desde archivo** y, a continuación, rellene los campos en la ventana **Documento entrante**. El campo se adjunta automáticamente.  
        * Use el botón **Nuevo** y, a continuación, rellene los campos en la ventana **Documento entrante** y adjunte el archivo relacionado manualmente.
        * Desde una tableta o un teléfono, utilice el botón **Crear desde la cámara** para crear un registro de documento entrante nuevo y, a continuación, envíe la imagen al servicio OCR, por ejemplo.
    * De forma automática, recibiendo el documento del servicio OCR como documento electrónico una vez haya enviado por correo electrónico el PDF o el archivo de imagen relacionado al servicio OCR. La ficha desplegable **Información financiera** se rellena automáticamente en la ventana **Documento entrante**.
* Use el servicio de OCR para convertir documentos PDF o archivos de imagen a documentos electrónicos que se puedan convertir a registros de documento en Dynamics NAV.
* Crear documentos nuevos o líneas de diario general desde registros de documento entrante manualmente especificando la información a medida que la lee de los archivos de documento entrante.
* Adjuntar archivos de documento entrantes a documentos de compra y de venta en cualquier estado, incluidos los movimientos de proveedor, cliente y contabilidad de la operación de registro.
* Permite ver registros de documento entrantes y sus archivos adjuntos desde cualquier documento o movimiento de compra y venta, o buscar todos los movimientos de contabilidad sin registros de documento entrantes desde la ventana **Catálogo de cuentas**.


|Para |Vea |
|---|----|
|Configurar la función Documentos entrantes y el servicio OCR.|[Configurar documentos entrantes](across-how-setup-income-documents.md)|
|Crear registros de documentos entrantes, adjuntar archivos, usar OCR para convertir archivos PDF en documentos electrónicos, convertir documentos electrónicos en registros de documentos y auditar registros de documentos entrantes de documentos de compra y venta registrados.|[Procesar documentos entrantes](across-process-income-documents.md)|

## <a name="see-also"></a>Consulte también  
[Gestionar compras](purchasing-manage-purchasing.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

