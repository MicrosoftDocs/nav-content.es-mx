---
title: "Previsión de inventario y ventas"
author: edupont04
ms.custom: na
ms.date: 09/23/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 765527ed4f4800acec20f0abbd4374e95c9c36dc
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="sales-and-inventory-forecast-for-dynamics-nav"></a>Previsión de inventario y ventas para Dynamics NAV
La gestión del inventario es un equilibrio entre el servicio al cliente y la administración del costo. Por un lado, un inventario bajo requiere menos capital de trabajo, pero, por otro lado, la falta de existencias puede llevar potencialmente a la pérdida de ventas. La extensión Previsión de inventario y ventas pronostica ventas potenciales con datos históricos y ofrece una visión general clara de la falta de existencias prevista. Según la previsión, la extensión ayuda a crear solicitudes de reposición a los proveedores y le ahorra tiempo.  

## <a name="setting-up-forecasting"></a>Configurar la previsión
En Dynamics NAV, debe configurar la conexión a Azure Machine Learning (Azure ML). Para obtener más información, vea [Procedimiento: Registrar Dynamics NAV en el portal de administración de Azure](ui-how-register-dynamics-nav-azure.md). Una vez haya establecido la conexión, puede configurar la previsión para que utilice diferentes tipos de periodo de información como, por ejemplo, cambiar la previsión mensual por la trimestral. También puede elegir el número de periodos para calcular la previsión según como desea que sea. Sugerimos que utilice la previsión mensual y con un horizonte de 12 meses.  

## <a name="using-the-forecasts"></a>Usar las previsiones
La extensión usa las capacidades de Azure ML para pronosticar las ventas futuras en función del historial de ventas para ayudarle a evitar la escasez de inventario. Por ejemplo, cuando elige un producto en la ventana **Productos**, la ficha del panel **Previsión del producto** muestra las ventas futuras estimadas de ese producto. De esta manera podrá ver si pronto agotará el stock del producto.  

También puede utilizar la extensión para sugerir cuándo desea almacenar el inventario. Por ejemplo, si crea una orden de compra para Fabrikam porque desea comprar su nueva silla de escritorio, la extensión de Previsión de inventario y ventas sugerirá que también reaprovisione la silla giratoria LONDON que normalmente le compra a ese proveedor. Eso se debe a que la extensión prevé que se le agotará el stock de la silla giratoria LONDON durante los próximos dos meses, de modo que es posible que desee pedir más sillas ahora.  

## <a name="see-also"></a>Consulte también
[Gestionar ventas](sales-manage-sales.md)  
[Gestionar inventario](inventory-manage-inventory.md)  
[Personalizar Dynamics NAV usando extensiones](ui-extensions.md)  
[Procedimiento: Registrar Dynamics NAV en el portal de administración de Azure](ui-how-register-dynamics-nav-azure.md)  

