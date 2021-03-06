---
title: "Configuración y creación de informes Intrastat"
description: "Obtener información sobre cómo configurar las funciones de informes de Intrastat y cómo informar sobre el comercio con empresas de otros países de la UE."
documentationcenter: 
author: bholtorf
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, Intrastat, trade, EU, European Union
ms.date: 08/15/2017
ms.author: bholtorf
ms.translationtype: HT
ms.sourcegitcommit: b9b1f062ee6009f34698ea2cf33bc25bdd5b11e4
ms.openlocfilehash: 1eb3a9a17f07806546022d941f923bc195c7c7fc
ms.contentlocale: es-mx
ms.lasthandoff: 10/23/2017

---
# <a name="how-to-set-up-and-report-intrastat"></a>Procedimiento: configuración y creación de informes Intrastat
Todas las empresas de la Unión Europea deben informar de su comercio con otros países o regiones de la UE. Debe notificar el movimiento de mercancías al organismo de estadística de su país o región todos los meses, y el informe se debe remitir a las autoridades fiscales. Esto se denomina Informes de Intrastat. Para realizar los informes de Intrastat periódicos se usa la página **Diario Intrastat**.  
  
## <a name="required-and-optional-setups"></a>Configuraciones necesarias y opcionales
Para poder usar el diario de Intrastat para informar sobre Instratat, debe configurar algunos parámetros:  
  
* **Libros diario de Intrastat**: debe configurar los libros y secciones del diario de Intrastat que utilizará. Como el informe de Intrastat se realiza mensualmente, debe utilizar 12 procesos de diarios Intrastat basados en el mismo libro.  
* **Códigos de mercancía**: las autoridades aduaneras y fiscales han establecido códigos numéricos que clasificar productos y servicios. Especifique estos códigos para los productos.
* **Códigos de naturaleza de la transacción**: los países y regiones tienen diferentes códigos para los tipos de transacciones de Intrastat, como la compra y venta ordinaria, el intercambio de mercancías devueltas y el intercambio de mercancías no devueltas. Configure todos los códigos que se aplican a su país o región. Utilice estos códigos en los documentos de venta y compra y cuando procese las devoluciones.  
* **Métodos de transporte**: Existen siete códigos de un dígito para los modos de transporte de Intrastat. **1** para mar, **2** para ferrocarril, **3** para carretera, **4** para aire, **5** para correo, **7** para instalaciones fijas y **9** para autopropulsión (por ejemplo, transportar un coche conduciéndolo). Dynamics NAV no requiere estos códigos, sin embargo, recomendamos que las descripciones proporcionen un significado similar.  

Opcionalmente, también puede configurar:

* **Especificaciones de transacción**: se utilizan para complementar las descripciones de los tipos de transacción.  
* **Áreas**: se utilizan para complementar la información sobre los países y regiones.  
* **Puertos y aeropuertos**: se utilizan para especificar las ubicaciones de otros países donde envía o recibe productos. El aeropuerto de Heathrow es un ejemplo de valor de este campo. Introduzca los puertos y aeropuertos en los documentos de ventas y compras en la ficha desplegable **Internacional**. Esta información se copiará también de los movimientos de productos al crear el diario de Intrastat.  

### <a name="to-set-up-intrastat-templates-and-batches"></a>Para configurar libros y secciones de Intrastat
Los trabajos por lotes de Intrastat incluyen solo entradas de elementos y no movimientos de contabilidad. Si tiene movimientos de contabilidad aptos para informes de Intrastat, deberá introducirlos manualmente. Por ejemplo, si compra un equipo desde otro país o región de la UE, el equipo no se coloca en inventario, sino que se registra en una cuenta de contabilidad. Debe introducir este tipo de movimiento manualmente en el diario de Intrastat.  
  
Puede exportar los movimientos a un archivo que puede enviar a las autoridades de Intrastat. También puede imprimir un informe, introducir manualmente la información en formularios de dichas autoridades, y enviar la información.

>  [!Note]
> Es aconsejable crear una sección de diario de Intrastat para cada mes.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Libros diario Intrastat** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]. Cree una plantilla para cada formulario Intrastat que utilice.  
3. Para crear secciones, elija la ficha **Navegar** y, a continuación, seleccione **Secciones**.  
4. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]. Cree una plantilla para cada formulario Intrastat que utilice.  

> [!Note]
> En el campo **Periodo estadístico**, introduzca el periodo en forma de número de cuatro dígitos, donde los dos primeros dígitos representan el año y los dos siguientes el mes. Por ejemplo, escriba 1706 para junio de 2017.

### <a name="to-set-up-commodity-codes"></a>Para configurar códigos de mercancías
Todos los productos que compre o venda deben tener un código de mercancía.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Códigos de mercancías** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Para asignar un código de mercancía a un producto, vaya a la página **Ficha producto**, expanda la ficha desplegable **Costes y registro** y, a continuación introdúzcalo en el campo **Código mercancía**.   

