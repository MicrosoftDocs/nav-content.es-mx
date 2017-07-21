---
title: "Procedimiento: Configuración del servicio de fuentes de banco de Envestnet Yodlee"
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
ms.openlocfilehash: 270568214afd2ca8af15f0fa7640337c77ec2f1e
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-envestnet-yodlee-bank-feeds-service"></a>Procedimiento: Configuración del servicio de fuentes de banco de Envestnet Yodlee
Puede importar extractos electrónicos de su banco para rellenar rápidamente la ventana **Diario de conciliación de pagos** para que pueda liquidar pagos y conciliar la cuenta bancaria. Para obtener más información, vea [Liquidar pagos automáticamente y conciliar cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Nota**: es posible que el servicio Fuentes de banco de Envestnet Yodlee, o el servicio fuentes de banco de otro proveedor, no esté disponible en su sistema. Póngase en contacto con su socio de Microsoft si desea usar un servicio de fuentes de banco para importar extractos bancarios.

Cuando ha activado el servicio de fuente de banco, debe vincular la cuenta bancaria implicada a la cuenta bancaria de la que proviene la fuente. Vincula las cuentas a cuentas en línea en los siguientes ejemplos:

- No existe una cuenta en Dynamics NAV para su cuenta bancaria en línea. Por tanto, cree la cuenta vinculando de la cuenta bancaria en línea.
- Existe una cuenta en Dynamics NAV que desea vincular a una cuenta bancaria en línea.
- Una cuenta vinculada debe ser desvinculada porque desea dejar de usar el servicio de fuente de banco de la cuenta.
- Las cuentas en línea se han modificado y desea actualizar la información en las cuentas en Dynamics NAV.

Cuando se ha habilitado el servicio de fuente de banco, puede definir una cuenta bancaria que importe automáticamente nuevos extractos de cuenta en la ventana **Diario de conciliación de pagos** cada dos horas. Las transacciones para los pagos que ya se hayan registrado como liquidados o conciliados en la ventana **Diario de conciliación de pagos** no se importarán. Para obtener más información, vea la sección "Para habilitar la importación automática de los estados de cuenta bancarios".

**Nota**: Si usa la configuración asistida Configurar empresa, algunos de los pasos en los procedimientos siguientes se realizarán automáticamente cuando acceda a la configuración de la cuenta bancaria de la empresa. Para obtener más información, consulte [Este es Dynamics NAV](across-get-started.md).

## <a name="to-enable-the-bank-feed-service"></a>Para activar el servicio de fuente de banco
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Abra la cuenta bancaria que usará para el servicio de fuente de banco.
3. En la ventana **Banco**, en el campo **Formato de importación de estados de cuenta bancarios**, seleccione YODLEEBANKFEED.  

El servicio de fuente de banco se activará cuando vincule una cuenta a la cuenta bancaria en línea relacionada. Vea el procedimiento siguiente.  

## <a name="to-create-a-new-linked-bank-account"></a>Para crear una nueva cuenta bancaria vinculada
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la cuenta bancaria correspondiente y, a continuación, seleccione **Crear una nueva cuenta bancaria vinculada**. La ventana **Vinculación de cuenta bancaria** se abre después de unos segundos.

    **Nota**: Esta ventana muestra la página web del servicio de fuentes de banco de Envestnet Yodlee. La terminología y las funciones de la ventana pueden no coincidir con las instrucciones que ofrece este tema.  
3. En la ventana **Vinculación de banco en línea**, en el panel **Vínculo de cuenta** use la función Buscar para buscar el banco en el que tiene una o varias cuentas bancarias en línea.
4. Seleccione el nombre del banco. Se abre el panel **Iniciar sesión**.
5. Introduzca el nombre de usuario y la contraseña que usa para conectarse al banco en línea y, a continuación, seleccione el botón **Siguiente**.  
6. El servicio de fuente de banco se prepara para vincular la primera cuenta bancaria en línea en el banco especificado a una nueva cuenta en Dynamics NAV.

    **Nota**: Si ha configurado más de una cuenta en línea en el banco deberá crear las cuentas adicionales en Dynamics NAV para aquellas cuentas bancarias en línea adicionales. Consulte los pasos 8 a 10.

    Cuando el proceso ha finalizado correctamente, el nombre del banco aparecerá en el panel **Mis cuentas** en la pestaña **Vinculado**. El valor entre corchetes indica la cantidad de cuentas bancarias en línea que están vinculadas.
7. Elija el botón **Aceptar**.

    Si solo está vinculada una cuenta bancaria en línea, la ventana **Ficha banco** se abre para crear una nueva, previamente rellenada con el nombre de la cuenta bancaria en línea. En este caso, la vinculación de la cuenta bancaria se ha completado. solo resta configurar la cuenta bancaria. Para obtener más información, vea [Procedimiento: Configurar cuentas bancarias](bank-how-setup-bank-accounts.md).

    Si se vinculan más de una cuenta bancaria en línea, la ventana **Vinculación de banco** abre una ventana que enumera la lista de cuentas bancarias en línea adicionales que no se han vinculado en Dynamics NAV. En ese caso, siga el paso siguiente.  
8. En la ventana **Vinculación de banco**, seleccione la línea para una cuenta bancaria en línea y, a continuación, seleccione la acción **Vincular a nuevo banco**.

    La ventana **Ficha banco** se abre para crear una nueva, rellenada previamente con el nombre de la cuenta bancaria en línea.

    Si ya existe una cuenta bancaria en Dynamics NAV al que desea vincular la cuenta bancaria en línea adicional, siga el siguiente paso.  
9. En la ventana **Vinculación de banco**, seleccione la línea para una cuenta bancaria en línea y, a continuación, seleccione la acción **Vincular a banco existente**.
10. En la ventana **Lista de bancos**, seleccione la cuenta bancaria que desee vincular y, a continuación, haga clic en **Aceptar**.

## <a name="to-link-a-bank-account-to-an-online-bank-account"></a>Para vincular una cuenta bancaria a una cuenta bancaria en línea.
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la línea para una cuenta bancaria que no está vinculada a una cuenta en línea y, a continuación, seleccione la acción **Vincular a banco en línea**. La ventana **Vinculación de banco en línea** se abre rellenada previamente con el nombre del banco en el panel **Vincular cuenta**.
3. Seleccione el nombre del banco. Se abre el panel **Iniciar sesión**.
4. Introduzca el nombre de usuario y la contraseña que usa para conectarse al banco en línea y, a continuación, seleccione el botón **Siguiente**.

    El servicio de fuente de banco se prepara para vincular su cuenta bancaria en Dynamics NAV a la cuenta bancaria en línea relacionada.

    Cuando el proceso ha finalizado correctamente, el nombre del banco aparecerá en el panel **Mis cuentas** en la pestaña **Vinculado**. Si el banco tiene más de una cuenta bancaria, solo se vincula la cuenta bancaria seleccionada en el paso 2.
5. Elija el botón **Aceptar**.

En la ventana **Lista de bancos**, se activa la casilla **Vinculado**.

## <a name="to-unlink-a-bank-account"></a>Para desvincular una cuenta bancaria
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.  
2. Seleccione la línea para una cuenta bancaria vinculada que desee desvincular de su cuenta en línea relacionada y, a continuación, seleccione la acción **Desvincular un banco en línea**.

**Nota**: Si selecciona **Sí** en el cuadro de diálogo de confirmación, el vínculo a la cuenta bancaria en línea se elimina y se eliminan los detalles de inicio de sesión. Para vincular nuevamente la cuenta bancaria a una cuenta bancaria en línea, debe volver a iniciar sesión en el banco. Para obtener más información, vea la sección "Para vincular una cuenta bancaria a una cuenta bancaria en línea".

## <a name="to-update-bank-account-linking"></a>Para actualizar la vinculación de la cuenta bancaria
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la cuenta bancaria correspondiente y, a continuación, seleccione la acción **Actualizar vinculación de banco**.

Si surgen problemas para alguna de las cuentas bancarias vinculadas en la ventana **Lista de bancos**, se abre la ventana **Vinculación de banco** y se especifican qué cuentas bancarias tienen problemas. Los problemas se solucionan mejor desvinculando la cuenta y reconstruyendo el vínculo. Para obtener más información, vea la sección "Para vincular una cuenta bancaria a una cuenta bancaria en línea".

## <a name="to-enable-automatic-import-of-bank-statements"></a>Para activar la importación automática de los extractos de cuenta
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Seleccione la línea para una cuenta bancaria vinculada y, a continuación, seleccione la acción **Configuración de la importación automática de estados de cuenta bancarios**.
3. En la ventana **Configuración de la importación automática de estado de cuentas bancarias**, en el campo **N.º de días incluidos**, especifique hasta qué fecha en el pasado desea obtener nuevas transacciones bancarias.

    **Nota**: Se recomienda establecer este valor a 7 días o más.
4. Seleccione la casilla de verificación **Habilitado**.  
Cada hora, la ventana **Diario de conciliación de pagos** se rellenará de cualquier nuevo pago que se realice en la cuenta bancaria en línea.

**Nota**: Las transacciones para los pagos que ya se hayan registrado como liquidados o conciliados en la ventana de **Diario de conciliación de pagos** no se importarán.

## <a name="see-also"></a>Consulte también  
[Configurar la banca](bank-setup-banking.md)  
[Administrar cuentas bancarias](bank-manage-bank-accounts.md)  
[Liquidar pagos automáticamente y conciliar cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md)  
[Personalizar Dynamics NAV usando extensiones](ui-extensions.md)

