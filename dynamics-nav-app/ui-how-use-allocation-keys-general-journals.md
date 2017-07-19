---
title: "Procedimiento: utilizar claves de asignación en diarios generales"
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
ms.openlocfilehash: d239ab62c4be88ccc4a2ce2669dcc2c20a3c0126
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

#  <a name="how-to-use-allocation-keys-in-general-journals"></a>Procedimiento: utilizar claves de asignación en diarios generales
Puede asignar un movimiento en un diario general a varias cuentas diferentes al registrar el diario. La distribución puede realizarse por cantidad, porcentaje o importe.

## <a name="to-set-up-allocation-keys"></a>Para configurar claves de asignación 
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general periódico** y, a continuación, seleccione el enlace relacionado.
2. Seleccione el campo **Nombre de sección** para abrir la ventana **Secciones diario general**.
3. Puede modificar las asignaciones en una sección existente de la lista o crear une nueva sección con asignaciones.
  * Para crear un lote nuevo, seleccione la acción **Nuevo** y vaya al paso siguiente.
  * Para cambiar las asignaciones de un diario existente, seleccione el diario y vaya al paso 7.    
4. En el campo **Nombre**, escriba un nombre para la sección, por ejemplo LIMPIEZA. En el campo **Descripción**, escriba una descripción, por ejemplo, Limpieza de diario de gastos.
5. Cuando haya terminado, cierre la ventana. Aparecerá un nuevo diario periódico vacío. 
6. Complete los campos de la línea.
7. Seleccione la acción **Asignaciones**. 
8. Agregue una línea para cada asignación. Debe rellenar el campo **% Distribución**, **Cantidad a distribuir** o **Importe**. también debe rellenar el campo **N.º de cuenta** y, si distribuye la transacción entre dimensiones globales, los campos de dimensión global.
9. Si escribe un porcentaje en una línea, el importe del campo **Importe** se calcula automáticamente. Estos importes tienen el signo contrario al importe total del campo **Importe** en el diario periódico.
10. Después de introducir las líneas de asignaciones, seleccione **Aceptar** para volver a la ventana **Diario general periódico**. El campo **Importe asignado (USD)** se rellena y coincide con el campo **Importe**.
11. Registre el diario.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Para modificar una clave de asignación que ya haya sido configurada
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diario general periódico** y, a continuación, seleccione el enlace relacionado.
2. En la ventana **Diarios generales periódicos**, seleccione el diario con la distribución.
3. Seleccione la línea con la asignación y, a continuación, seleccione la acción **Asignaciones**.
4. Modifique los campos correspondientes y cierre la ventana.

## <a name="see-also"></a>Consulte también
[Trabajar con diarios generales](ui-work-general-journals.md)  
[Registrar documentos y diarios](ui-post-documents-journals.md)




