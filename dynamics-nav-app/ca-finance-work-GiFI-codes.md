---
title: "Procedimiento: Trabajar con los códigos GIFI en Canadá"
author: SorenGP
ms.custom: na
ms.date: 09/21/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 695bca0a6836c47610210b759ae48af27484761f
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

#<a name="how-to-work-with-gifi-codes-in-canada"></a>Procedimiento: Trabajar con los códigos GIFI en Canadá
La información fiscal puede incluir cuentas contables, informes, resultados, balances de situación y estados de cuenta de remanentes. La información se fiscal clasifica mediante códigos. El uso de los códigos ayuda al director a procesar la información, a prepararse para el registro electrónico y a validar la información de impuestos electrónicamente. El uso de los códigos ayuda también a las organizaciones estadísticas a trabajar más eficazmente puesto que la información financiera es más fácilmente accesible. Para obtener más información, vea [la página web de la Agencia de Ingresos de Canadá](http://www.cra-arc.gc.ca/)

La Agencia de Ingresos de Canadá usa el código del Índice General de Información Financiera (GIFI) para recopilar, validar y procesar la información financiera y de impuestos electrónicamente. Se recomienda asignar códigos del GIFI únicamente a las cuentas auxiliares, de forma que todo se realice mediante el software de preparación de impuestos.

Cuando una cuenta está asociada a un código GIFI se informa a la agencia de ingresos que está bajo ese código. Varias cuentas pueden tener el mismo código GIFI pero cada cuenta solo puede tener un código.

Puede exportar la información del saldo con el código GIFI y guardar el archivo exportado en un Excel que será útil para transferir la información en el software de preparación de impuestos.

## <a name="to-set-up-gifi-codes"></a>Para configurar códigos GIFI
En Dynamics NAV deberá configurar los códigos GIFI para las cuentas contables, los informes, los balances de ingresos, las hojas de balance y los extractos de remanentes.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Códigos GIFI** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Códigos GIFI**, seleccione la acción **Nuevo**.
3. Configurar los códigos GIFI rellenando los campos. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

## <a name="to-associate-gifi-codes-with-gl-accounts"></a>Para asignar códigos GIFI a cuentas
Para realizar un informe sobre la información financiera por código GIFI, cada uno de estos debe estar asociado con la cuenta apropiada en el catálogo de cuentas.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Catálogo de cuentas** y, a continuación, seleccione el enlace relacionado.
2. Seleccione una cuenta contable relevante y, a continuación, seleccione la acción **Editar**.
3. En la ficha desplegable **Contabilidad de costos**, en el campo **Código GIFI**, seleccione un código GIFI apropiado.

## <a name="to-view-account-balances-using-the-gifi-code-report"></a>Para ver los saldos de la cuenta usando el informe del código GIFI
Puede revisar los saldos de su cuenta con el código GIFI usando el informe **Saldos de cuenta con código GIFI**.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Saldos de cuenta con código GIFI** y, a continuación, seleccione el enlace relacionado.
2. Especifique qué se debe incluir en el informe rellenando los campos. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Haga clic en el botón **Imprimir** o **Vista previa**.

## <a name="to-export-balance-information-using-gifi-codes"></a>Para exportar información del saldo usando los códigos GIFI
Puede exportar la información del saldo usando los códigos GIFI y guardar el archivo exportado en Excel. Puede modificar, guardar o eliminar el archivo. Puede usar el archivo para transferir información sobre el software de preparación de impuestos.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Exportar info. GIFI a Excel** y, a continuación, seleccione el enlace relacionado.
2. Especifique que desea exportar a Excel rellenando los campos. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Elija el botón **Aceptar**.

**Nota:** El archivo de Excel tiene las características siguientes:

* El saldo se redondea al porcentaje más próximo, pero el valor de celda mantiene el mismo como hace en la contabilidad general.

* Los números negativos se representan como número positivo entre corchetes. Por consiguiente, -123 se representa como (123).

## <a name="see-also"></a>Consulte también
[Finanzas](finance-setup.md)   
[Configurar los procesos financieros más importantes](finance-setup-setup-finance-setup.md)

