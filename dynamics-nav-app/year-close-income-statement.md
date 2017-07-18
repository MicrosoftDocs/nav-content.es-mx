---
title: Cerrar cuenta de resultado
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
ms.openlocfilehash: 83dfa0db1345aa18d6900470c93ccdc00bd1b403
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="close-income-statement"></a>Cerrar cuenta de resultado
Cuando finaliza un ejercicio, debe cerrar los periodos que lo forman. Para ello, puede ejecutar el proceso **Asiento regularización**. Esta tarea transfiere el resultado anual a una cuenta en la hoja de balance y cierra las cuentas del balance de ingresos. Se realiza creando líneas en un diario, que después puede registrar.

## <a name="to-run-the-close-income-statement-batch-job"></a>Para ejecutar el proceso Cerrar cuenta de resultado
1. Cierre el ejercicio fiscal. Antes de ejecutar el proceso se debe cerrar el ejercicio fiscal. Para obtener más información, vea [Procedimiento: Cerrar periodos contables](year-close-account-periods.md).
2. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Asiento regularización** y, a continuación, seleccione el enlace relacionado.
3. Elija el botón **Aceptar** para iniciar el trabajo por lotes.

## <a name="about-the-close-income-statement-batch-job"></a>Acerca del proceso Cerrar cuenta de resultado
El trabajo por lotes procesa todas las cuentas generales del tipo resultado y crea movimientos que cancelan los saldos respectivos. Es decir, cada movimiento es la suma de todos los movimientos de contabilidad de la cuenta del ejercicio. Estos nuevos movimientos se disponen en un diario, en el que debe especificar una cuenta de contrapartida y una cuenta de retención de beneficios en el balance antes del registro. Cuando se registra el diario, también se registra un movimiento en cada cuenta del resultado, de manera que su saldo sea cero y, a la vez, el resultado del año se transfiera al balance.

Debe registrar el diario manualmente. El trabajo por lotes no registra los movimientos automáticamente, salvo cuando se utiliza una divisa adicional. En ese caso, el proceso registra los movimientos directamente en contabilidad.

La fecha de las líneas que inserta el trabajo por lotes en el diario siempre es una fecha de cierre de ejercicio. La U-fecha es una fecha ficticia comprendida entre el último día de un ejercicio y el día primero del siguiente. La ventaja de registrar en una U-fecha es que se mantienen los saldos correctos para las fechas ordinarias del ejercicio.

El proceso **Asiento regularización** se puede usar varias veces. Puede registrar en un ejercicio anterior, incluso después de que haya cerrado las cuentas de resultado (siempre que vuelva a ejecutar nuevamente este proceso).

## <a name="see-also"></a>Consulte también
[Cerrar libros](year-close-books.md)  
[Procedimiento: registrar movimiento de cierre del ejercicio](year-how-post-year-end-close-entry.md)  
[Procedimiento para abrir un nuevo ejercicio](finance-setup-how-open-new-fiscal-year.md)
