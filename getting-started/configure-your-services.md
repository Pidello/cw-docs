---
description: >-
  Los servicios de su restaurante representan los distintos tipos de pedidos que
  acepta. Vea nuestro vídeo para obtener una explicación detallada de todas las
  configuraciones disponibles.
---

# Configura tus Servicios

{% embed url="https://youtu.be/EUW9nZVAE68" %}
Services video tutorial
{% endembed %}

Actualmente hay 4 servicios disponibles. Ellos son:

* **Recoger en tienda (Pick Up):** pedidos que los clientes recogen en la tienda para llevar&#x20;
* **Entrega a domicilio (Delivery):** pedidos que se entregan en la dirección del cliente.&#x20;
* **Ordena y paga en Restaurante:** pedidos realizados por clientes actualmente sentados en su tienda.&#x20;
* **Reserva de mesa:** una reserva realizada para una fecha y hora posteriores

## Cómo configurar tus Servicios

1. Visita el panel de tu restaurante y ve a la página de configuración.
2. Seleccione la pestaña "Servicios" y edite su configuración según sea necesario

## Habilitación y deshabilitación de servicios

Puede habilitar o deshabilitar servicios según sea necesario. Vaya a la configuración del servicio deseada y simplemente active el interruptor "Activado" para habilitarlo o deshabilitarlo.

{% hint style="info" %}
Debes tener al menos un servicio habilitado
{% endhint %}

## Notas de Servicio

Puede agregar notas personalizadas para cada servicio que se mostrarán al cliente cuando lo seleccione. Útil si necesita transmitir un mensaje importante a su cliente

## Tiempos de pedidos

Un cliente solo puede realizar un pedido con vencimiento inmediato si su tienda está abierta. Los pedidos para una fecha posterior deben programarse dentro de su horario de atención. Como tal, los horarios de los pedidos están controlados principalmente por el horario de apertura de su tienda. A partir de ahí, cada servicio tiene su propia configuración de tiempo de pedido independiente que le permite un control más profundo.

### Habilitar y deshabilitar tiempos de pedido

En la pestaña "Horarios de pedidos" en la configuración del servicio, puede habilitar y deshabilitar pedidos inmediatos y programados.

### Compensación de primer orden

Este es el período de tiempo desde que abre su tienda por primera vez hasta que acepta el primer pedido. Por ejemplo, si el primer pedido se establece en 30 minutos y su tienda abre a las 9:00 am, el primer pedido se puede realizar o programar a las 9:30 am.

### Compensación del último pedido

Este es el período de tiempo desde que cierra su tienda hasta que se acepta el último pedido. Por ejemplo, si la compensación del último pedido se establece en 30 minutos y su tienda cierra a las 9:00 pm, el último pedido se puede realizar o programar a las 8:30 pm.

### Order Offset

La compensación de orden normal solo se aplica a órdenes programadas para un momento posterior. Este es el período a partir de ahora en el que se puede realizar un pedido programado. Por ejemplo, está ahí para evitar que los clientes programen pedidos en los próximos 10 minutos en lugar de simplemente pedir que venzan lo antes posible.

Entonces, por ejemplo, si el desplazamiento de su pedido es de 30 minutos y la hora actual son las 6:00 pm, la próxima vez que un cliente puede programar un pedido sería a las 7:00 pm Si lo quieren antes de las 7:00 pm, aún pueden realizar el pedido lo antes posible. Si el desplazamiento del pedido fue de 15 minutos, entonces el cliente puede realizar el pedido a las 6:30 pm.

La compensación del pedido también actúa como un punto de corte para darle tiempo para cumplir con el cronograma del pedido. Por ejemplo, si son las 6:00 pm y el desplazamiento de su pedido es de 30 minutos. Si el cliente programa un pedido para las 7:00 pm, deberá realizarlo antes de las 6:30 pm. Esto es para darle 30 minutos para cumplir con el tiempo programado.

If they take too long and the time passes 6:30pm, they will receive a notification to tell them that the order has been changed to due ASAP instead of their scheduled time, 7:00pm.

## Horario de servicio personalizado

Cada servicio puede tener su propio horario de funcionamiento independiente. Establecer un horario de atención personalizado para un servicio en particular anulará el horario de atención establecido para la ubicación de su tienda.

