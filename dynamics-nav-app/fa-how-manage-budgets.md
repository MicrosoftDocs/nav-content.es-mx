---
title: 'Procedimiento: Gestionar presupuestos de los activos fijos'
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
ms.openlocfilehash: 47b5e0abcae4fab92da5dd9c1bda350a37ec0358
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-manage-budgets-for-fixed-assets"></a>Procedimiento: Gestionar presupuestos de los activos fijos
Puede configurar activos fijos presupuestados. Esto permite incluir cualquier adquisición y venta anticipada en los informes.  

 Para preparar sus presupuestos de resultados, presupuestos de cuentas de balance y el presupuesto de caja, necesitará información acerca de las inversiones futuras, ventas/bajas y depreciación de activos fijos. Puede obtener esta información desde el informe **A/F - Proyección amort**. Antes de imprimir este informe, debe preparar el presupuesto.  

## <a name="to-budget-the-acquisition-cost-of-a-fixed-asset"></a>Para presupuestar el costo de adquisición de un activo fijo
Para preparar presupuestos, necesita configurar fichas de activo fijo para los activos fijos que quiera comprar en el futuro. Los activos fijos presupuestados se configuran como activos normales, pero deben configurarse para que no se registren en el libro mayor.

Al registrar el costo de adquisición, introduzca el número del activo fijo presupuestado en el campo **A/F N.º pptdo.** . Esto provocará que se registre un costo con signo inverso en el activo presupuestado. Significa que el costo total del activo presupuestado es la diferencia entre el costo presupuestado y el real.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Elija la acción **Nuevo** para crear una nueva ficha del activo para el activo presupuestado.
3. Seleccione la casilla **Activo presupuestado** para evitar su registro en el libro mayor.
4. Rellene los campos restantes, asigne un libro de amortización y, a continuación, registre el primer costo de adquisición con el activo fijo presupuestado especificado en el campo **A/F N.º pptdo.** de la línea del diario. Para obtener más información, vea [Procedimiento: Activos fijos adquiridos](fa-how-acquire.md).

## <a name="to-budget-the-disposal-of-a-fixed-asset"></a>Para presupuestar la venta/baja de un activo fijo
Si desea vender activos en el periodo de presupuesto, puede especificar información acerca del precio y fecha de venta.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo que desee dar de baja o vender y, a continuación, elija la acción **Libros amortización**.
3. En la ventana **Libros amortización A/F**, rellene los campos **Fecha prevista venta/baja** y **Ingresos previstos venta/baja**. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

## <a name="to-view-projected-disposal-values"></a>Para ver valores venta/baja previstos
Para ver los valores venta/baja previstos y que se calculen las ganancias y pérdidas, puede usar el informe **Proyección de la amortización A/F**.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proyección de la amortización A/F** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.
3. Haga clic en el botón **Imprimir** o **Vista previa**.

## <a name="to-budget-depreciation"></a>Para presupuestar amortización
Puede usar el informe **A/F - Proyección amort.** para calcular la amortización futura. El informe muestra el valor neto y la amortización acumulada al principio del periodo seleccionado, los cambios durante el periodo y el valor neto y la amortización acumulada al final del periodo seleccionado.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Proyección de la amortización A/F** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.
3. Para ver los valores totales de todos los activos, desactive la casilla **Imprimir por activo fijo**.
4. Deje en blanco la ficha desplegable **Activo** para incluir todos los activos. En el campo **Activo presupuestado**, puede especificar **No** para excluir los activos presupuestados o **Sí** para ver solo los activos presupuestados.
5. Haga clic en el botón **Imprimir** o **Vista previa**.

## <a name="see-also"></a>Consulte también
[Gestión de activos fijos](fa-manage.md)  
[Configuración de activos fijos](fa-setup.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)

