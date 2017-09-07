---
title: Cerrar libros
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
ms.openlocfilehash: ad75bfd18936df07e0fe9dcc5ed6bb94360ea965
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="close-books"></a>Cerrar libros
Una vez que se haya asegurado de que todas sus cuentas estén actualizadas, y que asigne costos e ingresos, puede cerrar los libros para un ejercicio o periodo.

El cierre del año no es obligatorio, pero haciéndolo le resultará más fácil trabajar en el sistema, porque podrá utilizar las opciones de filtrado disponibles. Tampoco tendrá que temer la pérdida de datos de las transacciones al realizar el cierre, porque todos los datos se conservan, incluso después de cerrar el año.

## <a name="closing-book-process"></a>Cerrar procesos de libros
El proceso de cerrar el libro incluye estas tareas principales:

1. Cerrar el periodo contable.

    Un ejercicio se define como uno o varios periodos abiertos como se define en la página **Periodos contables**. Un ejercicio normal contiene 12 periodos de un mes cada uno, pero también puede elegir otro método para definir un ejercicio.

    Para obtener más información, vea [Procedimiento: Cerrar periodos contables](year-close-account-periods.md).

2. Registrar asientos post-cierre.

    Cuando cierre un ejercicio, debe introducir diversas transacciones administrativas (como productos prepagados y acumulados). Estas transacciones se denominan movimientos de ajuste. No existen reglas especiales para registrar estos movimientos y contienen (al igual que otros movimientos) una marca de verificación en el campo **Asiento post-cierre** si se registran en una fecha de un ejercicio cerrado. Incluso aunque un ejercicio se haya cerrado, todavía podrá registrar en él movimientos de contabilidad.

3. Transferir saldos de las cuentas de resultado al balance de situación.

    Una vez cerrado un ejercicio y registrados todos asientos post-cierre, las cuentas de resultados deben cerrarse y los ingresos netos para el año deben transferirse a una cuenta bajo los fondos propios de los propietarios en el balance. Utilice el proceso Cerrar cuenta de resultado con este fin. El proceso procesa todas las cuentas de contabilidad del tipo Resultado y crea movimientos que revierten sus saldos. Estos movimientos se colocan en un diario, desde donde se pueden registrar. El proceso no los registra automáticamente, salvo si se utiliza una divisa de informes adicional. En este caso, el proceso registra directamente en la contabilidad.

    Para obtener más información, consulte [Asiento regularización](year-close-income-statement.md).
4. Registro del movimiento de cierre de fin de año junto con los movimientos de cuenta de desplazamiento de capital.

    Cuando finalice el proceso Cerrar cuenta de resultado, puede registrar los movimientos que ha generado el proceso. Si no ha especificado una cuenta de ajustes red. div. adic. en el proceso, escriba una línea con un movimiento de saldo que registre los ingresos netos en la cuenta contable correcta bajo los fondos propios de los propietarios en el balance. Finalmente, registre el diario.

    Para obtener más información, consulte [Procedimiento: Registrar movimiento de cierre del ejercicio](year-how-post-year-end-close-entry.md).

## <a name="what-happens-when-you-close"></a>Consecuencias del cierre
Al realizar el cierre al final del año, el programa traslada los ingresos calculados a la cuenta de remanentes. Además, el programa marca el ejercicio como "cerrado," y todos los movimientos siguientes del año cerrado como "movimientos del año anterior."

El sistema genera un movimiento de cierre, pero no lo registra automáticamente. Tiene la opción de realizar los movimientos de la cuenta de desplazamiento de capital, para poder decidir cómo asignar el movimiento de cierre. Por ejemplo, si la empresa consta de varias divisiones, puede dejar que el sistema genere un sólo movimiento de cierre para todas ellas y, a continuación, puede realizar un movimiento de desplazamiento para la cuenta de capital de cada división.

Puede realizar registros en un ejercicio anterior, después de se hayan cerrado las cuentas de resultados, si vuelve a ejecutar el proceso Asiento regularización.

## <a name="see-also"></a>Consulte también
[Procedimiento para abrir un nuevo ejercicio](finance-setup-how-open-new-fiscal-year.md)
