---
description: >-
  Aprenda cómo configurar Stripe, nuestro proveedor de pagos en línea
  recomendado debido a su configuración optimizada y experiencia de usuario.
---

# Configurar pagos de Stripe



{% hint style="success" %}
Recomendamos usar [stripe+-integrated-payments.md](stripe+-integrated-payments.md "mention")
{% endhint %}

Puedes aceptar pagos con tarjeta en línea usando [Stripe](https://stripe.com/). Actualmente es compatible con numerosos países con una variedad de monedas. Si Stripe no es compatible en tu país, puedes solicitar probar Stripe Atlas. A continuación se muestra nuestra guía sencilla sobre cómo configurar Stripe y administrar su cuenta.

## Cómo funcionan los pagos de Stripe

Cuando Stripe está habilitado, los clientes pueden elegir entre la opción de pago en línea al realizar el pago. Si un cliente selecciona "Tarjeta", el campo de la tarjeta de crédito/débito se desplegará a continuación.

![Stripe payment example](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_16wk7ks.png)

## Conectando tu cuenta Stripe

1. Cree una cuenta en el sitio web de Stripe si aún no tiene una.
2. Asegúrese de estar viendo su cuenta real y no su cuenta de prueba.
3. Inicie sesión en el panel de su cuenta. En la navegación de la izquierda, vaya a "Desarrolladores > Claves API".
4. A continuación, abre el panel de tu restaurante y navega hasta "Configuración > Pagos > Stripe".
5. Habilite los pagos de Stripe usando el interruptor "Habilitar"
6. Copie la "Clave publicable" y la "Clave secreta" del panel de Stripe al panel del restaurante.
7. Configure su moneda de pago en el panel del restaurante y guarde la configuración.

![Stripe API keys](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_4cpfy8.png)

## Haciendo pruebas

Si desea realizar un pago de prueba, copie sus claves API de prueba de Stripe. Puede hacerlo activando el interruptor "Ver datos de prueba".

![Stripe test data](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_1bjx53a.png)

Una vez hecho esto, podrá utilizar el número de tarjeta de crédito "4242 4242 4242 4242" con cualquier vencimiento válido, CVC y código postal. Esta tarjeta le permitirá realizar un pago ficticio.

## Validando tu cuenta de Stripe

Para retirar pagos en línea a su banco, deberá asegurarse de que su cuenta Stripe sea completamente válida. Por favor, asegúrese de haber completado todas las validaciones requeridas.

## Stripe Fee's

We are not responsible for your Stripe account management or fees. Your Stripe account is simply linked to your CloudWaitress account to process charges on your behalf with the money going straight to your account.

As such it is important you are aware of Stripe's payment processing fees. You can read more here [https://stripe.com/pricing](https://stripe.com/pricing). Please also take the time to read their FAQ and support to clear up any issues you may have.

## Stripe Currency Conversions

Stripe enables you to accept different currencies online depending on the country you are in. If your Stripe currency is different from your store currency, we will convert the order amount to your Stripe default currency using real-time exchange rates for payment to be made.

## Issuing Refunds

Stripe refunds can be processed from your order management dashboard or the Stripe dashboard. In the order management dashboard, the refund payment option is available in the order details popup. Simply press the action select bar and choose "Refund Stripe Payment".
