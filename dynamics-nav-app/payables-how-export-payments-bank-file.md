---
title: "Exportación de pagos a un archivo de banco"
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
ms.openlocfilehash: 09bdf56b3d5e76b12d868091e89232ce9c08e215
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-export-payments-to-a-bank-file"></a>Exportación de pagos a un archivo de banco
Cuando esté listo para hacer los pagos a los proveedores mediante la ventana **Diario de pagos**, puede exportar un archivo con la información de pago en las líneas del diario. Después, puede cargar el archivo al banco electrónico para procesar las transferencias de dinero relacionadas.

En la versión genérica de Dynamics NAV, ya está configurado y conectado un proveedor global de servicios de conversión de datos bancarios a cualquier formato de archivo que el banco requiera.

**Nota**: Antes de poder exportar desde un diario de pagos, debe activar la función de exportar en la sección del diario relacionada. Además, su cuenta bancaria y la del proveedor deben haberse configurado para el pago electrónico. Para obtener más información, vea [Procedimiento: Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md).

Use la ventana **Registros de transferencia de crédito** para ver los archivos de pago que han sido exportados del diario de pagos. Desde esta ventana, también puede reexportar los archivos de paso en caso de errores técnicos o cambios en el archivo.

## <a name="to-export-payments-to-a-bank-file"></a>Para exportar pagos a un archivo bancario
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios de pago** y, a continuación, seleccione el enlace relacionado.
2. Rellene las líneas de diario de pago, por ejemplo, mediante la función **Proponer pagos a proveedores**. Para obtener más información, vea [Procedimiento: Proponer pagos a proveedores](payables-how-suggest-vendor-payments.md).  
3. Cuando haya completado todas las líneas del diario de pagos, seleccione **Exportar pago al archivo**.

    Los mensajes de error aparecerán en el cuadro informativo **Errores del archivo de pagos**, donde también puede elegir un mensaje de error para ver información detallada. Debe resolver todos los errores para que se pueda exportar el archivo de pagos.

    **Sugerencia**: Cuando usa la función del servicio de conversión de datos bancarios, un mensaje de error común indica que el número de la cuenta bancaria no tiene la longitud que el banco requiere. Para evitar o resolver error, debe eliminar el valor **IBAN** en la ventana **Tarjeta de cuenta bancaria** y, a continuación, en el campo **N.º cuenta bancaria** introduzca un número de cuenta en el formato que el banco requiere.
4. En la ventana **Guardar como**, especifique la ubicación a la que se exporta el archivo y, a continuación, seleccione **Guardar**.

El archivo del pago de banco se exporta a la ubicación que se especifique y puede empezar a cargarlo en la cuenta bancaria electrónica y hacer los pagos en sí.

Cuando se recibe confirmación de que los pagos se han procesado correctamente en el banco, puede registrar las líneas del diario de pagos exportadas.

## <a name="to-plan-when-to-post-exported-payments"></a>Para planificar cuando registrar los pagos exportados
Si no desea registrar una línea de diario de pagos para un pago exportado, por ejemplo porque se está esperando confirmación de que la transacción ha sido procesada por el banco, puede eliminar solo la línea del diario. Cuando se crea posteriormente una línea de diario de pagos para pagar el importe pendiente en la factura, el campo **Importe total exportado** muestra qué parte del importe del pago se ha exportado ya. También puede encontrar información detallada acerca del total exportado seleccionando el botón **Movimientos de reg. de transferencia de crédito** para ver detalles acerca de los archivos de pago exportados.

Si hace un seguimiento de un proceso en el que no registra pagos hasta que haya confirmado que se han procesado en el banco, puede controlarlo de dos formas.

* En un diario de pagos con líneas de pago propuestas, puede ordenar tanto por la columna **Exportado a archivo de pagos** como por la columna **Importe total exportado** y después eliminar las propuestas de pago de las facturas pendientes para las que ya se han realizado los pagos y no desea realizar ninguno más.
* En la ventana **Proponer pagos a proveedores**, donde puede especificar qué pagos desea insertar en el diario de pagos, puede seleccionar la casilla **Omitir pagos exportados** si no desea insertar líneas de diario para pagos que ya se hayan exportado.

Para ver información acerca de pagos exportados, seleccione la acción **Historial de exportación de pagos**.

## <a name="to-re-export-payments-to-a-bank-file"></a>Para reexportar pagos a un archivo bancario
Puede volver a exportar los archivos de pago desde la ventana **Registros de transferencia de crédito**. Antes de eliminar o registrar líneas de diario de pagos, también puede volver a exportar el archivo de pago desde la ventana **Diario de pagos** simplemente exportándolo de nuevo.

Si ha eliminado o registrado las líneas de diario de pagos tras exportarlas, solo puede volver a exportar el mismo archivo de pago desde la ventana **Registros de transferencia de crédito**. Seleccione la línea para el lote de transferencias de crédito que desee volver a exportar y, a continuación, use la acción **Reexportar pagos al archivo**.

## <a name="see-also"></a>Consulte también
[Pagos](payables-manage-payables.md)  
[Gestionar compras](purchasing-manage-purchasing.md)  
[Configurar compra](purchasing-setup-purchasing.md)