## Tiempos de espera estimados y estados automáticos

Para ayudarlo a administrar mejor sus pedidos y las expectativas de los clientes, brindamos una forma simplificada de calcular los tiempos de espera de los pedidos y actualizar automáticamente los estados. Hay 6 estados de pedido:

* Sin Confirmar&#x20;
* Confirmado&#x20;
* Listo&#x20;
* En ruta (solo entrega)&#x20;
* Completo&#x20;
* Cancelado

Tanto los tiempos de espera estimados como las actualizaciones de estado automáticas están conectados a la misma configuración de tiempo. Esto es para que sus actualizaciones de estado y tiempos de espera estén sincronizados entre sí. Esto evita cualquier confusión del cliente. Estas configuraciones de tiempo son:

| Ajuste (minutos)                          | Desde el Estado | Al estado  |
| ----------------------------------------- | --------------- | ---------- |
| Tiempo hasta confirmar                    | Sin Confirmar   | Confirmado |
| Tiempo hasta que esté listo               | Confirmado      | Listo      |
| Tiempo hasta estar en ruta (solo entrega) | Listo           | En Ruta    |
| Tiempo hasta que esté completado          | Listo           | Completado |

{% hint style="info" %}
* El tiempo hasta la confirmación es el tiempo entre el momento en que se realiza un pedido y el momento en que se confirma. Establecer el tiempo hasta la confirmación en "0" dará como resultado una confirmación instantánea del pedido. También deberá habilitar el estado automático para el estado confirmado.
* El tiempo hasta que esté listo es el tiempo que le lleva preparar un pedido después de su confirmación.
* El tiempo hasta el estado en ruta es efectivamente el tiempo entre el momento en que se prepara un pedido y el momento en que el conductor de entrega lo toma.
* El tiempo hasta que se complete es útil para marcar automáticamente los pedidos como completos.
{% endhint %}

### Tiempos de espera estimados

Como se indicó, los tiempos de espera de los clientes se calculan utilizando la configuración de tiempo anterior.

**Cómo se calcula el tiempo de espera estimado para pedidos para recoger o cenar en el restaurante.**

Para pedidos para recoger y cenar, el tiempo de espera estimado se calcula comprando sumando el **tiempo hasta la confirmación** con los valores de **tiempo hasta que esté listo**. Entonces, por ejemplo, si su **tiempo hasta la confirmación** fue 5 y su **tiempo hasta que esté listo** fue 20, el cliente obtendría un tiempo de espera estimado de 20 + 5 = 25 minutos.

Si no ha agregado un valor para el tiempo hasta la confirmación o el tiempo hasta que esté listo, no se calculará el tiempo de espera estimado.

**Cómo se calcula el tiempo de espera estimado para los pedidos de entrega.**

For deliveries, the wait time is calculating by adding the **time till confirm** + **time till ready** + **time till on route** together. Then the **driving time** is added onto that. The driving time is determined using an external service that takes into account traffic data. This provides the customer with an extremely accurate wait time for their order to be delivered. Assuming

If you have not added a value for time till confirm or time till ready or time till on route, the delivery time would not be calculated.

### Automated Statuses

Automated statuses change an order's status after a set period of time has passed. This will allow you to do things such as:

* Automatically confirm new orders
* Mark orders as ready after a period of time
* Mark orders as complete after a period of time

This is very helpful if you know your business timings well and don't want to manually be updating order statuses. Auto status updates can also be enabled or disabled on a per status basis. This way you can provide estimated wait times without auto-updating statuses. Or you can just instantly confirm orders and handle the rest manually.

For automated status updates to work, you will need to enable it for a particular status and ensure the timing settings are added to that particular status.

#### How automated statuses work

Status updates are dependent on your timing settings, the type of order and the order due time. It's best explained through a series of examples.

For the examples, we will assume our timing settings are as follows

* Time till confirm - 10 minutes
* Time till ready - 10 minutes
* Time till on route - 10 minutes
* Time till complete - 60 minutes

#### Pickup and dine-in examples

If a customer places an order at 7:00pm for pickup or dine in which is due immediately

