---
title: 'Procedimiento: Depreciar o amortizar activos fijos'
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
ms.openlocfilehash: af71f30681d436ed5da1cd6cb3c2e13f86558631
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-depreciate-or-amortize-fixed-assets"></a>Procedimiento: Depreciar o amortizar activos fijos
La amortización se utiliza para distribuir el costo de los activos fijos, como maquinaria y equipos, a lo largo de su vida amortizable. Debe definir cómo se amortizará cada activo fijo.  

 Existen dos formas de registrar la amortización:
- Automática, ejecutando el proceso **Calcular amortización** .
- Manualmente, con el diario general de activos fijos.  

Dynamics NAV puede calcular la amortización diaria, lo que le permitirá calcular la amortización de cualquier periodo. Podrá analizar los resultados actuales de la operación de forma mensual, trimestral o anual. El cálculo utiliza un año de 360 días y un mes de 30 días estándar. Para obtener más información, consulte [Métodos de amortización](fa-depreciation-methods.md).

Si se utiliza un activo fijo en varios departamentos, la amortización periódica se puede distribuir automáticamente en esos departamentos según una tabla de distribución definida por usuario.  

Puede anular movimientos de amortización incorrectos con el proceso **A/F Anular movs**. Después, podrá registrar el importe correcto de la amortización con el proceso **Calcular amortización**. Cuando se corrigen errores, se registran como movimientos A/F anulados.  

El ajuste de valores se utiliza para ajustar los valores a los cambios de niveles generales de precio. El proceso **Ajustar valores activos** puede utilizarse para volver a calcular el valor de amortización.  

## <a name="to-calculate-a-depreciation-automatically"></a>Para calcular la amortización de forma manual
Una vez al mes, o cuando desee, puede ejecutar el proceso **Calcular amortización**. Se ignoran los activos fijos vendidos, bloqueados o inactivos y los que utilizan el método de amortización manual.    

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Calcular amortización** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Elija el botón **Aceptar**.  

    El proceso calcula la amortización y crea líneas en el diario general de activos fijos.  
4. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.

    En la ventana **A/F Diario general**, en el campo **N. º días amortización** puede ver los días de amortización calculados.  
5. Seleccione la acción **Registrar**.

## <a name="to-post-a-depreciation-manually-from-the-fixed-asset-gl-journal"></a>Para registrar una apreciación manualmente desde el diario general de activos fijos
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **A/F Diario general** y, a continuación, seleccione el vínculo relacionado.  
2. Cree una línea inicial de diario y rellene los campos según sea necesario.
3. En el campo **A/F Tipo registro**, seleccione **Amortización**.
4. Elija la acción **Introducir saldo AF**. Se crea una segunda línea de diario para la cuenta contrapartida que se ha configurado para el registro de amortizaciones. Para obtener más información, vea la sección "Para configurar grupos contables de activos fijos" en [Procedimiento: Configurar información general del activo fijo](fa-how-setup-general.md).
5. En la pestaña **Inicio**, elija **Registrar** para registrar el diario.

Si configuró las claves de distribución de activos fijos para distribuir importes entre varios departamentos o proyectos, los importes se podrán distribuir durante el registro. Para obtener más información, consulte [Procedimiento: Configurar información general de activos fijos](fa-how-setup-general.md).

## <a name="to-calculate-allocations-in-the-fixed-asset-gl-journal"></a>Para calcular distribuciones en el diario general de activos fijos
Si se utiliza un activo fijo en varios departamentos, la amortización periódica se puede distribuir automáticamente en esos departamentos según una tabla de distribución definida por usuario.  

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **A/F Diario general** y, a continuación, seleccione el vínculo relacionado.   
Cree una línea inicial y rellene los campos según sea necesario.
3. En el campo **A/F Tipo registro**, seleccione **Distribución**.
4. Elija la acción **Introducir saldo AF**. Se crea una segunda línea de diario para la cuenta contrapartida que se ha configurado para el registro de distribuciones.
5. En la pestaña **Inicio**, elija **Registrar** para registrar el diario.

## <a name="use-duplication-lists-to-prepare-to-post-to-multiple-depreciation-books"></a>Use las listas de duplicados para preparar el registro a varios libros de amortización  
Cuando se rellenan las líneas de diario que se van a registrar en un libro de amortización y duplicarlas en un diario independiente desde el que se pueden registrar en otro libro de amortización. Para obtener más información, vea la sección "Para registrar movimientos en distintos libros de amortización".

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Libros amortización** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el libro de amortización correspondiente y, a continuación, seleccione la casilla **Compone lista duplicados**.  

**Importante**: Si ha seleccionado el campo **Utiliza lista duplicados**, no use series numéricas en el diario. La razón es que las series numéricas del diario general de activos no corresponden a las series del diario de activos fijos.

## <a name="to-post-entries-to-different-depreciation-books"></a>Para registrar movimientos en distintos libros de amortización  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **A/F Diario general** y, a continuación, seleccione el vínculo relacionado.
2. En el diario que desee registrar la amortización, seleccione la casilla **Utilizar lista duplicados**.
3. Rellene los campos restantes según sea necesario.
4. Seleccione la acción **Registrar**.
5. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **A/F Diarios** y, a continuación, seleccione el vínculo relacionado.

    La ventana **Diario activos fijos** contiene nuevas líneas para diferentes libros de amortización según la lista de duplicados.   

6. Revise o edite las líneas y, a continuación, seleccione la acción **Registrar**.

**Nota**: Otra forma de duplicar un movimiento en otro libro es especificar un código de amortización en el campo **Duplicado en libro amort.** al rellenar una línea de diario.

Puede copiar los movimientos de un libro de amortización a otro con el proceso **Copiar libro amortización**. El proceso crea líneas de diario en el proceso diario especificado en la ventana **Config. diario activos** para el libro de amortización al que desea copiar. Para obtener más información, consulte el procedimiento siguiente.

## <a name="to-copy-fixed-asset-ledger-entries-between-depreciation-books"></a>Para copiar los movimientos de activos fijos entre los libros de amortización  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Libros amortización** y, a continuación, seleccione el vínculo relacionado.
2. Abra la ficha de libro de amortización correspondiente y, a continuación, elija la acción **Copiar libro amortización**.  
3. En la ventana **Copiar libro amortización**, rellene los campos según sea necesario.  
4. Elija el botón **Aceptar**.  

Las líneas copiadas se crean en el diario general de activos o en el de activos fijos, según si el libro de amortización que va a copiar tiene integración con el libro mayor.

## <a name="see-also"></a>Consulte también
[Gestión de activos fijos](fa-manage.md)  
[Configuración de activos fijos](fa-setup.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)

