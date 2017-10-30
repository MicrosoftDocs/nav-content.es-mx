---
title: "Verificación de números CIF/NIF"
description: "Puede usar un servicio web de la UE para verificar que los números de CIF/NIF que introduzca en las fichas de cliente, proveedor o contacto sean válidos."
documentationcenter: 
author: SorenGP
ms.prod: dynamics-nav-2017
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 08/10/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 4fefaef7380ac10836fcac404eea006f55d8556f
ms.openlocfilehash: 8ed345e346ba32a38ebb2738afbe6c12749842ff
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-verify-vat-registration-numbers"></a>Verificación de números CIF/NIF
Puede usar un servicio web de la UE para verificar que los números de CIF/NIF que introduzca en las fichas de cliente, proveedor o contacto sean válidos.  

 Cuando modifique el **RFC/Curp** en una tarjeta donde el valor del campo **Código país/región** es un país/región de la Unión Europea, el nuevo RFC/Curp y su Id. de usuario aparecen en la ventana **Registro de RFC/Curp**. Para verificar un número de CIF/NIF se selecciona el botón **Verificar CIF/NIF** en la ventana **Registro de CIF/NIF**. Se crea una nueva línea cada vez que se usa la función de verificación. Si el número se pudo verificar, el campo **Estado** contiene **Válido**. Si no se puede verificar el número, el campo **Status** contiene **No válido** y se debe modificar el número del campo **RFC/Curp** en la ficha e iniciar la función de verificación de nuevo.  

 La URL del servicio web predeterminado está configurada en el campo **URL de validación de RFC/Curp** en la ventana **Configuración de contabilidad**.  

 En la tabla **Formato RFC/Curp** puede modificar según cada país o región los distintos formatos de número de RFC/Curp que se permite a los usuarios especificar en el campo **RFC/Curp**.  

> [!WARNING]  
>  Este servicio web utiliza el protocolo HTTP, lo que significa que los datos transferidos a través del servicio no están cifrados.  

> [!NOTE]  
>  Puede experimentar tiempos de inactividad para este servicio, de los cuales Microsoft no es responsable, ya que el servicio forma parte de una amplia red de registros nacionales de IVA de la UE.  

## <a name="to-verify-a-vat-registration-number-from-a-customer-card"></a>Para verificar un número de CIF/NIF desde una ficha de cliente  
A continuación se describe cómo comprobar un CIF/NIF para un cliente. Los pasos son parecidos para un proveedor y un contacto.   
1.  Seleccione el icono ![Buscar página o informe](media/ui-search/search_small.png "icono Buscar página o informe"), escriba **Clientes** y, a continuación, seleccione el vínculo relacionado.  

2.  Abra la ficha de un cliente para el cual desee comprobar el número de CIF/NIF.  

    > [!NOTE]  
    >  El campo **Código país/región** en la ficha del cliente debe contener un país o región de la UE.  
3.  En la ficha desplegable **Facturación**, seleccione el botón Análisis junto al campo **RFC/Curp**.  

    La ventana **Registro de CIF/NIF** se abre con una línea en la que el campo **Estado** contiene **No verificado**.  
4.  Seleccione la acción **Comprobar nº reg. mercantil**.  

     Se crea una nueva línea donde el campo **Estado** contiene **Válido** o **No válido**.  
5.  Si el campo **Estado** contiene **No válido**, cambie el número en el campo **RFC/Curp** en la ficha y, a continuación, repita los pasos 3 y 4.  

## <a name="see-also"></a>Consulte también  
[Finanzas](finance.md)  
[Registro de clientes nuevos](sales-how-register-new-customers.md)  
[Registro de proveedores nuevos](purchasing-how-register-new-vendors.md)  
[Trabajar con [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

