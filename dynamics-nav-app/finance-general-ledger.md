---
title: "Contabilidad y catálogo de cuentas"
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
ms.openlocfilehash: 9965ddcad214e97c5e4858824395d6f651b3c003
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="the-general-ledger-and-the-chart-of-accounts"></a>Contabilidad y catálogo de cuentas
La contabilidad almacena sus datos financieros y el catálogo de cuentas muestra las cuentas donde se registran todos los movimientos contables. Dynamics NAV incluye un catálogo de cuentas estándar que está preparado para respaldar su negocio.

## <a name="general-ledger-setup-and-general-posting-setup"></a>Configuración de contabilidad y grupos contables
La contabilidad y la configuración de cómo los datos se registran en la contabilidad son la base de sus procesos empresariales.
En la ventana **Configuración contabilidad** especifique cómo gestionar determinados asuntos de contabilidad en su empresa. Esto incluye los detalles del redondeo de las facturas, los formatos de dirección y si desea usar una divisa adicional, por ejemplo.
De manera similar, en la ventana **Configuración grupos contables**, puede especificar cómo desea configurar las combinaciones generales del negocio y los grupos contables de producto. Rellene una línea por cada combinación de grupo contable de negocio y de producto.  

## <a name="the-chart-of-accounts"></a>Catálogo de cuentas
El catálogo de cuentas muestra todas las cuentas. Desde aquí, puede abrir los distintos informes que muestran los movimientos de contabilidad y los saldos, y cerrar las cuentas de resultado. Desde cada cuenta, puede la ficha de cuenta y agregar o cambiar la configuración. También puede ver una lista de grupos contables que registran en dicha cuenta.  

Dynamics NAV impedirá que elimine una cuenta de contabilidad que almacena los datos que se necesitan en el catálogo de cuentas.  

## <a name="account-categories"></a>Categorías de cuenta
Con las categorías de cuenta puede asignar las cuentas contables a las categorías como personalización de la estructura de los informes financieros.  

La ventana **Categorías de cuenta** muestra las categorías y subcategorías principales existentes y las cuentas que asignó cada categoría. Puede crear nuevas subcategorías y asignarlas a las cuentas existentes.  

Puede agrupar las categorías de cuenta indentando las subcategorías individuales. Esto le facilita la obtención de una descripción general, porque cada agrupación muestra un balance total. Por ejemplo, puede crear las subcategorías para distintos tipos de activos y a continuación crear grupos de categorías para los activos fijos y los activos circulantes. Puede crear un grupo de categorías indentando otras subcategorías debajo de una línea de la ventana **Categorías de cuenta**.  

Para cada subcategoría puede especificar si las cuentas de esta categoría deben incluirse en los tipos específicos de informes financieros. Las categorías de cuentas ayudan a definir el diseño de sus balances financieros. Por ejemplo, el estado de cuenta de saldo predeterminado tiene un único movimiento para efectivo en activos. Si desea que el estado de cuenta del saldo tenga entradas secundarias de efectivo pequeño y de su cuenta corriente, puede agregar dos nuevas subcategorías, especificar la definición de informe adicional Cuentas de efectivo para cada una de ellas e indentarlas debajo de la subcategoría Efectivo. A continuación, cuando haya generado las estructuras de cuentas basadas en sus cambios, su nuevo estado de cuenta de saldo mostrará un saldo total de efectivo y dos líneas con saldos para caja chica y cuenta corriente.     

##<a name="see-also"></a>Consulte también
[Finanzas](finance-setup.md)  
[Configure o cambie el plan de cuentas](finance-setup-setup-chart-accounts.md)  
[Esquemas de cuentas](finance-setup-account-schedule.md)  

