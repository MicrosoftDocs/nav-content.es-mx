---
title: "Obtener información sobre contabilidad y plan de cuentas"
description: "Describe la contabilidad, el catálogo de cuentas y las categorías de cuenta."
documentationcenter: 
author: edupont04
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 348a1bcbe6908c7bfd84e99245363e733414aeae
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="understanding-the-general-ledger-and-the-coa"></a>Descripción de contabilidad y plan de cuentas
La contabilidad almacena sus datos financieros y el catálogo de cuentas muestra las cuentas donde se registran todos los movimientos contables. [!INCLUDE[d365fin](includes/d365fin_md.md)] incluye un gráfico estándar de cuentas que está preparado para respaldar su negocio.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Configuración de contabilidad y grupos contables
La configuración de la contabilidad es en la base de los procesos financieros porque define cómo se registran los datos.  

En la ventana **Configuración contabilidad** especifique cómo gestionar determinados asuntos de contabilidad en su empresa, como:  

* Detalles de redondeo de factura  
* Formatos de dirección  
* Informes financieros  

De manera similar, en la ventana **Configuración grupos contables**, puede especificar cómo desea configurar las combinaciones generales del negocio y los grupos contables de producto. Los grupos contables asignan entidades como clientes, proveedores, productos, recursos y documentos de venta y compra a cuentas contables. Rellene una línea por cada combinación de grupo contable de negocio y de producto. Para obtener más información, consulte [Configuraciones de grupos de registro](finance-posting-groups.md)  

## <a name="the-chart-of-accounts"></a>Catálogo de cuentas
El catálogo de cuentas muestra todas las cuentas de contabilidad. Desde el catálogo de cuentas, puede realizar acciones como las siguientes:  

* Ver informes que muestran movimientos de contabilidad y saldos.  
* Cierre el resultado.  
* Abrir la ficha de cuenta para agregar o cambiar la configuración.  
* Ver una lista de grupos contables que registran en dicha cuenta.
* Para ver los saldos del Debe y el Haber de una sola cuenta  

Puede agregar, cambiar o eliminar cuentas de contabilidad. Sin embargo, para evitar discrepancias, no puede eliminar una cuenta de contabilidad si sus datos se utilizan en el catálogo de cuentas.  

## <a name="account-categories"></a>Categorías de cuenta
Puede personalizar la estructura de los informes financieros con la asignación de las cuentas de contabilidad a las categorías de cuenta.  

La ventana **Categorías de cuenta** muestra las categorías y subcategorías, y las cuentas que asignó a cada categoría. Puede crear nuevas subcategorías y asignarlas a las cuentas existentes.  

Puede crear un grupo de categorías indentando otras subcategorías debajo de una línea de la ventana **Categorías de cuenta**. Esto le facilita la obtención de una descripción general, porque cada agrupación muestra un balance total. Por ejemplo, puede crear las subcategorías para distintos tipos de activos y a continuación crear grupos de categorías para los activos fijos y los activos circulantes.  

Puede especificar si las cuentas de cada categoría deben incluirse en los tipos específicos de informes. Las categorías de cuentas ayudan a definir el diseño de sus balances financieros.  

Por ejemplo, el estado de cuenta de saldo predeterminado tiene una subcategoría para efectivo en Activo circulante. Si desea que el estado de cuenta de saldo tenga en cuenta la caja chica y la cuenta corriente, puede:  

1. Agregar dos nuevas subcategorías. Una para el efectivo pequeño y otra para su cuenta corriente.  
2. Especifique la definición de informe adicional **Cuentas de efectivo** de estas subcategorías.  
3. Aplique sangría en la subcategoría **Efectivo**.  

La próxima vez que genere las estructuras de cuentas, su estado de cuenta de saldo mostrará un estado de cuenta total de efectivo y dos líneas con estados de cuenta para caja chica y cuenta corriente.  

## <a name="see-also"></a>Consulte también
[Finanzas](finance.md)  
[Configurar o cambiar el plan de cuentas](finance-setup-chart-accounts.md)  
[Inteligencia empresarial](bi.md)  

