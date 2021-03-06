---
title: "Seleccione el método de pagos electrónicos"
description: "Procese pagos a sus proveedores exportando un archivo junto con la información de pago desde las líneas de diario."
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/21/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: baafa833fb170fb05f866aac91a05085545aaf97
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Realizar pagos con Servicio de conversión de datos del banco o Transferencia de crédito SEPA
En la ventana **Diario de pagos**, puede procesar pagos a sus proveedores exportando un archivo junto con la información de pago desde las líneas de diario. Después, puede cargar el archivo al banco electrónico donde procesar las transferencias de dinero relacionadas. [!INCLUDE[d365fin](includes/d365fin_md.md)] admite el formato de transferencia de crédito SEPA, pero en su país o región, es posible que haya otros formatos para pagos electrónicos.   

 Para habilitar las transferencias de crédito de SEPA, primero debe configurar una cuenta bancaria, un proveedor y la sección de diario general en el que se basa el diario de pagos. A continuación, prepare los pagos a los proveedores; para ello, rellene automáticamente la ventana **Diario de pagos** con los pagos por vencimientos con fechas de registro específicas.  

> [!NOTE]  
>  Cuando haya comprobado que el banco ha procesado correctamente los pagos, puede continuar con el registro de las líneas del diario de pagos.  

 En la tabla siguiente se describe una secuencia de tareas, con vínculos a temas que las describen.   

|**Para**|**Vea**|  
|------------|-------------|  
|Active la función de servicio de conversión de datos bancarios para convertir los archivos de estado de cuenta de cuenta a un formato que pueda importar o para tener los archivos de pago exportados convertidos al formato que el banco requiere.|[Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md)|  
|Configure un banco, un proveedor y un diario de pagos para la transferencia de crédito de SEPA.|[Configuración de transferencias de crédito SEPA](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Rellenar el diario de pagos con líneas de pagos vencidos a proveedores, con opción de insertar fechas de registro según la fecha de vencimiento de los documentos de compra relacionados.|[Gestionar pagos](payables-manage-payables.md)|  
|Exportar líneas de diario de pagos a un archivo en formato de transferencia de crédito SEPA.|[Exportación de pagos a un archivo de banco](payables-how-export-payments-bank-file.md)|  
|Consulte los pagos que se han exportado y los archivos a los que se han exportado.|Registros de transferencia de crédito|  
|Cuando el banco procese correctamente el pago electrónico, registre los pagos.|[Trabajar con diarios generales](ui-work-general-journals.md)|  

## <a name="see-also"></a>Consulte también  
[Configuración del servicio de conversión de datos bancarios](bank-how-setup-bank-data-conversion-service.md)  
[Configuración de transferencias de crédito SEPA](finance-how-to-set-up-sepa-credit-transfer.md)  
[Gestionar pagos](payables-manage-payables.md)   
[Trabajar con diarios generales](ui-work-general-journals.md)  
[Cobro de pagos mediante adeudo directo SEPA](finance-collect-payments-with-sepa-direct-debit.md)   

