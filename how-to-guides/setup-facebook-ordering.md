---
description: >-
  Habilitar los pedidos en Facebook permitirá a sus clientes realizar pedidos
  desde su página de Facebook.
---

# Configurar pedidos en Facebook

{% hint style="danger" %}
Por mucho que esta característica suene genial, sinceramente, no es muy agradable para las personas realizar pedidos a través de Facebook. Estas pestañas también solo están disponibles en las versiones de escritorio de Facebook, lo que las limita aún más. Eso significa que no funcionará para los usuarios en sus teléfonos móviles. Facebook también realiza cambios con regularidad y, a veces, las cosas se rompen inesperadamente. Como tal, en general recomendamos no utilizar esta función. Simplemente enviar personas a su dominio de pedidos es una opción mucho más confiable.
{% endhint %}

Visita [https://developers.facebook.com](https://developers.facebook.com). Si aún no ha iniciado sesión en Facebook, puede iniciar sesión con su cuenta habitual de Facebook. Una vez hecho esto, seleccione el botón "Mis aplicaciones" en la parte superior derecha y seleccione "crear nueva aplicación".

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_f92n5y.png)

Ingrese el nombre de su empresa para el nombre de su aplicación junto con su dirección de correo electrónico y presione crear&#x20;

Después de crear la aplicación, accederá al panel de la aplicación. En el menú de la izquierda, vaya a "Configuración > Básico"

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_wtsxiz.png)

Elija "Pestaña Página". Ahora deberá completar la URL de su tienda en "URL de la pestaña de página segura" y cómo desea llamar a la pestaña de su página en "Nombre de la pestaña de la página". La URL de su tienda puede ser su subdominio de Pidello, como "https://tudominio.pidello.com", o su nombre de dominio personalizado si está configurado.

![](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_cb565a.png)

Para agregar la pestaña de la página a su página de Facebook, necesitará su ID de aplicación de Facebook, que verá resaltada en naranja en la foto anterior en la parte superior de la página.&#x20;

A continuación, debe visitar la siguiente URL en su navegador y asegurarse de reemplazarla con su ID de aplicación de Facebook y con la URL de la tienda que ingresó anteriormente.&#x20;

https://www.facebook.com/dialog/pagetab?app\_id=\{{YOUR\_APP\_ID\}}\&redirect\_uri=\{{YOUR\_STORE\_URL\}}&#x20;

Si lo hace correctamente, verá una página en Facebook que dice "Agregar pestaña de página" y podrá seleccionar una de sus páginas de Facebook.&#x20;

Si lo hace correctamente, verá una página en Facebook que dice "Agregar pestaña de página" y podrá seleccionar una de sus páginas de Facebook.
