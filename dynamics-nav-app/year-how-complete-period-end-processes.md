---
title: Cerrar periodos
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: ac1ed2d1dcf8bf780bda91fbf0a04e5c5e8d106a
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="close-periods"></a>Cerrar periodos
La aplicación no le exige que cierre los periodos, sin embargo, puede realizar muchas actividades de fin de periodo (fin de mes) si lo desea. Este tema proporciona una descripción general de estos procesos y actividades, que pueden ser o no ser necesarios para su empresa.

## <a name="general-ledger"></a>Contabilidad
* Especifique fechas de registro para todos el sistema y específicos para el usuario.

    Esto especifica las fechas entre las cuales se permiten los registros. En función de sus necesidades comerciales, puede restringir los intervalos de fechas de registro de los usuarios al inicio del proceso de fin de periodo o posteriormente durante el fin del periodo. Para obtener más información, vea [Procedimiento: Especificar periodos de registro](finance-setup-how-specify-posting-periods.md).
* Lleve a cabo todos los ajustes de contabilidad necesarios
* Actualice y registre los Diarios periódicos.
<!--* Process Consolidations-->
* Ejecute los esquemas de cuentas como se indica a continuación:
  1. Abra la ventana **Estructura de cuentas** y seleccione la acción **Imprimir**.
  2. Rellene la ventana de solicitud **Esquema cuentas** y seleccione la acción **Imprimir**.

## <a name="sales--receivables"></a>Ventas y cobros
* Registre todas las órdenes, facturas, notas de crédito y devoluciones de ventas.
* Registre todo los diarios de recepciones de efectivo.
* Actualice y registre los diarios periódicos relativos a ventas y cobros.
* Concilie los cobros en el libro de contabilidad
* Ejecute el proceso **Eliminar peds. venta factdos**.

## <a name="purchases--payables"></a>Compras y pagos
* Registre todas las órdenes, facturas, notas de crédito y devoluciones de compra.
* Registre todos los registros de pagos.
* Actualice y registre los diarios periódicos que son relativos a compras y pagos.
* Ejecute el informe **Antigüedad pagos** y concilie las cuentas por pagar en el libro de contabilidad.
* Ejecute el proceso **Eliminar peds. compra factdos**.

<!-- ### Fixed Assets
* Post all maintenance costs have been posted through the fixed asset journals or invoices.
* Post adjustments.
* Post appreciation.
* Post depreciation.
* Update and post the recurring fixed asset journal.-->

<!--### Intercompany
* Process Intercompany Postings.-->

## <a name="calculate-and-process-sales-tax"></a>Calcular y procesar los impuestos de venta
*  Realice los extractos de impuesto.

## <a name="see-also"></a>Consulte también
[Cerrar años y periodos](year-close-years-periods.md)  
[Cerrar libros](year-close-books.md)

