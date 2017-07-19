---
title: 'Procedimiento: Asociar y desasociar registros de documentos entrantes desde documentos y movimientos'
author: SorenGP
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: fece4e6e38075db6d394c71418fda82a7aa082e1
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-connect-and-disconnect-incoming-document-records-from-documents-and-entries"></a>Procedimiento: Asociar y desasociar registros de documentos entrantes desde documentos y movimientos
Puede almacenar los documentos empresariales externos en Dynamics NAV adjuntando los archivos de documento a los registros de documento entrante relacionados. Si el documento, como una factura de compra, no se ha iniciado como un registro de documento entrante, puede crear un registro de documento entrante y conectarlo a él más adelante. También puede adjuntar archivos de documento entrante a los documentos de compra y de venta registrados, y a los movimientos de proveedor, de cliente y de contabilidad mediante el cuadro informativo **Archivos de documento entrante**, por ejemplo, en las ventanas **Facturas de compra registradas** y **Movimientos de proveedor**.

En las ventanas **Catálogo de cuentas** y **Movs. contabilidad**, puede usar una función de búsqueda para buscar los movimientos de contabilidad para aquellos documentos de compra y de venta registrados que no tienen registros de documento entrantes y después vincularlos de forma centralizada a registros existentes o crear registros nuevos con archivos de documentos adjuntos. Para obtener más información, consulte [Procedimiento: Buscar documentos registrados sin registros de documentos entrantes](across-how-find-posted-documents-without-income-document-records.md).

Los procedimientos siguientes muestran cómo adjuntar un archivo a una factura de compra existente que no se ha creado a partir de un registro de documento entrante y cómo adjuntar un archivo a un movimiento de proveedor. Adjuntar un archivo a los documentos de compra o venta registrados funciona de forma similar.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Para crear y conectar un registro de documento entrante a partir de una factura de compra
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Facturas de compra** y, a continuación, elija el enlace relacionado.
2. Seleccione la línea de una factura de compra a la que desee adjuntar un archivo y, a continuación, elija la acción **Crear documento entrante desde archivo**.
3. También puede seleccionar la línea de una factura de compra a la que desee adjuntar un archivo y, a continuación, elija la acción **Adjuntar archivo**.
4. En la ventana **Insertar archivo**, seleccione el archivo que representa el documento entrante en cuestión y, a continuación, elija el botón **Abrir**.

## <a name="to-create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Para crear y conectar un registro de documento entrante a partir de movimiento de proveedor
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Movimientos de proveedor** y, a continuación, seleccione el enlace relacionado.
2. Seleccione una línea de un movimiento de proveedor al que desee adjuntar un archivo y, a continuación, elija la acción **Crear documento entrante desde archivo**.
3. También puede seleccionar una línea de un movimiento de proveedor al que desee adjuntar un archivo y, a continuación, elija la acción **Adjuntar archivo**.
4. En la ventana **Insertar archivo**, seleccione el archivo que representa el documento entrante en cuestión y, a continuación, elija el botón **Abrir**.

## <a name="to-remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Para eliminar la conexión de un registro de documento entrante a un documento registrado
En cualquier momento puede eliminar los archivos adjuntos de los documentos no registrados eliminando el registro de documento entrante relacionado. Si se registra el documento, primero deberá eliminar la conexión desde el registro de documento entrante.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Documentos entrantes** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la línea de un registro de documento entrante asociado a un documento registrado que quiera eliminar y, a continuación, elija la acción **Eliminar referencia al registro**.

Se elimina la conexión al documento registrado. Ahora puede asociar otro registro de documento entrante al documento registrado como se describe en este tema.

## <a name="see-also"></a>Consulte también  
[Procesar documentos entrantes](across-process-income-documents.md)  
[Documentos entrantes](across-income-documents.md)  
[Gestionar compras](purchasing-manage-purchasing.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

