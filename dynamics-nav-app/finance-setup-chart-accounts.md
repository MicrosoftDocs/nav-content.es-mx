---
title: "Configurar o cambiar el catálogo de cuentas"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 48cd91958545b40b2ab0c5e48442fc874845af5b
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="set-up-or-change-the-chart-of-accounts"></a>Configurar o cambiar el catálogo de cuentas
El catálogo de cuentas muestra las cuentas de contabilidad que almacenan sus datos financieros. Dynamics NAV incluye un catálogo de cuentas estándar que está preparado para respaldar su negocio.
Sin embargo, puede cambiar las cuentas predeterminadas y puede agregar nuevas cuentas.  

## <a name="adding-or-changing-accounts"></a>Agregar o cambiar cuentas
Desde el catálogo de cuentas, puede abrir cada cuenta de contabilidad y agregar o cambiar opciones.

**Nota**: Puede eliminar una cuenta contable. Sin embargo, antes de eliminarla, deben cumplirse las condiciones siguientes:  
- El saldo de la cuenta debe ser cero.  
- El campo **Permite borrar ctas. anteriores a** se debe configurar en la ventana **Configuración de contabilidad** y la cuenta no debe tener movimientos contables en o después de esa fecha.  
- Si se selecciona el campo **Chequear uso ctas. cont.** en la ventana **Configuración de contabilidad**, la cuenta no se debe usar en grupos contables ni en la configuración de grupos contables.  

Dynamics NAV impedirá que elimine una cuenta de contabilidad que almacena los datos que se necesitan en el catálogo de cuentas.  

##<a name="see-also"></a>Consulte también  
[Libro mayor y plan de cuentas](finance-setup-general-ledger.md)  
[Administrar cuentas bancarias](bank-manage-bank-accounts.md)  
[Dimensiones](finance-setup-dimensions.md)  
[Procedimiento: Trabajar con los códigos GIFI en Canadá](ca-finance-setup-work-GiFI-codes.md)