| Time   | Action                                                                                                                                     |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------ |
| 7:00pm | Order has been placed, status unconfirmed                                                                                                  |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes                                                                        |
| 7:20pm | Status updated to ready because time till ready is 10 minutes. This would also be the estimated order ready time as shown to the customer. |
| 8:20pm | Status updated to complete because time till complete is 60 minutes                                                                        |

In the event that you added an extra 10 minutes onto the customers estimated order ready time, it will play out as follows:

| Time   | Action                                                                                                                  |
| ------ | ----------------------------------------------------------------------------------------------------------------------- |
| 7:00pm | Order has been placed, status unconfirmed, you add 10 minutes to estimated ready time                                   |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes                                                     |
| 7:30pm | Status updated to ready because the old ready time was 7:20pm, since you added an extra 10 minutes, that becomes 7:30pm |
| 8:30pm | Status updated to complete because time till complete is 60 minutes                                                     |

If we are unable to calculate an estimated ready time for the order, for example if the time till confirm was missing, it would play out as follows

| Time   | Action                                                              |
| ------ | ------------------------------------------------------------------- |
| 7:00pm | Order has been placed, status unconfirmed                           |
| 7:05pm | You manually update the order status to confirmed                   |
| 7:15pm | Status updated to ready, because the time till ready is 10 minutes  |
| 8:15pm | Status updated to complete because time till complete is 60 minutes |

If a customer places an order at 6:00pm for pickup or dine in which is due at 7:00pm, the following would occur

| Time   | Action                                                                             |
| ------ | ---------------------------------------------------------------------------------- |
| 6:00pm | Order has been placed, status unconfirmed                                          |
| 6:10pm | Status updated to confirmed because time till confirm is 10 minutes                |
| 7:00pm | Status updated to ready, because this is when the customer scheduled the order for |
| 8:00pm | Status updated to complete because time till complete is 60 minutes                |

#### Delivery examples

For the delivery examples, we will assume the driving time between your store and the delivery address is calculated as 10 minutes.

If a customer places a delivery order at 7:00pm which is due immediately

| Time   | Action                                                                                                                         |
| ------ | ------------------------------------------------------------------------------------------------------------------------------ |
| 7:00pm | Order has been placed, status unconfirmed                                                                                      |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes                                                            |
| 7:20pm | Status updated to ready because time till ready is 10 minutes                                                                  |
| 7:30pm | Status updated to on route because time till on route is 10 minutes. This would also be shown to you as the driver pickup time |
| 7:40pm | Order will have been delivered to customer since the driving time is 10 minutes                                                |
| 8:40pm | Order marked as completed because time till complete is 60 minutes                                                             |

If we were unable to calculate the estimated delivery time and driver pickup time, say if the time till on route was missing, the following would occur

| Time   | Action                                                                          |
| ------ | ------------------------------------------------------------------------------- |
| 7:00pm | Order has been placed, status unconfirmed                                       |
| 7:10pm | Status updated to confirmed because time till confirm is 10 minutes             |
| 7:20pm | Status updated to ready because time till ready is 10 minutes                   |
| 7:40pm | You manually mark the order an on route for delivery                            |
| 7:50pm | Order will have been delivered to customer since the driving time is 10 minutes |
| 8:50pm | Order marked as completed because time till complete is 60 minutes              |

If a customer places a delivery order at 6:00pm which is due at 7:00pm, the following would occur

| Time   | Action                                                                                                                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 6:00pm | Order has been placed, status unconfirmed                                                                                                                                                               |
| 6:10pm | Status updated to confirmed because time till confirm is 10 minutes                                                                                                                                     |
| 6:40pm | Status updated to ready because delivery time is 10 minutes and time till on route is 10 minutes, which means that the order must be ready by this time if it is going to reach your customer at 7:00pm |
| 6:50pm | Status updated to on route because the delivery time is 10 minutes, so it has to leave your store at this time. This is also the estimated driver pickup time.                                          |
| 7:00pm | Order will have been delivered to customer                                                                                                                                                              |
| 8:00pm | Order marked as completed because time till complete is 60 minutes                                                                                                                                      |

If a delivery order is scheduled for a later time but the estimated delivery time could not be calculated, then the ready and on route status will not update automatically.

{% hint style="info" %}
If ever in doubt about how the auto status timings will work for your scenario, just think about how it would logically work in a way that makes sense to your customer and you. That is how we have designed it to work.
{% endhint %}
