---
title: "Descripción general de las configuraciones de los productos de servicio y de los componentes del producto de servicio"
description: Conozca los aspectos que debe configurar antes de poder utilizar los productos del servicio, incluidos los valores predeterminados, como el tiempo de respuesta, el porcentaje de descuento del contrato y el grupo de precios de servicio.
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2018
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 0632bdc3b12e60c9b49893df748e8ca165c5b9d4
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-set-up-service-items-and-service-item-components"></a>Cómo configurar componentes de servicio y de productos
Para trabajar con productos de servicio, debe configurar lo siguiente

* Grupos de producto de servicio. 
* Opcional

## <a name="to-set-up-service-item-groups"></a>Para configurar grupos de producto de servicio
Puede establecer los grupos de productos relacionados en relación con la reparación y el mantenimiento. Puede definir valores predeterminados para productos de servicio de un grupo de productos de servicio, como el tiempo de respuesta, el porcentaje de descuento de contrato y el grupo de precios de servicio. Para productos de un grupo de productos de servicio, puede seleccionar si desea que se registren automáticamente como productos de servicio cuando se vendan.  
  
Puede asignar grupos de producto de servicio a productos de la ficha de **producto** y a productos de servicio de la ficha de **producto de servicio**.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Grupos producto servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Cree un grupo de productos de servicio nuevo.  
3. Rellene los campos **Código** y **Descripción**.  
4. En el campo **% Descuento contrato genér.**, introduzca el porcentaje de descuento de contrato genérico que desea que tengan los productos de servicio del grupo.  
5. En el campo **Cód. grupo precio serv. genér.**, introduzca el código de grupo de precio de servicio genérico que desea que tengan los productos de servicio del grupo.  
6. En el campo **Tiempo respuesta genér.(horas)**, introduzca el tiempo de respuesta genérico en horas que desea que tengan los productos de servicio del grupo.  
7. Si desea registrar los artículos del grupo como artículos de servicio cuando se vendan, seleccione el campo **Crea prod. servicio**.  

## <a name="to-set-up-service-item-components"></a>Para configurar componentes de producto de servicio
Los productos de servicio pueden constar de varios componentes que se pueden reemplazar con otros componentes durante el servicio del producto. Estos componentes se configuran en la página **Lista componente producto servicio**. Además, si desea configurar componentes para productos de servicio que sean L.M., puede copiar los productos de la L.M. y los cree como componentes de producto de servicio. 
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos servicio** y, a continuación, seleccione el vínculo relacionado. 
2. Abra el producto de servicio cuyos componentes desea configurar.  
3. Seleccione la acción **Componentes**. Se abrirá la ventana **Lista componente prod. serv.**  
4. Agregue un componente nuevo.  
5. En el campo **Tipo**, seleccione **Producto de servicio** si el propio componente es un producto de servicio registrado. De lo contrario, seleccione **Artículo**.  
6. En el campo **N.º**, seleccione el producto o producto de servicio que sea un componente del producto de servicio.  

## <a name="to-set-up-service-item-components-from-a-bom"></a>Para configurar componentes de producto de servicio desde una L.M.
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Productos servicio** y, a continuación, seleccione el vínculo relacionado.  
2. Abra el producto de servicio para el cual desee configurar componentes desde una L.M.  
3. Seleccione la acción **Componentes**. Se abrirá la ventana **Lista componente prod. serv.**  
4. Elija la acción **Copiar desde L.M.**.  
  
    Si el producto al que está vinculado el producto de servicio es una L.M., los componentes para todos los productos de la L.M. se crearán automáticamente.  

## <a name="to-set-up-a-service-shelf"></a>Para configurar una estantería de servicio
Puede configurar estanterías de servicio que identifiquen dónde almacena los artículos de servicio. Las estanterías de servicio se asignan a los productos de servicio en las páginas **Pedido servicio** y **Hoja trabajo producto servicio**.  
  
1. Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Estanterías servicio** y, a continuación, seleccione el vínculo relacionado.
2. Rellene los campos según sea necesario.

## <a name="see-also"></a>Consulte también
[Cómo configurar códigos para servicios estándar](service-how-setup-service-coding.md)   
[Para configurar la detección de errores](service-how-setup-troubleshooting.md)
