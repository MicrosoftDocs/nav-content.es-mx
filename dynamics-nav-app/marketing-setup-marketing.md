---
title: "Configurar la gestión de marketing y contactos"
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
ms.openlocfilehash: ddeef7532db8e16652ecab06d1303869531be9b2
ms.contentlocale: es-mx
ms.lasthandoff: 06/26/2017

---
# <a name="set-up-marketing-and-contact-management"></a>Configurar la gestión de marketing y contactos
Antes de empezar a trabajar con sus contactos e intereses de marketing, hay algunas decisiones y pasos que debe tomar para configurar la manera en que el área de marketing administra ciertos aspectos de sus contactos. Por ejemplo, puede decidir si sincronizar la ficha de contacto con la ficha de cliente, proveedor o cuenta bancaria, cómo se definirán las series numéricas o qué saludo estándar se usará al escribir a sus contactos.

La gestión de contactos y el establecimiento de una estrategia para identificar, atraer y conservar a los clientes le ayudará a optimizar su negocio y a incrementar la satisfacción del cliente. Asimismo, el uso de un sistema adecuado de gestión de contactos será de gran ayuda en los procesos de creación y mantenimiento de relaciones con los clientes. La comunicación es la clave en estas relaciones. Para lograr el éxito, las empresas deben ser capaces de establecer la comunicación adecuada con sus clientes, proveedores y socios comerciales potenciales y existentes. El establecimiento de una estrategia sobre cómo utilizará la empresa la información de contactos es un paso fundamental. Esta información estará accesible para muchos grupos diferentes de su empresa, por lo que un sistema adecuado incrementará la productividad de todos los usuarios.

Puede configurar la gestión de marketing y de contactos desde la ventana **Configuración de marketing**. Para abrir la ventana **Configuración de marketing**, en la esquina superior derecha, seleccione el icono **Buscar página o informe**, escriba **Configuración de marketing** y seleccione el vínculo relacionado.

## <a name="automatically-copy-specific-information-from-the-contact-companies-to-the-contact-persons"></a>Copiar automáticamente información específica de las empresas de contacto a las personas de contacto
Parte de la información de contacto de las empresas es la misma que la de las personas que trabajan allí, como la dirección. En la sección **Herencia** de la ventana **Configuración de marketing**, puede configurar la aplicación para que copie automáticamente campos específicos de la ficha de empresa de contacto a la ficha de persona de contacto cada vez que cree una persona de contacto de una empresa de contacto. Por ejemplo, puede seleccionar copiar el código de vendedor, los detalles de dirección (dirección, colonia 2, municipio/ciudad, código postal y provincia), los detalles de comunicación (número de fax, respuesta de télex y número de teléfono) y más.

Al modificar uno de estos campos en la ficha Empresa de contacto, el sistema modificará de forma automática el campo de la ficha Persona de contacto, a menos que ese campo se haya modificado manualmente.

Para obtener más información, consulte [Procedimiento: Crear personas de contacto](marketing-how-create-contact-persons.md).

## <a name="use-predefined-defaults-on-new-contacts"></a>Usar valores predeterminados predefinidos en contactos nuevos
Puede hacer que la aplicación asigne de forma automática ciertos códigos de idioma, territorio, vendedor y país/región como valores predeterminados para cada nuevo contacto. También se puede especificar un ciclo de ventas predeterminado que el sistema asignará de forma automática a cada nueva oportunidad creada.

La herencia de campos sobrescribe los valores predeterminados en la configuración. Por ejemplo, si el idioma predeterminado es inglés, pero el de la empresa de contacto es el alemán, el sistema asignará automáticamente el alemán como idioma para las personas de contacto almacenadas de esa empresa.

<!--You can also setup a default salutation that the program automatically assigns to your contacts. You can use these salutations in your interaction template attachments (for example, Microsoft Word documents). When setting up a default salutation, you can enter a salutation text and a salutation format. For example, if the salutation text is Dear, and the salutation format is Salutation Text + Title + Name, the program will automatically enter Dear Mr. John Smith as a salutation for a contact called John Smith.-->

## <a name="automatically-record-interactions"></a>Registrar interacciones automáticamente
Dynamics NAV puede registrar automáticamente los documentos de compras y ventas como interacciones (por ejemplo, órdenes, facturas, recibos, etc.), así como los correos electrónicos, las llamadas telefónicas y las hojas de portada.

Para obtener más información, vea [Registro automático de interacciones con contactos](marketing-auto-record-interactions.md)

## <a name="synchronize-contacts-with-customers-and-more"></a>Sincronizar contactos con clientes, etc.
Para poder sincronizar la ficha del contacto con la del cliente, proveedor y banco, debe seleccionar un código de relación de negocio para clientes, proveedores y bancos. Por ejemplo, solo se puede enlazar un contacto con un cliente existente si seleccionó un código de relación de negocio para los clientes en la ventana **Configuración de marketing**.

Para obtener más información, consulte [Procedimiento: Sincronizar contactos con clientes, proveedores y cuentas bancarias](marketing-synchronize-contacts-customers-vendors-bank-accounts.md).

## <a name="assign-a-number-series-to-contacts-and-opportunities"></a>Asignar una serie numérica a contactos y oportunidades
Puede configurar números de serie para contactos y oportunidades. Si ha configurado una serie numérica para contactos, cuando cree un contacto, pulse Entrar en el campo N.º de la ficha de contacto y el programa introduce automáticamente el siguiente número de contacto disponible.

Para obtener más información acerca de las series numéricas, consulte [Crear series numéricas](ui-create-number-series.md).

## <a name="search-for-duplicate-contacts-when-contacts-are-created"></a>Buscar contactos duplicados al crear contactos
Puede elegir que el sistema busque duplicados de forma automática cada vez que crea una empresa de contacto o buscarlos de forma manual después de crearlos. También puede hacer que el sistema actualice las cadenas de búsqueda de forma automática cada vez que se crea un contacto o se modifica su información. Puede elegir el porcentaje de acierto búsqueda, es decir, el porcentaje de cadenas idénticas que dos contactos deben tener para considerarlos duplicados.

## <a name="set-up-email-logging"></a>Configurar registro de correo electrónico
Puede intercambiar correos electrónicos con sus contactos, clientes, proveedores, etc. Puede enviar y recibir sus mensajes de correo electrónico desde la aplicación o desde Outlook. Antes de que pueda intercambiar mensajes de esta forma y hacer que el sistema los almacene y los ponga en cola, tiene que configurar algunos parámetros, como el intervalo de tiempo en que el sistema comprobará si hay correos electrónicos esperando a procesarse, el nombre de perfil de la conexión con el correo, etc.

## <a name="see-also"></a>Consulte también
[Gestionar contactos](marketing-contacts.md)  
