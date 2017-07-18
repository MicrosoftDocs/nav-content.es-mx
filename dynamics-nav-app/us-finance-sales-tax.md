---
title: "Impuesto de ventas y grupos de impuestos en EE. UU. y Canadá"
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms-prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: f70a191fc8392bf1685c08c7e905ac96ba7ed069
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="sales-tax-and-tax-groups-in-the-us-and-canada"></a>Impuesto de ventas y grupos de impuestos en EE. UU. y Canadá
Cuando empieza por primera vez a usar Dynamics NAV, puede ejecutar una guía asistida de instalación para configurar rápida y fácilmente la información de los impuestos de venta para su empresa y, opcionalmente, para clientes y proveedores. En cuestión de minutos puede empezar a crear documentos de compra y venta con los impuestos calculados correctamente.
Si cambia a la opción vacía Mi empresa, recomendamos que empiece usando todas las guías asistidas de instalación incluyendo la de los impuestos de venta. Si prefiere configurar los impuestos sin asistente, este artículo explica qué debe tener en cuenta.  

## <a name="tax-groups-tax-areas-and-tax-jurisdictions"></a>Grupos de impuesto, áreas de impuesto y jurisdicciones fiscales
En Dynamics NAV, un grupo de impuesto representa un grupo de productos de inventario o de recursos que están sujetos a los mismos términos de impuesto. Por ejemplo, puede configurar un grupo de impuesto para los productos imponibles y otro para productos no imponibles. Deberá asignar códigos de grupo de impuestos a los productos de inventario y en las cuentas de contabilidad. De manera similar, deberá asignar códigos de área de impuesto a los clientes, las ubicaciones, y a su propia configuración de la empresa. La guía asistida de configuración le ayuda a realizar este proceso.  

Cada área de impuesto es un conjunto de jurisdicciones que cobran el impuesto según un lugar geográfico en particular. Por ejemplo, el área de impuesto de Miami, Florida, incluye tres jurisdicciones del impuesto sobre las ventas: municipio/ciudad (Miami), condado (Dade) y estado (Florida). Dynamics NAV incluye un conjunto limitado de áreas de impuesto con una configuración predeterminada, pero puede modificarlas y agregar nuevas áreas.  

Si configura nuevas áreas de impuesto y jurisdicciones impositivas, debe asegurarse de rellenar los campos correctamente. En los Estados Unidos: los estados, los condados, los municipios/ciudades y las localidades pueden cobrar impuestos. En Canadá: el gobierno federal y las provincias pueden cobrar impuestos. Las empresas recaudan y envían el impuesto de las ventas que se cobra por los productos que venden a los usuarios finales a estos organismos gubernamentales. El impuesto de las ventas también se puede cobrar sobre un impuesto de las ventas existentes. Por ejemplo, se puede calcular el impuesto sobre el importe de una factura de ventas que ya incluya el impuesto gravado por otra jurisdicción.  

En Canadá, los importes del impuesto se deben detallar en los documentos para cada jurisdicción fiscal. Se pueden mostrar hasta cuatro jurisdicciones en un documento, y se combinan las que tengan el mismo orden de impresión cuando se imprimen.

## <a name="tax-details"></a>Detalles impuesto
La ventana **Detalles de impuesto** muestra distintas combinaciones de jurisdicciones del impuesto de ventas y de grupos de impuesto de venta para establecer las tasas del impuesto de ventas. Por cada jurisdicción fiscal, recomendamos que configure un grupo de impuestos para el impuesto de venta normal, otro para productos o servicios que no cobran impuestos y un grupo adicional para cada tipo de producto o servicio que se gestione con una tarifa distinta del impuesto de ventas en dicha jurisdicción.  

En los Estados Unidos, cuando vende a un cliente en un lugar donde no tiene una *sede* (o un domicillio legal en ese estado) no cobra impuesto de las ventas. En lugares donde no tiene una sede, asegúrese de que los campos **Impto. inferior al máximo** e **Impto. superior al máximo** estén en 0.00.  

## <a name="see-also"></a>Consulte también
[Finanzas](finance-setup.md)  
[Configurar finanzas](finance-setup-setup-finance-setup.md)  
[Impuesto sobre bienes y servicios e impuesto de ventas en Canadá](ca-finance-setup-tax.md)  
[Configuración fácil del Impuesto de ventas](https://madeira.microsoft.com/en-us/blog/sales-tax-setup-made-easy)  

