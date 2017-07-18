---
title: Trabajar con diarios generales
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 2dc2b22fbc0ff70addd16ca14e8c5416c49915e7
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="work-with-general-journals"></a>Trabajar con diarios generales
Puede usar diarios generales para registrar transacciones financieras en cuentas generales y otras cuentas, como cuentas bancarias, de cliente y de proveedor. Registrar con un diario general siempre crea movimientos en cuentas contables. Esto es así incluso si, por ejemplo, una línea del diario se registra en una cuenta de cliente, pues un movimiento se registra en una cuenta de cobros de contabilidad a través de un grupo de registro.

La información que introduzca en un diario es temporal y se puede modificar mientras se encuentre en el diario. Al registrar el diario, la información se transfiere a movimientos en cuentas individuales, donde no se puede modificar. Sin embargo, puede desliquidar los movimientos registrados y puede registrar movimientos de inversión o correctores.

## <a name="journal-templates-and-batches"></a>Secciones y plantillas del diario
Existen varias plantillas de diario general. Cada libro de diario se representa mediante una ventana específica con funciones particulares y los campos que se requieren para admitir estas funciones, como la ventana **Diario de conciliación de pagos** para procesar pagos bancarios y la ventana **Diario de pagos** para pagar a sus proveedores.

Para cada libro diario, puede configurar su propio diario personal como una sección de diario. Por ejemplo, puede definir su propia sección de diario del diario de pagos que tiene su diseño y configuración personal.

**Nota**: Un ejemplo de una configuración personal que puede definir en su sección de diario general es tener la ayuda del sistema para rellenar los campos de importes. Si marca la casilla **Proponer importe de compensación** en la línea de su sección en la ventana **Secciones diario general**, a continuación, el campo **Importe**, por ejemplo, las líneas de diario general del mismo número de documento se rellena automáticamente con el valor necesario para incluir el saldo del documento. Para obtener más información, consulte [Permitir que Dynamics NAV proponga valores](ui-let-system-suggest-values.md).

## <a name="main-accounts-and-balancing-accounts"></a>Cuentas principales y cuentas de contrapartida
Si ha configurado cuentas de contrapartida predeterminadas para las secciones del diario, la cuenta de contrapartida se rellenará automáticamente cuando rellene el campo **N.º cuenta**. . Si no, rellene los campos **N.º de cuenta** y **N.º cuenta contrapartida** manualmente. Un importe positivo en el campo **Importe** se adeuda en la cuenta principal y se carga en la cuenta de contrapartida. Un importe negativo se acredita en la cuenta principal y se debita de la cuenta de contrapartida.

**Nota**: El IVA se calcula de manera independiente para la cuenta principal y la cuenta de contrapartida, para que puedan usar diferentes tipos porcentuales de IVA.

## <a name="recurring-journals"></a>Diarios periódicos
Un diario periódico es un diario general con campos especiales para administrar las transacciones que registre frecuentemente con pocos cambios o con ninguno. Al usar estos campos para las transacciones periódicas, puede registrar importes tanto fijos como variables. También puede especificar la movimientos de reversión automática al día siguiente a la fecha de registro y usar claves de asignación con los movimientos periódicos.

## <a name="see-also"></a>Consulte también
[Utilizar claves de asignación en diarios generales](ui-how-use-allocation-keys-general-journals.md)  
[Finanzas](finance-setup.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

