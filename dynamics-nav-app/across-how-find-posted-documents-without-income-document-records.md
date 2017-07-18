---
title: 'Procedimiento: Buscar documentos registrados sin registros de documentos entrantes'
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
ms.openlocfilehash: eb65922decc86ca6834cae4cf46c6f2ff492e29c
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-find-posted-documents-without-incoming-document-records"></a>Procedimiento: Buscar documentos registrados sin registros de documentos entrantes
En las ventanas **Catálogo de cuentas** y **Movs. contabilidad**, puede usar una función de búsqueda para buscar los movimientos de contabilidad para aquellos documentos de compra y de venta registrados que no tienen registros de documento entrantes y después vincularlos de forma centralizada a registros existentes o crear registros nuevos con archivos de documentos adjuntos.

## <a name="to-find-posted-documents-without-incoming-document-records"></a>para buscar documentos registrados sin registros de documentos entrantes
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Catálogo de cuentas** y, a continuación, seleccione el enlace relacionado.
2. Seleccione una línea para una cuenta de contabilidad para la que quiere ver los documentos de ventas y compras registrados de los movimientos de contabilidad sin registros de documentos entrantes y, a continuación, seleccione la acción **Documentos registrados sin documento entrante**.
3. De forma alternativa, elija la acción **Movimientos de activos**.
4. En la ventana **Movs. contabilidad**, elija la acción **Documentos registrados sin documento entrante**.

La ventana **Documentos registrados sin documento entrante** se abre con los documentos registrados de compra y de venta sin registros de documento entrantes representados por los movimientos de contabilidad de la cuenta para la que abrió la ventana. La ventana puede mostrar un máximo de 1000 líneas. De manera predeterminada, el campo **Filtro de fecha** contiene un filtro que limita las líneas a los movimientos con fechas de registro desde el inicio del periodo contable a la fecha de trabajo.

## <a name="to-connect-found-documents-to-existing-incoming-document-records"></a>Para vincular los documentos encontrados con registros de documento entrantes existentes
1. En la ventana **Documentos registrados sin documento entrante**, seleccione la línea para un documento registrado que desee conectar con un registro de documento entrante existente y, a continuación, elija la acción **Seleccionar documento entrante**.
2. En la ventana **Documentos entrantes**, seleccione el registro de documento entrante que desea agregar para conectarlo con el documento registrado encontrado y, a continuación, elija el botón **Aceptar**.
3. En la ventana **Documentos registrados sin documento entrante**, el registro de documento entrante seleccionado ahora está vinculado con el documento registrado, como se puede ver en el cuadro informativo **Archivos de documento entrante**.

Si no existe un registro de documento entrante correspondiente en la ventana **Documentos entrantes**, puede crearlo. Para obtener más información, vea [Procedimiento: Crear registros de documentos entrantes](across-how-create-income-document-records.md).

## <a name="see-also"></a>Consulte también  
[Procesar documentos entrantes](across-process-income-documents.md)  
[Documentos entrantes](across-income-documents.md)  
[Gestionar compras](purchasing-manage-purchasing.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

