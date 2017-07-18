---
title: 'Procedimiento: Vender/dar de baja o retirar activos fijos'
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
ms.openlocfilehash: 795bb23e7c0b46be095b2bbdfe7705b3d7b1e4ee
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-dispose-of-or-retire-fixed-assets"></a>Procedimiento: Vender/dar de baja o retirar activos fijos
En el momento de vender o dar de baja un activo fijo, el valor de venta o baja debe registrarse para calcular y anotar las ganancias o las pérdidas. Un movimiento venta o baja debe ser el último movimiento registrado de un activo fijo. Puede registrar más de un movimiento venta o baja en activos fijos que desea dar de baja parcialmente. El total de todos los importes de venta o baja registrados debe ser un crédito.

 **NOTA**: Si negocia con un activo y lo cambia por otro, deberá registrar la venta del activo anterior (venta/baja) y la compra del nuevo (adquisición). Para obtener más información, vea [Procedimiento: Activos fijos adquiridos](fa-how-acquire.md).

## <a name="to-post-a-disposal-from-the-fixed-asset-gl-journal"></a>Para registrar una venta/baja desde el diario general de activos fijos  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.  
2. Cree una línea inicial de diario y rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. En el campo **A/F Tipo registro**, seleccione **Venta/baja**.
4. Elija la acción **Introducir saldo AF**. Se crea una segunda línea de diario para la cuenta contrapartida que se ha configurado para el registro de venta/baja.

    **Nota**: El paso 4 solo funciona si ha configurado lo siguiente: en la ventana **A/F Ficha grupo contable** del grupo contable del activo fijo, el campo **Cuenta de venta/baja** contiene la cuenta de cargo y el campo **Cuenta contrapartida venta/baja** contiene la cuenta contable en la que desea registrar los movimientos de contrapartida para apreciación. Para obtener más información, vea la sección "Para configurar grupos contables de activos fijos" en [Procedimiento: Configurar información general del activo fijo](fa-how-setup-general.md).
5. Seleccione la acción **Registrar**.

Si vende o da de baja parte de un activo fijo, debe dividir el activo antes de poder registrar la transacción de venta/baja. Para obtener más información, consulte [Procedimiento: Transferir, dividir o combinar activos fijos](fa-how-trans-split-combine.md).

## <a name="to-view-disposal-ledger-entries"></a>Para ver movimientos venta/baja  
En el momento de vender o dar de baja un activo fijo, el valor de venta o baja se registra en el libro mayor donde puede ver el resultado.   

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione el activo en el que desea ver los movimientos y, a continuación, elija la acción **Libros amortización**.
3. Seleccione el libro de amortización en el que desea ver los movimientos y, a continuación, elija la acción **Movimientos**.
4. Seleccione una línea con **Venta/baja** en el campo **A/F Categoría registro**, y a continuación seleccione la acción **Navegar**.  
5. En la ventana **Navegar**, seleccione la línea del movimiento de contabilidad y, a continuación, seleccione la acción **Mostrar**.
La ventana **Movs. contabilidad** se abre y puede ver los movimientos que se produjeron al registrar la venta/baja.

## <a name="see-also"></a>Consulte también
[Gestión de activos fijos](fa-manage.md)  
[Configuración de activos fijos](fa-setup.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)

