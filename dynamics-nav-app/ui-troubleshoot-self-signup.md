---
title: "Solución de problemas en el registro de autoservicio"
author: SusanneWindfeldPedersen
ms.custom: na
ms.date: 09/22/2016
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.prod: dynamics-nav-2017
ms.translationtype: Human Translation
ms.sourcegitcommit: 51adfb3588099c496f0946ff71da5c6fe518f070
ms.openlocfilehash: 931c427518694cbd0003ea82735292a019b388d5
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---

# <a name="troubleshooting-self-service-sign-up"></a>Solución de problemas en el registro de autoservicio
Registrarse en Dynamics NAV es muy fácil y se puede realizar muy rápidamente. Puede crear una cuenta gratuita incluso si es una organización existente. Este recurso aborda los problemas que pueda tener durante el registro.

## <a name="what-email-address-can-i-use-with-dynamics-nav"></a>¿Qué dirección de correo electrónico puedo usar en Dynamics NAV?
Para iniciar sesión, Dynamics NAV requiere una dirección de correo electrónico del trabajo o la escuela. Dynamics NAV no admite direcciones de correo electrónico proporcionadas por servicios de correo electrónico del consumidor ni por proveedores de la telecomunicación. Esto incluye outlook.com, hotmail.com, gmail.com y otros.

Si intenta iniciar sesión con una dirección de correo personal, recibirá un mensaje indicando que use una dirección laboral o educativa.

## <a name="troubleshooting"></a>Solución de problemas
En muchas ocasiones, el registro para Dynamics NAV se puede conseguir siguiendo el proceso de registro. Sin embargo, existen varias razones por las que puede no completar su registro de autoservicio. La tabla siguiente resume algunas de las razones más comunes por las que no le es posible completar el registro y las formas con las que puede solucionar estos problemas.

|Síntoma/Mensaje de error                                                                             |Causa y solución alternativa|
|--------------------------------------------------------------------------------------------------|--------------------|
|Para las direcciones de correo electrónico de Office 365 que no se han registrado en EE.UU., recibirá un mensaje como el siguiente durante el registro: <br>**No funciona, aún no es soportado en su país o región.**<br> |Dynamics NAV actualmente solo admite las cuentas de correo electrónico registradas en Office 365 de los EE. UU.|
|No se admiten las cuentas de correo electrónico personales, como nancy@gmail.com. Recibe un mensaje como el siguiente durante el registro: <br>**Introdujo una dirección de correo electrónico personal: Introduzca su dirección de correo electrónico del trabajo para que se puedan guardar con seguridad los datos de su empresa.**<br> O <br> **Parece una dirección de correo electrónico personal. Introduzca su dirección de trabajo para que podamos conectarle con otros usuarios de la empresa. No se preocupe, no compartiremos su dirección con nadie.** | Dynamics NAV no admite direcciones de correo electrónico proporcionadas por servicios de correo electrónico del consumidor ni por proveedores de telecomunicaciones. Para completar el registro, intente de nuevo usar una dirección de correo electrónico asignada por su trabajo o escuela. Si todavía no puede registrarse y quiere completar un proceso de configuración más avanzado, puede registrarse para una nueva suscripción de prueba de Office 365 y usar esa dirección para registrarse.
|Las direcciones de correo electrónico de .gov o de .mil recibirán un mensaje como el siguiente durante el registro: <br>**Dynamics NAV no disponible: Dynamics NAV no está disponible para usuarios con direcciones de correo electrónico .gov o .mil en este momento. Utilice otra dirección de correo electrónico de trabajo o vuelva más tarde.** <br>O <br>**No se puede finalizar el registro. Parece que Dynamics NAV no se encuentra disponible actualmente para su trabajo o escuela.**|Dynamics NAV no soporta las direcciones de correo de .gov o .mil en este momento.|
|El registro de autoservicio no está habilitado. Recibe un mensaje como el siguiente durante el registro: <br>**No se puede finalizar el registro. Su departamento de TI ha desactivado el registro para Dynamics NAV. Póngase en contacto con ello para completar el registro.** <br>O <br> **Parece una dirección de correo electrónico personal. Introduzca su dirección de trabajo para que podamos conectarle con otros usuarios de la empresa. No se preocupe, no compartiremos su dirección con nadie.**|El administrador IT de su organización ha desactivado el registro de autoservicio para el Dynamics NAV. Para completar el registro, póngase en contacto con su administrador de IT y pídale que siga las instrucciones en la página de abajo para permitir a los usuarios existentes que se registren en Dynamics NAV y para permitir que los nuevos usuarios se unan a su suscriptor existente. También puede experimentar este problema si se registró para Office 365 a través de un socio.|
|La dirección de correo electrónico no es una Id. de Office 365 válida. Recibe un mensaje como el siguiente durante el registro: <br>**No es posible encontrarle en contoso.com. ¿Usa un identificador diferente en el trabajo o en la escuela? Intente iniciar sesión y, si no es posible, póngase en contacto con su departamento de TI.**|Su organización usa identificadores para iniciar sesión en Office 365 y otros servicios de Microsoft que son diferentes a su dirección de correo electrónico. Por ejemplo, su dirección de correo electrónico podría ser Nancy.Smith@contoso.com, pero su identificador ser nancys@contoso.com. Para completar el registro use el id. que su organización le ha asignado para iniciar sesión en Office 365 u otros servicios de Microsoft. Si no sabe qué es, contacte con su administrador IT. Si todavía no puede registrarse y es capaz de completar un proceso de configuración más avanzado, puede registrarse para una nueva suscripción de prueba de Office 365 y usar esa dirección para registrarse.|


## <a name="see-also"></a>Consulte también
[Este es Dynamics NAV](across-get-started.md)  
[Trabajar con Dynamics NAV](ui-work-product.md)




