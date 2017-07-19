---
title: "Procedimiento: Configuración del servicio de conversión de datos bancarios"
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
ms.openlocfilehash: 801e2abee52ec9804028a797e4f330b5e080549a
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-the-bank-data-conversion-service"></a>Procedimiento: Configuración del servicio de conversión de datos bancarios
Puede exportar líneas de pago desde la ventana **Diario de pagos** a una secuencia de datos que, más tarde, puede subir a su cuenta bancaria para procesarlas automáticamente, de manera que no deberá realizar pagos electrónicos de forma por separado. Para obtener más información, vea [Procedimiento: Exportar pagos a un archivo bancario](payables-how-export-payments-bank-file.md).

Ya está configurado y listo para habilitar un proveedor global de servicios de conversión de información de pagos a cualquier formato de datos que requiera el banco en Dynamics NAV.

Como alternativa al servicio de fuentes del banco Envestnet, también puede usar el servicio de conversión de datos bancarios para que un archivo de estado de cuenta bancario que reciba del banco se convierta a un flujo de datos que pueda importar a Dynamics NAV. Para obtener más información, vea [Procedimiento: Liquidar pagos automáticamente y conciliar cuentas bancarias](receivables-apply-payments-auto-reconcile-bank-accounts.md).

**Nota**: El servicio de conversión de datos bancarios puede imponer un límite de número de líneas que se pueden exportar en un archivo. Recibirá un mensaje de error si se supera el límite. Es aconsejable que los archivos de estado de cuenta no excedan las 1000 líneas, ya que el tiempo de procesado en el servicio de conversión de datos bancarios puede aumentar significativamente.

## <a name="to-sign-your-company-up-for-the-bank-data-conversion-service"></a>Para registrar su empresa en el servicio de conversión de datos de banco
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de servicio de conv. de datos del banco** y, a continuación, seleccione el enlace relacionado.  
2. La ventana **Configuración de servicio de conv. de datos del banco** se abre con tres campos rellenados previamente con las URL correspondientes del proveedor del servicio de conversión de datos de banco en .

    **Nota**: Examine el archivo CRONUS International Ltd. se rellenan previamente los campos Nombre de usuario y Contraseña con información de conexión de demostración, los cuales se reemplazarán con la información real de su empresa al registrarse con el servicio de conversión de datos bancarios.
3. En el campo **URL de registro**, seleccione el botón del explorador para abrir la página de inicio de sesión del proveedor de servicios.  
4. En la página de registro del proveedor de servicios del banco, escriba el nombre de usuario y la contraseña correspondientes a la suscripción de su empresa al servicio y, a continuación, complete el proceso de registro tal como indica el proveedor de servicios.

    Su empresa está ahora registrada con el servicio de conversión de datos de banco. Introduzca el nombre de usuario y la contraseña que especificó para el servicio en los campos de configuración relacionados en Dynamics NAV.
5. En la ventana **Configuración de servicio de conv. de datos del banco**, en el campo **Nombre**, introduzca el mismo valor que introdujo como nombre de inicio de sesión en la página del proveedor de servicios en el paso 4.
6. En el campo **Contraseña**, introduzca el mismo valor que introdujo en el campo **Contraseña** en la página del proveedor de servicios en el paso 4.

## <a name="to-encrypt-your-login-information"></a>Para cifrar la información de inicio de sesión
Se recomienda usar esta función para proteger la información de inicio de sesión que se introduce en la ventana **Configuración de servicio de conv. de datos del banco**. Puede cifrar datos en el servidor de Dynamics NAV generando claves de cifrado nuevas o importando claves existentes que se activarán en la instancia del servidor de Dynamics NAV que conecta con la base de datos.

1. En la ventana **Configuración de servicio de conv. de datos del banco**, seleccione la acción **Administración del cifrado**.
2. En la ventana **Administración del cifrado de datos**, habilite el cifrado de los datos.

##<a name="to-view-or-update-the-list-of-currently-supported-bank-data-formats"></a>Para ver o actualizar la lista de formatos de datos de banco actualmente compatibles
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de servicio de conv. de datos del banco** y, a continuación, seleccione el enlace relacionado.
2. En la pestaña **Configuración de servicio de conv. de datos del banco**, seleccione la acción **Nombre banco - Lista conversión de datos** para abrir la lista de nombres de banco que representan los datos de banco que admite el servicio de conversiones.
3. En la página **Nombre banco - Lista conversión de datos**, seleccione la acción **Actualizar lista de nombres de banco**.

Ahora se actualizará la lista de formatos de datos bancarios compatibles con el servicio de conversión de datos bancarios. Esta es la lista de nombres de bancos filtrada por país o región y que se puede seleccionar en el campo **Nombre del banco - Conversión de datos** en la ventana **Ficha de cuenta bancaria**.

**Nota**: La actualización de los formatos de datos bancarios se produce también cuando se selecciona o especifica un valor en el campo **Nombre del banco - Datos de conversión** en la cuenta bancaria.

Se ha registrado en el servicio de conversión de datos de banco. Refleje la información de registro en cada banco que usará el servicio.

## <a name="to-set-up-bank-accounts-to-use-the-bank-data-conversion-service"></a>Para configurar bancos para usar el servicio de conversión de datos de banco
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cuentas bancarias** y, a continuación, seleccione el enlace relacionado.
2. Abra la ficha de un banco del que exportará archivos de banco, o al que los importará, mediante el servicio de conversión de datos de banco.
3. En la ficha desplegable **Transferencia**, en el campo **Formato de exportación de pagos**, seleccione **Servicio de conversión de datos del banco - Transferencia de crédito** para configurar la exportación del pago.
4. En el campo **Nombre del banco - Conversión de datos**, escriba o seleccione el nombre del formato de datos del banco que registró en el paso 4 de la sección "Para registrarse en el servicio de conversión de datos bancarios".
5. Repita los pasos del 1 al 4 para otros bancos que usen el servicio de conversión de datos bancarios.

## <a name="see-also"></a>Consulte también  
[Configurar la banca](bank-setup-banking.md)  
[Administrar cuentas bancarias](bank-manage-bank-accounts.md)