### <a name="to-set-up-transaction-nature-codes"></a>Configurar códigos de naturaleza de transacción
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Especificación de códigos de naturaleza** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

> [!Tip]
> Si utiliza con frecuencia un código de naturaleza de transacción determinado, puede convertirlo en el valor predeterminado. Para ello, vaya a la página **Config. Intrastat** y elija el código. 

### <a name="to-set-up-transport-methods"></a>Configurar métodos de transporte
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Métodos transporte** y, a continuación, seleccione el vínculo relacionado.  
2. Rellene los campos según sea necesario. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-report-intrastat"></a>Para crear informes Intrastat
Después de rellenar el diario de Intrastat, puede imprimir el informe **Prueba** para asegurarse de que toda esa información del diario es correcta. Posteriormente, puede imprimir un informe Intrastat como un formulario o crear un archivo para enviarlo a la autoridad tributaria de su país o región.  

### <a name="to-fill-in-intrastat-journals"></a>Para rellenar diarios Intrastat  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diario Intrastat** y, a continuación, seleccione el vínculo relacionado.  
2. En la página **Diario Intrastat**, en el campo **Nombre sección**, elija la sección relevante del diario y, a continuación, elija el botón **Aceptar**.  
3. Elija la acción **Proponer líneas**. Los campos **Fecha inicial** y **Fecha final** aparecerán con las fechas especificadas como periodo estadístico en la sección de diario.  
4. En el campo **% Costo territorio nacional**, puede introducir un porcentaje que cubra el transporte y el seguro. Si escribe un porcentaje, el contenido del campo **Valor estadístico** del diario es proporcionalmente superior.  
5. Elija **Aceptar** para iniciar el trabajo por lotes.  
  
El proceso recupera todos los movimientos de producto en el periodo estadístico y los inserta como líneas en el diario Intrastat. Puede editar las líneas si es necesario.  
  
> [!IMPORTANT]  
>  El proceso únicamente obtiene los movimientos que contienen un código de país o región para el cual se ha introducido un código Intrastat en la página **Países y regiones**. Por lo tanto, debe escribir los códigos Intrastat de los códigos de país o región para los que se ejecutará el proceso.  

### <a name="how-to-report-intrastat-on-a-form-or-a-file"></a>Procedimiento: Creación de informes Intrastat en un formulario o un archivo
Para conseguir la información necesaria en el formulario Intrastat de las autoridades estadísticas, debe imprimir el informe **Intrastat – Formulario**. Para poder hacerlo, debe preparar el diario Intrastat y rellenarlo. Si tiene transacciones de ventas y de compras, debe completar un formulario independiente para cada tipo, por lo que deberá imprimir el informe dos veces.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios Intrastat** y, a continuación, seleccione el vínculo relacionado.  
2. En la página **Diario Intrastat**, elija la sección relevante de diario en el campo **Nombre sección**.  
3. Si todavía no lo ha hecho, rellene el diario manualmente o elija **Proponer líneas**.  
4. Seleccione la acción **Imprime el diario de intrastat**.  
5. En la ficha desplegable **Lín. diario Intrastat**, agregue un filtro **Tipo** y, a continuación, especifique si es una **Recepción** o un **Envío**.  
6. Haga clic en **Enviar a** para imprimir el informe.  

### <a name="how-to-report-intrastat-in-a-file"></a>Procedimiento: emitir informes de Intrastat en un archivo
Puede entregar el informe Intrastat como un archivo. Antes de crear el archivo, puede imprimir un informe test con la misma información que contendrá el archivo.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diario Intrastat** y, a continuación, seleccione el vínculo relacionado.  
2. En la ventana **Diario Intrastat**, seleccione la sección relevante de diario en el campo **Nombre sección**.  
3. Si todavía no lo ha hecho, rellene el diario manualmente o elija **Proponer líneas**.  
4. Elija la acción **Crear archivo**.  
5. Elija el botón **Aceptar** en la ventana el trabajo por lotes.  
6. Elija **Guardar**.  
7. Busque la ubicación donde desea guardar el archivo y, a continuación, escriba el nombre del archivo y elija **Guardar**. 

## <a name="how-to-reorganize-intrastat-journals"></a>Procedimiento para reorganizar diarios Intrastat
Dado que debe presentar un informe Intrastat cada mes y crear una nueva sección de diario para cada informe, dispondrá de varias secciones de diario. Las líneas de diario no se eliminan automáticamente. Es posible que desee reorganizar los nombres de las secciones de diario periódicamente. Para ello, debe eliminar las secciones de diario que ya no son necesarias. Las líneas de diario de dichas secciones también se eliminan.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Diarios Intrastat** y, a continuación, seleccione el vínculo relacionado.  
2. Para ver las opciones, seleccione el campo **Nombre sección**.  
3. Elija las secciones del diario que desea eliminar y, a continuación, seleccione **Eliminar**.  

## <a name="see-also"></a>Consulte también
[Gestión financiera](finance.md)

## 
