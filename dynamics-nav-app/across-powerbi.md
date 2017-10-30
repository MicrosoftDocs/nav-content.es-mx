---
title: Usar el paquete de contenido de Dynamics NAV para Power BI
author: edupont04
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: ad9519b8ce9c244480308ccc99c05e78e4926b06
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---

# <a name="using-the-dynamics-nav-content-pack-for-power-bi"></a>Usar el paquete de contenido de Dynamics NAV para Power BI
Obtener información de los datos de Dynamics NAV resulta muy sencillo con Power BI y el paquete de contenido de Dynamics NAV. Power BI extrae los datos y, a continuación, genera un panel original e informes en función de los datos.  

El paquete de contenido está preconfigurado para trabajar con los datos de ventas y los datos financieros de la empresa de demostración que aparecerá al registrarse para la versión preliminar de Dynamics NAV.  

- Seleccione cualquier representación visual del panel para traer uno de los siete informes subyacentes.  
- Filtre el informe o agregue los campos que desee supervisar.  
- Ancle esta visualización personalizada al panel para continuar con el seguimiento.  
El panel y los informes subyacentes se actualizan diariamente. Puede comprobar la programación de actualización y modificar la frecuencia en el conjunto de datos.  

## <a name="accessing-dynamics-nav-in-power-bi"></a>Acceder a Dynamics NAV en Power BI
Para visualizar los datos de Dynamics NAV en Power BI, deberá tener lo siguiente:  

