---
description: >-
  Aprenda cómo aceptar pagos en línea usando su propia cuenta PayPal con nuestro
  sencillo proceso de configuración
---

# Configurar pagos PayPal

PayPal es uno de los métodos de pago online más utilizados. Pidello utiliza la integración de pago de pago rápido REST de PayPal. Esto nos permite procesar pagos en su nombre y los fondos van directamente a su cuenta. Tenga en cuenta que PayPal sólo está disponible en determinados países y monedas. Puedes verlos [aquí.](https://developer.paypal.com/docs/integration/direct/rest-api-payment-country-currency-support/)

{% hint style="danger" %}
Recomendamos encarecidamente utilizar Stripe en lugar de PayPal para pagos en línea. Según nuestra experiencia, ocasionalmente PayPal tiene varios problemas de servicio. Vea cómo se guían los pagos de Stripe a continuación.
{% endhint %}

{% content-ref url="setup-stripe-payments.md" %}
[setup-stripe-payments.md](setup-stripe-payments.md)
{% endcontent-ref %}

## Cómo funcionan los pagos de PayPal

Una vez que PayPal esté habilitado, la opción estará disponible para los clientes durante la fase de pago de su pedido. Al realizar la selección, pueden iniciar sesión en su cuenta PayPal, crear una cuenta o usar su tarjeta de crédito y realizar el pago como invitado para completar el pago.

## Requerimientos

Para utilizar PayPal con CloudWaitress, necesitará una **cuenta comercial** totalmente válida. Si ya tiene una cuenta comercial de PayPal, puede omitir este paso.

Si aún no tienes uno, regístrate en [https://www.paypal.com/webapps/mpp/account-selection](https://www.paypal.com/webapps/mpp/account-selection). También puede actualizar su cuenta personal a una comercial desde la configuración de su cuenta.

## Conectando tu cuenta de PayPal

#### Crear una aplicación API REST

1. Visita [https://developer.paypal.com/developer/applications/](https://developer.paypal.com/developer/applications/)
2. Inicie sesión en su cuenta PayPal utilizando el botón de inicio de sesión
3. Una vez que haya iniciado sesión, desplácese hacia abajo hasta que vea el título "Aplicaciones API REST".
4. Presione el botón "Crear aplicación"
5. Ingrese el nombre de su empresa para el nombre de la aplicación, ignore el campo de cuenta de desarrollador de sandbox.
6. Presione el botón "Crear aplicación" para completar este paso.

![PayPal REST apps](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_141scma.png)

#### Copiar credenciales de aplicaciones Live

1. After creating your application, you will be on the page where you can copy your credentials
2. Change from the "Sandbox" to "Live" view using the buttons on the top right
3. Scroll down and press "Show" below the "Secret".
4. You will now be able to see your "Client ID" and "Secret" keys
5. In another window, go to your restaurant dashboard and to "Settings > Payments > PayPal"
6. Enable PayPal payments and paste in your "Client ID" and "Secret" key from the PayPal dashboard
7. Choose your payment currency and save the form

![Credenciales Live API de PayPal ](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_1g9uc8i.png)

## Comisiones de PayPal

Tenga en cuenta que al utilizar PayPal, al igual que otros procesadores de tarjetas de crédito en línea, se le cobrará una tarifa por cada transacción. Esto debe ser administrado por usted mismo a través de su propia cuenta PayPal, ya que no somos responsables de esto. Puede utilizar el sitio web de PayPal para ver las tarifas de su país y moneda respectivos.

## Reembolsos

Actualmente, los reembolsos deben procesarse manualmente desde su cuenta PayPal.
