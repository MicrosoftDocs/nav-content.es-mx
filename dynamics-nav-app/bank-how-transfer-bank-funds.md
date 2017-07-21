---
title: 'Procedimiento: Transferir fondos bancarios'
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f34bef80c64cbad0a0b20d4d021cefbdc5a1cb64
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-transfer-bank-funds"></a>Procedimiento: Transferir fondos bancarios
En ocasiones es necesario transferir un importe desde una cuenta bancaria a otra. Para hacerlo, debe registrar una transacción en el diario general. La tarea varía en función de si los bancos usan la misma divisa o distintas divisas.

## <a name="to-post-a-transfer-between-bank-accounts-with-the-same-currency-code"></a>Para registrar transferencias entre bancos con el mismo código de divisa
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general** y, a continuación, seleccione el enlace relacionado.
2. En una línea de diario, rellene **Fecha registro** y **N. º documento**. .
3. En el campo **Tipo mov**, seleccione **Banco**.
4. En el campo **N.º cuenta** seleccione la cuenta desde la que quiere transferir los fondos.
5. En el campo **Importe**, introduzca el importe que quiere transferir.
6. En el campo **Tipo contrapartida**, seleccione **Cuenta bancaria**.
7. En el campo **N.º cuenta contrapartida**, seleccione la cuenta a la que quiere transferir los fondos.
8. Registre el diario.

## <a name="to-post-a-transfer-between-bank-accounts-with-different-currency-codes"></a>Para registrar transferencias entre bancos con códigos de divisa distintos
Para transferir fondos entre cuentas bancarias que usan distintas divisas, debe registrar dos líneas de diario general.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general** y, a continuación, seleccione el enlace relacionado.
2. Cree dos líneas de diario y rellene los campos **Fecha de registro** y **N.º de documento**. .
3. En la primera línea de diario, en el campo **Tipo**, seleccione **Cuenta bancaria**.
4. En el campo **N.º cuenta** seleccione la cuenta desde la que quiere transferir los fondos.
5. En el campo **Importe**, introduzca el importe en la divisa de la cuenta bancaria. Escriba los importes de crédito con un signo menos. Escriba los importes de débito sin el signo menos.
6. En el campo **Tipo contrapartida**, seleccione **Cuenta bancaria**.
7. En el campo **N.º cuenta contrapartida**, seleccione la cuenta a la que quiere transferir los fondos.
8. En la segunda línea de diario, en el campo **Tipo**, seleccione **Cuenta bancaria**.
9. En el campo **N.º cuenta** seleccione la cuenta a la que quiere transferir los fondos.
10. En el campo **Importe**, introduzca el importe en la divisa de la cuenta bancaria. Escriba los importes de crédito con un signo menos. Escriba los importes de débito sin el signo menos.
11. En el campo **Tipo contrapartida**, seleccione **Cuenta bancaria**.  
12. En el campo **N.º cuenta contrapartida**, seleccione la cuenta desde la que quiere transferir los fondos.

    **Nota**: Si los tipos de cambio usados en el diario son diferentes a los contenidos en la ventana **Tipos de cambio de divisa**, introduzca una tercera línea para las diferencias positivas o negativas del cambio. Especifique **Cuenta** en el campo **Tipo mov**. Especifique el número de cuenta para la pérdida o ganancia de tipo de campo en el campo **N.º cuenta**. . Introduzca la diferencia positiva o negativa del tipo de cambio en el campo **Importe** con o sin el signo menos para los créditos y los débitos respectivamente.
13. Registre el diario.

## <a name="see-also"></a>Consulte también  
[Administrar cuentas bancarias](bank-manage-bank-accounts.md)  
[Configurar la banca](bank-setup-banking.md)  
[Trabajar con diarios generales](ui-work-general-journals.md)