- Acceso a Dynamics NAV. Consulte [Dynamics NAV](http://go.microsoft.com/fwlink/?LinkID=759714) para obtener más información.  
- Acceder a Power BI. Para obtener más información, consulte [Power BI](https://powerbi.microsoft.com).

En el sitio de Power BI, podrá encontrar información adicional sobre [cómo agregar el paquete de contenido de Dynamics NAV a Power BI](http://go.microsoft.com/fwlink/?LinkID=760850).  

Para acceder al paquete de contenido de Dynamics NAV en Power BI, deberá especificar la siguiente información en la ventana de conexión:

| Campo       | Descripción              |
|-------------|--------------------------|
|**URL de alimentación de OData**|La URL de OData para que Power BI pueda tener acceso a los datos de su empresa, como https://mybusiness.com:7048/MS/OData/Company('CRONUS%20US').|
|**Método de autenticación**|Seleccione **Básico**.|
|**Nombre de usuario**|La cuenta de correo electrónico con la que iniciaba sesión en Dynamics NAV, como *me@mybusiness.com*.|
|**Contraseña**|Esta es la clave de acceso al servicio web de su cuenta de usuario de Dynamics NAV.|

Esto significa que debe obtener dos tipos de información de Dynamics NAV: la URL de OData y la clave de acceso al servicio web para su cuenta de usuario.  
**Obtener la URL**  
Cuando agregue Dynamics NAV a Power BI, deberá especificar una URL para que Power BI puede tener acceso a los datos de su empresa. En la ventana de conexión, la URL se conoce como **URL de fuente de OData** y debe tener el formato siguiente:

         https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
En este ejemplo, *mybusiness* es el nombre del servicio de Dynamics NAV y *CRONUS US* el de la empresa de demostración con *%20* que representa el espacio del nombre.   
Para obtener la URL, en Dynamics NAV, busque y abra la ventana **Servicios web**. En esta ventana se muestra la lista de servicios web que están disponibles actualmente y puede copiar el enlace desde el campo **URL de OData** para uno de los servicios web de OData predeterminados.  
**Obtener la clave de acceso al servicio web**  
Para usar los datos de Dynamics NAV, en Power BI, en la ventana **Conectar a Dynamics NAV**, deberá especificar su nombre de usuario, que es su la cuenta de correo electrónico, y una contraseña. La contraseña es la clave de acceso al servicio web que se ha configurado para su cuenta de usuario de Dynamics NAV.  
Para obtener una clave de acceso al servicio web, en Dynamics NAV, busque la ventana **Usuarios** y, a continuación, abra la ficha de su cuenta de usuario. En la ficha desplegable **Acceso al servicio web**, copie el contenido del campo **Clave de acceso al servicio web**. Si el campo está en blanco, en la cinta, seleccione **Cambiar la clave de acceso al servicio web**, el campo **La clave nunca caduca** y, a continuación, seleccione el botón Aceptar. A continuación, podrá copiar la clave.  

## <a name="getting-data-from-dynamics-nav"></a>Obtener datos de Dynamics NAV
En el panel de Dynamics NAV se muestran los informes más habituales que tendrá que usar para realizar el seguimiento de la empresa. Los datos se recuperan de su empresa de Dynamics NAV usando los servicios web para leer los datos activos. En Dynamics NAV, en la ventana **Servicios web**, se enumera la lista de servicios web que se han configurado, incluidos los que se consumen por el paquete de contenido en Power BI:  

- ItemSalesAndProfit  
- ItemSalesByCustomer  
- powerbifinance-setup  
- SalesDashboard  
- SalesOpportunities  
- SalesOrdersBySalesPerson  
- TopCustomerOverview  

**Nota**: Si cambia el nombre de cualquiera de estos servicios web, los datos no aparecerán en Power BI.  
Si desea agregar el uso de otros datos en Power BI, deberá buscar las tablas en Dynamics NAV, mostrarlas como servicios web y, a continuación, agregarlas al paquete de contenido. Esto es un ejemplo avanzado y es recomendable que empiece por los datos que ya están disponibles en Power BI.  

## <a name="troubleshooting"></a>Solución de problemas
El panel de Power BI depende de los servicios web publicados que aparecen en la lista anterior y mostrará los datos de la empresa de demostración o de la suya propia si importa los datos de la solución de configuración de finanzas actual. Sin embargo, si se produce algún error, en esta sección se proporcionará una solución para los problemas más habituales.  

**"Error en la validación de parámetros, asegúrese de que todos los parámetros son válidos"**  
Si se muestra este error al introducir la URL de Dynamics NAV, asegúrese de que se cumplen los requisitos siguientes:  

- La URL sigue exactamente este modelo:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
- Elimine cualquier texto después del nombre de la empresa que aparece entre paréntesis  
- Asegúrese de que no haya ninguna barra diagonal al final del URL.  
- Asegúrese de que es una conexión segura tal como indica la URL que empieza por *https*.  


**"Error de inicio de sesión"**  
Si se produce un "error de inicio de sesión" al iniciar sesión en el panel con sus credenciales de Dynamics NAV, la causa puede ser una de los problemas siguientes:

* La cuenta que usa no tiene permisos para leer los datos de Dynamics NAV de su cuenta.

    Verifique la cuenta de usuario en Dynamics NAV y asegúrese de haber usado la clave de acceso al servicio web correcta como contraseña y, a continuación, inténtelo de nuevo.  
* La instancia de Dynamics NAV a la que está intentando conectarse no dispone de un certificado de SSL válido. En este caso, verá un mensaje de error más detallado ("incapaz de establecer una relación de SSL de confianza").

    **Nota**: No se admiten los certificados autofirmados.  


**"¡Vaya!"**  
Si se muestra un diálogo de error del tipo "¡Vaya!" después de pasar el diálogo de autenticación, la causa suele ser un problema de conexión con los datos del paquete de contenido.

* Verifique que la URL siga el modelo que se especificó anteriormente:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')  
* Un error común es indicar la URL completa de un servicio web específico:

    https://mybusiness.projectmadeira.com:7048/MS/OData/Company('CRONUS%20US')/powerbifinance-setup  
* O quizá haya olvidado indicar el nombre de la empresa:

    https://mybusiness.projectmadeira.com:7048/MS/OData/  


## <a name="see-also"></a>Consulte también
[Dynamics NAV](across-get-started.md)  

