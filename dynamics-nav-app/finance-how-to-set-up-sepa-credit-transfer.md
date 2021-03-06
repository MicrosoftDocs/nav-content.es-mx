---
title: "Configurar la transferencia de crédito de SEPA"
description: "Aprenda a configurar la transferencia de créditos SEPA en Dynamics NAV."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sepa, credit, transfer, payment,
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 5dd85579a39fc9bfb3bb362e9573facc0c0a3977
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-sepa-credit-transfer"></a>Configuración de transferencias de crédito SEPA
Desde la ventana **Diario de pagos** se pueden exportar pagos a un archivo para cargarlo en el banco electrónico para procesar transferencias monetarias relacionadas. [!INCLUDE[d365fin](includes/d365fin_md.md)] admite el formato de transferencia de crédito SEPA, pero en su país o región, es posible que haya otros formatos para pagos electrónicos.  

Para habilitar la exportación de formatos de archivos bancarios no compatibles originales en [!INCLUDE[d365fin](includes/d365fin_md.md)], puede configurar una definición de intercambio de datos mediante el marco de intercambio de datos. Para obtener más información, vea [Procedimiento: Configurar las definiciones de intercambio de datos](across-how-to-set-up-data-exchange-definitions.md).  

Para poder procesar el pago electrónicamente exportando los archivos de pago en el formato de transferencia de crédito SEPA, debe realizar los pasos de configuración siguientes:  

* Configure el banco en cuestión para administrar el formato de transferencia de crédito de SEPA  
* Configure las fichas de proveedor para procesar los pagos mediante la exportación de archivos en el formato de transferencia de crédito de SEPA  
* Configure la sección de diario general relacionada para habilitar la exportación de pagos desde la ventana **Diario de pagos**.  
* Conecte la definición de intercambio de datos para uno o varios tipos de pago con la forma de pago correspondiente  

### <a name="to-set-up-a-bank-account-for-sepa-credit-transfer"></a>Para configurar un banco para la transferencia de crédito de SEPA  
1. En el cuadro **Buscar**, escriba **Cuentas bancarias** y, a continuación, elija el vínculo relacionado.  
2. Abra la ficha del banco del que exportará los archivos de pagos en el formato de transferencia de crédito de SEPA.  
3. En la ficha desplegable **Transferencia**, en el campo **Formato de exportación de pagos**, elija **SEPADD**.  
4. En el campo **ID Nº Serie MEN SEPA CT**, seleccione un número de serie desde el cual se asignen números a los movimientos de transferencia de crédito SEPA.  
5. Asegúrese de que el archivo **IBAN** esté rellenado.  

    > [!NOTE]  
    >  El campo **Código divisa** se debe establecer en **EURO**, porque las transferencias de crédito de SEPA solo se pueden realizar en la divisa EURO.  

### <a name="to-set-up-a-vendor-card-for-sepa-credit-transfer"></a>Para configurar una ficha de proveedor para la transferencia de crédito de SEPA  
1. En el cuadro **Buscar**, escriba **Proveedores** y, a continuación, elija el vínculo relacionado.  
2. Abra la ficha del proveedor al que pagará electrónicamente mediante la exportación de archivos de pagos en el formato de transferencia de crédito de SEPA.  
3. En ficha desplegable **Pago**, en el campo **Código método pago**, seleccione **BANCO**.  
4. En el campo **Cuenta bancaria preferida**, seleccione el banco al que se transferirá el dinero cuando se procese por banco electrónico.  

     El valor del campo **Cuenta bancaria preferida** se copia en el campo **Cta. bancaria destinatario** en la ventana **Diario de pagos**.  

### <a name="to-set-the-payment-journal-up-to-export-payment-files"></a>Para configurar el diario de pagos para exportar archivos de pagos  
1. En el cuadro **Buscar**, escriba **Diarios de pagos** y, a continuación, elija el vínculo relacionado.  
2. Abra el diario de pagos que usa para procesar los pagos mediante la exportación de archivos en el formato de transferencia de crédito de SEPA.  
3. En el campo **Nombre sección**, elija el botón de lista desplegable.  
4. En la ventana **Secciones diario general**, de la pestaña **Inicio**, del grupo **Administrar**, elige **Editar lista**.  
5. En la línea del diario de pagos que usará para exportar los pagos, seleccione la casilla **Permitir exportación de pagos**.  

### <a name="to-connect-the-data-exchange-definition-for-one-or-more-payment-types-with-the-relevant-payment-method-or-methods"></a>Para conectar la definición de intercambio de datos para uno o varios tipos de pago con la forma de pago correspondiente  
1. En el cuadro **Buscar**, escriba **Formas de pago** y, a continuación, elija el vínculo relacionado.  
2. En la ventana **Métodos pago**, seleccione la forma de pago que se utiliza para exportar pagos y, a continuación, elija el campo **Definición de línea de exportación de pagos**.  
3. En la ventana **Definiciones de línea de exportación de pagos**, seleccione el código que se ha especificado en el campo **Código** en la ficha desplegable **Definiciones de línea** del paso 4 de la sección "Para describir el formato de líneas y columnas en el archivo” en [Procedimiento: Configurar las definiciones de intercambio de datos](across-how-to-set-up-data-exchange-definitions.md).  

    La orden de domiciliación de adeudo directo se inserta automáticamente en el campo **Id. de orden de domiciliación** de adeudo directo cuando se crea una factura de venta para el cliente que ha seleccionado en el paso 2. Para obtener más información, vea [Crear líneas de ventas y de compras periódicas](sales-how-work-standard-lines.md).  

## <a name="see-also"></a>Consulte también  
[Cobro de pagos mediante adeudo directo SEPA](finance-collect-payments-with-sepa-direct-debit.md)  
[Procedimiento: Configurar las definiciones de intercambio de datos](across-how-to-set-up-data-exchange-definitions.md)  
[Crear líneas de ventas y de compras periódicas](sales-how-work-standard-lines.md)  
[Intercambio de datos electrónicamente](across-data-exchange.md)  

