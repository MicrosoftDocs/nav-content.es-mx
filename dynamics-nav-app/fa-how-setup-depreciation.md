---
title: "Procedimiento: Configurar la amortización de los activos fijos"
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
ms.openlocfilehash: 7efc50c673514498de0caa5b3a2dc4b32d4f7f5d
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="how-to-set-up-fixed-asset-depreciation"></a>Procedimiento: Configurar la amortización de los activos fijos
 Puede utilizar varios métodos de amortización para preparar estados de cuenta financieros y devoluciones de impuestos. Muchas grandes empresas utilizan amortizaciones en línea en sus estados de cuenta financieros porque les suele permitir realizar informes de ganancias mayores. Sin embargo, en casos de devolución de impuestos, muchas empresas utilizan un método de amortización acelerado. Para obtener más información, consulte [Métodos de amortización](fa-depreciation-methods.md).

 Cuando cree los libros de amortización pertinentes, debe asignar uno o más a cada activo fijo. Un libro de amortización que se asigna a un activo fijo se lo denomina libro de amortización de activos fijos. Por consiguiente, la ventana de los libros asignados de amortización se denomina **Libros amortización A/F**.

## <a name="to-create-a-depreciation-book"></a>Para crear un libro de amortización  
En un libro de amortización de activos fijos puede especificar la forma en que se amortizarán los activos fijos. Para aplicar distintos métodos de amortización, puede configurar varios libros de amortización.  
1.  En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Libros amortización** y, a continuación, seleccione el vínculo relacionado.
2. En la ventana **Lista libros amortización**, elija la acción **Nuevo**.
3. En la ventana **Ficha libros amortización**, rellene los campos según sea necesario. Seleccione un campo para obtener una breve descripción del campo o el enlace a información adicional.

    **Nota**: Puede registrar transacciones de activos en las ventanas **A/F Diario general** o **Diario activos fijos**, dependiendo de si las transacciones son para la información financiera o la gestión interna. Vaya al siguiente paso para indicar qué tipo de diario se utiliza para las distintas actividades de activos fijos de forma predeterminada.
4. En la ficha desplegable **Integración**, seleccione la casilla de las transacciones de cada actividad de activo que desee registrar en la ventana **A/F Diario general**.
5. Repita los pasos del 2 al 4 para cada método de amortización o de registro que desee asignar a los activos fijos en un libro de amortización.

## <a name="to-assign-a-depreciation-book-to-a-fixed-asset"></a>Para asignar un libro de amortización a un activo fijo  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo fijo para el que desee configurar un libro de amortización de activos fijos.
3. En la ficha desplegable **Ficha libros amortización**, rellene los campos según sea necesario.
4. Si necesita asignar más de un libro de amortización al activo, elija la acción **Añadir más libros amortización**.
5. Opcionalmente, elija la acción **Libros amortización** para especificar uno o más libros de amortización de activos.

**Nota**: Cuando utilice el método de amortización manual, debe introducir la amortización de forma manual en el diario general de activos. La función **Calcular amortización** ignora los activos que utilizan el método de amortización manual. Puede utilizar este método para activos no sujetos a amortización como, por ejemplo, los terrenos.

## <a name="to-assign-a-depreciation-book-to-multiple-fixed-assets-with-a-batch-job"></a>Para asignar un libro de amortización a varios activos fijos con un solo proceso
Si desea asignar un libro de amortización a varios activos, puede utilizar el proceso **A/F Crear libros amortización** para que Dynamics NAV cree automáticamente los libros necesarios.  
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Activos** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el activo al que desea asignarle un libro de amortización y, a continuación, elija la acción **Editar**.
3. En la ventana **Ficha libro amortización**, elija la acción **A/F Crear libros amortización**.
4. En la ventana **A/F Crear libros amortización**, rellene el campo **Libro amortización**.
5. Elija el campo **A/F Copiar desde n. º** y, a continuación, seleccione el número de activos fijos que desea utilizar como base para la creación de los nuevos libros de amortización de activos fijos.

    Si rellena este campo, los campos de amortización de los nuevos libros de amortización de activos fijos contendrán la misma información que los campos correspondientes del libro desde el que va a copiarlos. Deje este campo en blanco si desea crear libros de depreciación de activos fijos con los campos de depreciación vacíos.  
6. En la ficha desplegable **Activo**, puede establecer un filtro para seleccionar los activos para los que desee crear los libros de amortización de activos.
7. Elija el botón **Aceptar**.

## <a name="to-set-up-depreciation-posting-types"></a>Para configurar los tipos de registro de amortización  
Para cada libro de amortización, debe configurar el modo en que desea que Dynamics NAV administre los distintos tipos de registro. Por ejemplo, si el registro debe ser débito o crédito, y si el tipo de registro se debe incluir en la base de amortización.  
1.  En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Libros amortización** y, a continuación, seleccione el vínculo relacionado.  
2. Seleccione el libro de amortización que desea configurar y, a continuación, elija la acción **A/F Config. tipo registro**.
3. En la ventana **A/F Config. tipo registro**, rellene los campos según sea necesario.

**NOTA**: No puede insertar o eliminar líneas en la ventana **A/F Config. tipo registro**. Sólo puede modificar las líneas existentes.

Se recomienda que no cambie la configuración de los libros de amortización de los movimientos que ya se han registrado. Los cambios no afectarán a los movimientos ya registrados, lo que provocaría estadísticas del libro de amortización erróneas.

## <a name="to-set-up-default-templates-and-batches-for-fixed-asset-depreciation"></a>Para configurar las plantillas y los procesos predeterminados para la amortización de activos fijos  
Puede definir para cada libro de amortización una configuración predeterminada para libros y secciones. Utilice esos valores predeterminados para:
- Duplica líneas de un diario a otro.
- Crear líneas de diario con los procesos **Calcular amortización** o **Ajustar valores activos**.
- Duplica los costos en el diario de seguros.

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Libros amortización** y, a continuación, seleccione el vínculo relacionado.
2. Seleccione el libro de amortización en el que desea definir los diarios predeterminados y, a continuación, elija la acción **Configuración del diario A/F**.
3. Si desea tener una configuración predeterminada para cada usuario, elija el campo **Id. usuario** y selecciónela desde la ventana **Usuarios**.
4. En el resto de los campos, seleccione el libro o la sección del diario que debe usarse de forma predeterminada.

## <a name="see-also"></a>Consulte también
[Configuración de activos fijos](fa-setup.md)  
[Gestión de activos fijos](fa-manage.md)  
[Finanzas](finance-setup.md)  
[Este es Dynamics NAV](across-get-started.md)
