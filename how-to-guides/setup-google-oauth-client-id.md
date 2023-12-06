---
description: >-
  La configuración de la ID de cliente de Google OAuth permitirá a sus clientes
  iniciar sesión a través de su cuenta de Google. Esta guía de soporte lo
  ayudará con el proceso de configuración.
---

# Configure inicio de sesión con Google OAuth Client ID

## Como configurar Google OAuth Client ID

1. Ir a  [Google Cloud Platform Console](https://console.cloud.google.com/).
2. De la lista de proyectos, seleccione un proyecto o cree uno nuevo.
3. Si la página API y servicios aún no está abierta, abra el menú del lado izquierdo de la consola y seleccione API y servicios.
4.  A la izquierda, haga clic en Credenciales.

    <figure><img src="../.gitbook/assets/Screen Shot 2023-10-13 at 5.09.09 AM.png" alt=""><figcaption></figcaption></figure>
5. Haga clic en Nuevas credenciales y luego seleccione ID de cliente de OAuth.

{% hint style="warning" %}
Nota: Si no está seguro de si OAuth 2.0 es apropiado para su proyecto, seleccione Ayúdame a elegir y siga las instrucciones para elegir las credenciales correctas.
{% endhint %}

6. Seleccione el tipo de aplicación apropiado para su proyecto e ingrese cualquier información adicional requerida. Los tipos de aplicaciones se describen con más detalle en las siguientes secciones.
7. Si es la primera vez que crea una ID de cliente, también puede configurar su pantalla de consentimiento haciendo clic en Pantalla de consentimiento. ([El siguiente procedimiento](https://support.google.com/cloud/answer/6158849?hl=en#userconsent\&zippy=%2Cuser-consent) explica cómo configurar la pantalla de consentimiento). No se le pedirá que configure la pantalla de consentimiento después de hacerlo la primera vez.
8. Click en Crear client ID
9. Copiar el Oauth Client ID
10. Vaya a Configuración > Pestaña Sistema > Desplácese hacia abajo hasta Cuenta de cliente > Pestaña Google

    <figure><img src="../.gitbook/assets/Screen Shot 2023-10-13 at 4.55.59 AM.png" alt=""><figcaption></figcaption></figure>
