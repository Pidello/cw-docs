---
description: Postmates es un servicio de entrega de última milla que opera en EE. UU.
---

# Como integrar Postmates con Pidello

## Integración POSTMATES

{% hint style="info" %}
**¿En qué ciudades está disponible Postmates?**

[Esta es la lista actualizada de ciudades donde Postmates está disponible](https://cloudwaitresswiki.notion.site/POSTMATES-Integration-ca913853d3ad493eb935d2a5f1120c30#8f10f90feb7a4b94ab35dfdbe0b14158)
{% endhint %}

## How to set-up CloudWaitress > Postmates integration

{% tabs %}
{% tab title="¿Cómo generar el Webhook?" %}
1 - Inicie sesión en la cuenta de Postmates en - partner.postmates.com

2 - Haga clic en Desarrollador > Webhooks > Crear webhook.

3 - Pegue la URL de la API en la sección 'Webhooks' de Producción y Sandbox. La URL de API para el webhook se puede encontrar en el panel de control de su restaurante en configuración > integraciones > Postmates > URL del webhook de Postmates.

![](../.gitbook/assets/generate-postmates-webhook.png)
{% endtab %}

{% tab title="Configuraciones para probar" %}
Para realizar pruebas, asegúrese de que los 'tiempos de espera y estados automáticos' estén configurados como se muestra a continuación;

Confirmar = Encendido a los 0 minutos

Listo = Encendido a 0min

![](../.gitbook/assets/postmates-testing-settings-cloudwaitress.png)
{% endtab %}

{% tab title="Claves Requeridas" %}
A continuación se encuentran las claves en Postmates que necesitará usar al agregar a la configuración de integración de Shipday dentro del restaurante (Configuración > Integraciones > Postmates);

* Clave Sandbox (Clave de autenticación para pruebas)
* Clave de producción (Clave de autenticación para vivo)
* Identificación del cliente
* Secreto de firma

![](../.gitbook/assets/postmates-required-keys.png)

Agregue los valores de su cuenta de Postmates como se indica a continuación (Configuración > Integraciones > Postmates);

![](../.gitbook/assets/settings-integration-postmates.png)
{% endtab %}

{% tab title="UI para realizar pedidos" %}
Los postmates se mostrarán durante el proceso de pago;

![Postmates delivery estimation in checkout](../.gitbook/assets/postmates-checkout-ui.png)

Postmates deliveries will show on the dashboard with the Postmates logo;

![Postmates logo shows in the CloudWaitress order dashboard](../.gitbook/assets/postmates-dashboard-ui.png)
{% endtab %}
{% endtabs %}

## Creando una cuenta de Postmates

Agregar Postmates como su servicio de entrega es simple y le ayudará a aumentar sus ventas a los clientes que desean que el pedido se entregue directamente en su puerta.

**Configurar la cuenta y el método de pago**

Primero deberá crear una cuenta de desarrollador de Postmates que puede encontrar en este enlace: [https://postmates.com/developer](https://postmates.com/developer)

Una vez que ingrese la información de su restaurante, será redirigido al Panel de Postmates. Para obtener la información de Postmates que necesitamos, debe ingresar un método de pago para que Postmates pueda cobrarlo una vez que se complete el pedido. Para hacer esto, haga clic en "Agregar tarjeta de pago", ingrese la información de su tarjeta de crédito y "Guardar". Ahora que ha ingresado la información de su tarjeta de crédito, verá aparecer algunas "claves" diferentes en la pantalla.

## AJUSTES ESENCIALES

{% hint style="warning" %}
IMPORTANTE - Se deben aplicar las siguientes configuraciones para que funcione la integración de Postmates.
{% endhint %}

**En Pidello se deben aplicar las siguientes configuraciones;**

1\. Genere y agregue el webhook a Postmates (detalles arriba)

2\. Agregue las claves de Postmates al panel del restaurante. Configuración > Integraciones > Postmates.

3\. Configuración > Servicios > Entregas > Tarifas > Ninguna

![](../.gitbook/assets/postmates-essential-settings-1.png)

4\. Configuración > Servicios > Entregas > General > Proveedor de entrega predeterminado = Postmates

![](../.gitbook/assets/postmates-essential-settings-2.png)

5\. Configuración > Servicios > Entregas > Tiempos de espera y estados automáticos

Las siguientes configuraciones DEBEN estar habilitadas;

* Tiempo hasta confirmar (minutos)
* Tiempo hasta que esté listo (minutos)
* Tiempo hasta estar en ruta (minutos)

Nota: Puedes establecer diferentes tiempos para estos campos y puedes usar los otros campos dentro de esta sección; sin embargo, esto no afectará la integración de Postmates.

![](../.gitbook/assets/postmates-essential-settings-3.png)

## Preguntas Frecuentes

* **¿Qué pasa si ya tengo una cuenta de Postmates y estoy en su aplicación? ¿Aún necesito una cuenta de desarrollador?** Ya debería tener acceso a la sección Desarrollador de Postmates y todo lo que tendrá que hacer es copiar las claves existentes en el Panel de administración de Pidello.
