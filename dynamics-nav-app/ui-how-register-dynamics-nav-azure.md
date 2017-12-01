---
title: "Procedimiento: Registrar Dynamics NAV en el portal de administración de Azure"
author: edupont04
manager: edupont
ms.author: edupont
ms.custom: na
ms.date: 11/15/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2018
ms.translationtype: HT
ms.sourcegitcommit: 6b60b1344a1e18ad91863046110df880f75f7c04
ms.openlocfilehash: d41b96ab5807402a342991d5c5bc2d672db09e2f
ms.contentlocale: es-mx
ms.lasthandoff: 10/16/2017

---
# <a name="how-to-register-dynamics-nav-in-the-azure-management-portal"></a>Procedimiento: Registrar Dynamics NAV en el portal de administración de Azure
Si desea usar los servicios que se basan en Microsoft Azure, debe registrar su Dynamics NAV en el portal de administración de Azure. Por ejemplo, la extensión [Previsión de inventario y ventas](ui-extensions-sales-forecast.md) requiere que se especifique una clave de API y un URI de API, y otros servicios requieren información similar. Por lo tanto, ¿dónde se encuentra esa información?

Puede utilizar la guía **Configurar el portal de administración de Azure** para registrar Dynamics NAV en el portal de administración de Azure y extraer la información que necesita para usar servicios como la extensión Previsión de inventario y ventas, Power BI, Office 365 y así sucesivamente. Debe registrarse en el portal de administración de Azure una sola vez y debe ser administrador o superusuario en Dynamics NAV.

El punto del registro es que Dynamics NAV y el servicio al que desea conectarse deben conocer los detalles de Azure Active Directory (Azure AD) de cada uno.

## <a name="to-register-dynamics-nav-in-the-azure-management-portal"></a>Registrar Dynamics NAV en el portal de administración de Azure
1. Inicie sesión en el portal de administración de Azure en [https://portal.azure.com](https://portal.azure.com). Si no está familiarizado con el portal de administración de Azure, puede encontrar indicaciones en la [biblioteca de documentación de Azure](https://azure.microsoft.com/en-us/documentation/articles).
2. En el panel de navegación izquierdo, elija **Más servicios** y, a continuación, elija **Registros de aplicación**.
3. En el menú superior, elija **Agregar** y, a continuación, en **Crear panel**, rellene los campos con la siguiente información:
    - **Nombre**: especifique un nombre para la solución de Dynamics NAV, como *Dynamics NAV*.
    - **Tipo de aplicación**: elija **Aplicación web*/API**.
    - **URL de inicio de sesión**: introduzca la URL del cliente del explorador de Dynamics NAV, como *https://MiServidor:8080/DynamicsNAV/WebClient/OAuthLanding.htm*.
        El archivo OAuthLanding.htm es un archivo que ayuda a administrar el intercambio de datos entre Dynamics NAV y otros servicios a través de Azure AD.
4. Haga clic en el botón **Crear**.
    Esto agrega Dynamics NAV al **panel de registros de aplicación**, por lo que ahora puede agregarle opciones de configuración.
5. En la **lista de registros de aplicación**, elija la nueva aplicación. Si de este modo no se abre el panel **Configuración**, debería ver una acción para abrir **Configuración**.
6. En el panel **Configuración**, en la sección **Acceso de API**, elija **Claves**.
7. En el panel **Claves**, especifique una descripción y cuándo desea permitir que expire la clave y, a continuación, elija **Guardar**.
8. Copie la clave generada a una ubicación temporal; la necesitará en el procedimiento siguiente.
9. En la sección **Acceso de API**, elija **Permisos requeridos**.
    - Agregar permisos delegados para todos los informes a los servicios de Power BI
    - Agregar permisos delegados para iniciar sesión y leer el perfil de usuario en Windows Azure Active Directory
    - Repita el proceso para otros servicios a los que desee conceder acceso a Dynamics NAV
10. Cierre el panel **Configuración** y, a continuación, en el panel **Essentials**, copie el valor de **Id. de aplicación** a una ubicación temporal.

Ya ha registrado Dynamics NAV en el portal de administración de Azure, se le ha concedido acceso a los servicios relevantes y ha extraído la información que necesita en Dynamics NAV.  

## <a name="to-add-the-information-to-dynamics-nav"></a>Para agregar información a Dynamics NAV
1. En la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Asistente para instalación de aplicaciones de Azure AD** y, a continuación, seleccione el vínculo relacionado.
2. En el asistente, elija **Siguiente**.
3. En el campo **Id. del cliente**, especifique el contenido que copió anteriormente del campo **Id. de aplicación**.
4. En el campo **Clave secreta**, especifique el contenido que copió anteriormente del panel **Claves**.
5. Elija **Siguiente**. Si no ve un mensaje de error, significa que ya ha terminado.

Su Dynamics NAV está registrado y listo para conectarse a servicios como Cortana Intelligence y Power BI.

## <a name="see-also"></a>Consulte también
[Previsión de ventas e inventario](ui-extensions-sales-forecast.md)  
[Configurar Dynamics NAV](setup.md)  

