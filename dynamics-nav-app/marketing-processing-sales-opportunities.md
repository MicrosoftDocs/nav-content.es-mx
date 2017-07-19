---
title: Procesar oportunidades de ventas
author: jswymer
ms.custom: na
ms.date: 09/16/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 00f316dd3032d41239a75c0f40e6db6dc54601fe
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="processing-sales-opportunities"></a>Procesar oportunidades de ventas
Después de crear una oportunidad, existen numerosas funciones para gestionarla y avanzar hasta completarla.

## <a name="view-opportunities"></a>Ver oportunidades
Las oportunidades de venta existentes están disponibles en la ventana **Lista oportunidades**. Existen varias formas de acceder a esta ventana para procesar las oportunidades de ventas:

|Para ver las oportunidades |Entonces |
|--------------------------|-----|
|Todos los vendedores y contactos|En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Lista oportunidades** y, a continuación, seleccione el enlace relacionado.|
|Un vendedor específico|En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Vendedor** y, a continuación, seleccione el enlace relacionado. Seleccione el vendedor, seleccione la acción **Oportunidades** y, a continuación, seleccione la acción **Lista**.|
|Un contacto específico|En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Contactos** y, a continuación, seleccione el enlace relacionado. Seleccione el contacto de la lista y, a continuación, seleccione la acción **Oportunidades**.|

Todas estas tareas abren la ventana **Lista oportunidades**.

## <a name="close-opportunities"></a>Para cerrar oportunidades
Puede cerrar oportunidades cuando terminen las negociaciones. Al cerrar una oportunidad, puede especificar tanto si las ha ganado como si las ha perdido y también las razones de su cierre. Para especificar una razón, debe configurar los cód. oportunidades cerradas.

1. En la ventana **Lista oportunidad**, seleccione la oportunidad y, a continuación, seleccione la acción **Cerrar**. Se abre la ventana **Cerrar oportunidad**.
2. Rellene los campos relevantes y, a continuación, haga clic en el botón **Aceptar**.

  Los campos **Cód. cierre oportunidad** y **Fecha cerrada** son obligatorios y deben rellenarse antes de hacer clic en **Aceptar**.

  En el campo **Cód. cierre oportunidad**, puede seleccionar entre uno de los códigos cierre oportunidad existentes o agregar uno nuevo. Para agregar un nuevo código, seleccione **Seleccionar de la lista completa** de la lista desplegable y, a continuación, seleccione **Nuevo**. En la nueva línea en blanco, rellene los campos **Código**, **Tipo** y **Descripción** y, a continuación, haga clic en **Aceptar**.

## <a name="create-quotes-for-opportunities"></a>Crear cotizaciones para oportunidades
Puede crear cotizaciones de venta para los contactos que no están registrados como clientes.

1. En la ventana **Lista oportunidad**, seleccione la oportunidad y, a continuación, seleccione la acción **Asignar cotización venta**. Se abre la ventana **Cotización venta**.
2. Rellene los campos pertinentes.

## <a name="create-sales-orders-for-opportunities"></a>Crear órdenes de venta para oportunidades
Puede hacer órdenes de venta a partir de las cotizaciones ventas creadas para las oportunidades. Antes de poder crear órdenes de venta para sus contactos, debe crear el contacto como cliente. Para obtener más información, consulte [Crear un cliente, proveedor o cuenta bancaria a partir de un contacto](marketing-how-create-contacts-new-customers-vendors-bank-accounts.md).

1. En la ventana **Lista oportunidad**, busque la oportunidad para la que creó la cotización de venta.
2. Seleccione las acciones Asignar cotización venta. Aparece la ventana **Cotización venta** para mostrar la cotización de venta asignada a la oportunidad.
3. Rellene los campos adicionales y, a continuación, seleccione la acción **Convertir en orden**.

Al manejar oportunidades de ventas puede ser necesario crear una cotización para el contacto con el que se relaciona la oportunidad.

## <a name="delete-opportunities"></a>Borrar oportunidades
Puede borrar oportunidades, por ejemplo, después de terminar un acuerdo. Sin embargo, solo puede borrar las oportunidades cerradas. Hay dos formas de borrar oportunidades cerradas. Puede eliminar oportunidades cerradas individuales de la ventana **Lista oportunidad** o puede ejecutar el proceso **Eliminar oport. cerradas** para eliminar múltiples oportunidades basándose en los criterios especificados.

Para eliminar oportunidades cerradas de la ventana **Lista oportunidad**, seleccione la oportunidad y, a continuación, seleccione la acción **Eliminar**.

Para borrar oportunidades cerradas usando el proceso **Eliminar oport. cerradas** siga estos pasos:

1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Borrar oportunidades** y, a continuación, seleccione el enlace relacionado.
2. En la sección **Oportunidad** configure los filtros que especifican las oportunidades que se tienen que eliminar.
3. Elija el botón **Aceptar**.

Después de borrar una oportunidad, se elimina de la ventana **Lista oportunidad**.

## <a name="move-an-opportunity-through-sales-cycle-stages"></a>Mover una oportunidad a varias etapas del ciclo de ventas
Si una oportunidad sigue un ciclo de ventas, puede moverla hacia adelante o hacia atrás en las diferentes etapas, por ejemplo, ir a una etapa anterior o posterior e incluso saltarla.

1. En la ventana **Lista oportunidades**, seleccione la acción **Actualizar**. Aparecerá el asistente **Actualizar oportunidad**,
2. Use el campo **Tipo acción** para mover la oportunidad a través de las etapas del ciclo de ventas:
  * **Siguiente** mueve la oportunidad una etapa adelante.
  * **Omitir** mueve la oportunidad hacia adelante una o varias etapas del ciclo de ventas, que usted especifica en el campo **Presentación**. Puede omitir solo las etapas que se han configurado para permitir la omisión.
  * **Anterior** mueve la oportunidad una etapa hacia atrás.
  * **Saltar** mueve la oportunidad hacia atrás una o varias etapas del ciclo de ventas, que usted especifica en el campo **Presentación**.
  * **Actualizar** le permite cambiar la información (por ejemplo, modificar la evaluación de las posibilidades de éxito y valores estimados) sin moverse a otra etapa.
3. Rellene los otros campos requeridos y, a continuación, haga clic en el botón **Aceptar**.

##<a name="see-also"></a>Consulte también  
[Gestionar ventas](sales-manage-sales.md)  
[Crear y gestionar contactos](marketing-contacts.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)

