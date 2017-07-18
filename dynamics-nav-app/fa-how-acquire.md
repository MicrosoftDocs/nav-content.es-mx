---
title: 'Procedimiento: Adquirir activos fijos'
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
ms.openlocfilehash: 5b58a6cf0a0c22c8076082328f92725cb7dbc4d1
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-acquire-fixed-assets"></a>Procedimiento: Adquirir activos fijos
Deberá configurar una ficha con la información de cada activo fijo. Puede configurar los edificios o los bienes de producción como activos principales con una lista de componentes y puede agruparlos de diferentes maneras como, por ejemplo, por clase, departamento o ubicación. Un libro de amortización debe estar configurado y asignado a cada activo fijo antes de que pueda adquirirlo.

Cuando se ha configurado un activo fijo y se le ha asignado un libro de amortización, debe adquirir el activo fijo. Para adquirir un activo fijo, registre el costo de adquisición en la cuenta de contabilidad, la cuenta bancaria o el proveedor correspondientes al registrar una transacción de adquisición desde la ventana **A/F Diario general**. Puede utilizar la ventana **Adquisición activos asistida** para crear y registrar las líneas del diario general requeridas automáticamente.

El valor residual es el valor restante de un activo fijo cuando ya no se puede utilizar. Puede registrar el valor residual en el momento de registrar el costo de adquisición. Para obtener más información, consulte [Procedimiento: Depreciar o amortizar activos fijos](fa-how-depreciate-amortize.md).

El ajuste de valores se utiliza para ajustar los valores a los cambios de niveles generales de precio. El proceso **Ajustar valores activos fijos** puede utilizarse para calcular los costos de adquisición como de sustitución.

## <a name="to-create-a-fixed-asset-and-acquire-it-automatically"></a>Para crear un activo fijo y adquirirlo automáticamente
El procedimiento siguiente describe cómo crear un activo y después adquirirlo utilizando la ventana **Adquisición activos asistida** para crear y registrar las líneas necesarias del diario general de activos. También puede crear y registrar las líneas de diario manualmente. Para obtener más información, consulte la sección "Para registrar la adquisición de un activo fijo manualmente con el diario general de activos fijos".

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.  
2. Elija la acción **Nuevo** y, a continuación, rellene los campos de la ficha desplegable **General** como sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. En la ficha desplegable **Ficha libros amortización**, rellene los campos según sea necesario. Este paso asigna un libro de amortización al activo fijo.  
4. Si necesita asignar más de un libro de amortización al activo, elija la acción **Añadir más libros amortización**. Para obtener más información, vea la sección "Para asignar un libro de amortización a un activo" en [Procedimiento: Configurar la amortización de los activos fijos](fa-how-setup-depreciation.md).

    Cuando estén rellenados todos los campos requeridos para adquirir un activo, aparecerá la notificación **Está listo para adquirir el activo. Adquirir** en la parte superior de la página.
5. Seleccione la acción **Adquirir** en la notificación.
6. Siga los pasos de la ventana **Adquisición activos asistida** para completar la adquisición automática del activo.

**Nota**: Puede registrar los costos de adquisición como créditos. En ese caso, recuerde que el valor del campo **Costo con IVA** debe tener el símbolo menos que indica un crédito.

Cuando elige **Finalizar**, se rellena el campo **Valor libro** de la ventana **Ficha activo fijo** que indica que el activo fijo se ha adquirido según el costo especificado.  

## <a name="to-set-up-a-component-list-for-a-main-asset"></a>Para configurar una lista de componentes para un activo principal  
Puede agrupar los activos fijos en activos principales y sus componentes. Por ejemplo, puede tener un equipo de producción que consista en muchas partes, las cuales desea agrupar de esta manera.  

Tanto el activo principal como todos sus componentes deben configurarse como fichas individuales de activos fijos. Después de configurar una lista de componentes, Dynamics NAV rellena automáticamente los campos **Principal/Componente** y **Componentes de activo principal** de las fichas de activos fijos.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo principal y, a continuación, elija la acción **Componentes activo ppal**.
3. En la ventana **Componentes activo ppal.**, elija el campo **A/F n. º** y, a continuación, seleccione el activo fijo que desea agregar como componente del activo principal.
4. Cierre la ventana.
5. Repita los pasos 3 y 4 para cada componente que desee agregar.
6. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración activos** y, a continuación, seleccione el vínculo relacionado.
7. Seleccione la casilla de verificación **Permitir reg. en activos pples**.

## <a name="to-post-a-fixed-asset-acquisition-manually-with-the-fixed-asset-gl-journal"></a>Para registrar una adquisición de activo manualmente con el diario general de activos fijos
El procedimiento siguiente describe cómo adquirir un activo manualmente creando y registrando líneas en la ventana **A/F Diario general**. También puede adquirir un activo de manera automática utilizando la ventana **Adquisición activos asistida**. Para obtener más información, consulte el paso 5 en la sección "Para crear un activo fijo y adquirirlo automáticamente".

**Nota**: Puede registrar los costos de adquisición como créditos. En ese caso, recuerde que el valor del campo **Importe** debe tener el símbolo menos que indica un crédito.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Diarios generales A/F** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **A/F Diario general**, en el campo **A/F Tipo registro**, seleccione **Costo**.
3. Rellene los campos restantes según sea necesario.
4. Seleccione la acción **Registrar**.  

**Sugerencia**: Si rellena el campo **N. º seguro** del diario general de activos fijos en el momento de registrar un costo, Dynamics NAV también registrará el costo del activo fijo en los movimientos de cobertura de seguro. Para obtener más información, vea [Procedimiento: Asegurar activos fijos](fa-how-insure.md).

## <a name="to-cancel-an-acquisition-cost-posting-for-one-fixed-asset"></a>Para anular el registro del costo de adquisición de un activo fijo
Si se equivoca al registrar un costo, puede eliminar el movimiento mediante el proceso **Cancelar movs. A/F** y registrar seguidamente el movimiento de adquisición correcto. Los movimientos incorrectos se transfieren a la ventana **A/F Movs. anulados**.

Por ejemplo, si registra una adquisición con la fecha incorrecta, debe corregirla lo más pronto posible porque la fecha de registro de un activo fijo se utiliza para realizar muchos cálculos importantes.

**Importante**: No puede usar la función **Transacciones inversas** para los movimientos de un activo.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cancelar movs. A/F** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.
3. Elija el botón **Aceptar** para iniciar el trabajo por lotes.
4. Cuando se hayan cancelado el movimiento o los movimientos incorrectos, registre el costo correcto.

Para anular los movimientos de varios activos fijos a la vez, use el proceso **A/F Anular movs**.

## <a name="to-post-the-salvage-value-together-with-the-acquisition-cost"></a>Para registrar el valor residual junto con el costo de adquisición  
Puede registrar el valor residual junto con el costo de adquisición a partir del diario general de activos fijos.    

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Cancelar movs. A/F** y, a continuación, seleccione el vínculo relacionado.
2. Cree la línea de adquisición del diario. Para obtener más información, consulte la sección "Para registrar la adquisición de un activo fijo manualmente con el diario general de activos fijos".
3. En el campo **Valor residual** de la línea del diario, escriba el importe del valor residual como abono (con un signo menos).
4. Seleccione la acción **Registrar**.

**Nota**: El tipo de registro **Valor residual** es una opción exclusiva del **Diario de activos**. No está disponible en la ventana **A/F Diario general** porque el valor residual nunca se registra en el libro mayor.

## <a name="see-also"></a>Consulte también
[Gestión de activos fijos](fa-manage.md)  
[Configuración de activos fijos](fa-setup.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)

