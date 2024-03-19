---
description: >-
  Los servicios de su restaurante representan los distintos tipos de pedidos que
  acepta. Vea nuestro vídeo para obtener una explicación detallada de todas las
  configuraciones disponibles.
---

# Configura tus Servicios

Actualmente hay 4 servicios disponibles. Ellos son:

* **Recoger en tienda (Pick Up):** pedidos que los clientes recogen en la tienda para llevar&#x20;
* **Entrega a domicilio (Delivery):** pedidos que se entregan en la dirección del cliente.&#x20;
* **Ordena y paga en Restaurante (Dine in):** pedidos realizados por clientes actualmente sentados en su tienda.&#x20;
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

Para las entregas, el tiempo de espera se calcula sumando el **tiempo hasta la confirmación + el tiempo hasta que esté listo + el tiempo hasta que esté en ruta** juntos. Luego se le suma el tiempo de conducción. **El tiempo de conducción** se determina mediante un servicio externo que tiene en cuenta los datos del tráfico. Esto proporciona al cliente un tiempo de espera extremadamente preciso para que se entregue su pedido.&#x20;

Si no ha agregado un valor para el tiempo hasta la confirmación o el tiempo hasta que esté listo o el tiempo hasta en ruta, el tiempo de entrega no se calculará.

### Estatus automáticos

Los estados automatizados cambian el estado de un pedido después de que haya transcurrido un período de tiempo determinado. Esto le permitirá hacer cosas como:

* Confirmar automáticamente nuevos pedidos&#x20;
* Marcar pedidos como listos después de un período de tiempo
* Marcar pedidos como completos después de un período de tiempo

Esto es muy útil si conoce bien los horarios de su negocio y no desea actualizar manualmente los estados de los pedidos. Las actualizaciones automáticas de estado también se pueden habilitar o deshabilitar según el estado. De esta manera, puede proporcionar tiempos de espera estimados sin actualizar automáticamente los estados. O simplemente puede confirmar los pedidos al instante y gestionar el resto manualmente.

Para que funcionen las actualizaciones de estado automáticas, deberá habilitarlas para un estado en particular y asegurarse de que la configuración de tiempo se agregue a ese estado en particular.

**Cómo funcionan los estados automatizados**

Las actualizaciones de estado dependen de su configuración de tiempo, el tipo de pedido y la hora de vencimiento del pedido. Se explica mejor a través de una serie de ejemplos.&#x20;

Para los ejemplos, asumiremos que nuestra configuración de tiempo es la siguiente

* Tiempo hasta confirmar - 10 minutos
* Tiempo hasta que esté listo - 10 minutos
* Tiempo hasta estar en ruta - 10 minutos
* Tiempo hasta que esté completo - 60 minutos

#### Ejemplos de 'Pick up' y 'Dine in'

Si un cliente realiza un pedido a las 7:00 p. m. para recogerlo o cenar en el lugar que vence inmediatamente

| Tiempo | Acción                                                                                                                                                                        |
| ------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 7:00pm | Se ha realizado el pedido, estado no confirmado                                                                                                                               |
| 7:10pm | Estado actualizado a confirmado porque el tiempo hasta la confirmación es de 10 minutos                                                                                       |
| 7:20pm | Estado actualizado a listo porque el tiempo hasta que esté listo es de 10 minutos. Este también sería el tiempo estimado de preparación del pedido que se muestra al cliente. |
| 8:20pm | Estado actualizado para completar porque el tiempo hasta completar es 60 minutos                                                                                              |

En el caso de que haya agregado 10 minutos adicionales al tiempo estimado de preparación del pedido del cliente, se desarrollará de la siguiente manera:

| Tiempo | Acción                                                                                                                                                       |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 7:00pm | Se realizó el pedido, estado no confirmado, agrega 10 minutos al tiempo estimado de preparación                                                              |
| 7:10pm | Estado actualizado a confirmado porque el tiempo hasta la confirmación es de 10 minutos                                                                      |
| 7:30pm | El estado se actualizó a Listo porque la hora anterior de preparación eran las 7:20 pm, como agregaste 10 minutos adicionales, se convierten en las 7:30 pm. |
| 8:30pm | Estado actualizado para completar porque el tiempo hasta completar es 60 minutos                                                                             |

Si no podemos calcular un tiempo estimado de preparación para el pedido, por ejemplo, si falta el tiempo hasta la confirmación, se desarrollará de la siguiente manera:

| Tiempo | Acción                                                                             |
| ------ | ---------------------------------------------------------------------------------- |
| 7:00pm | Se ha realizado el pedido, estado no confirmado                                    |
| 7:05pm | Actualizas manualmente el estado del pedido a confirmado                           |
| 7:15pm | Estado actualizado a listo, porque el tiempo hasta que esté listo es de 10 minutos |
| 8:15pm | Estado actualizado para completar porque el tiempo hasta completar es 60 minutos   |

Si un cliente realiza un pedido a las 6:00 pm para recogerlo o cenar y debe entregarse a las 7:00 pm, ocurriría lo siguiente

| Tiempo | Acción                                                                                    |
| ------ | ----------------------------------------------------------------------------------------- |
| 6:00pm | Se ha realizado el pedido, estado no confirmado                                           |
| 6:10pm | Estado actualizado a confirmado porque el tiempo hasta la confirmación es de 10 minutos   |
| 7:00pm | Estado actualizado a listo, porque fue entonces cuando el cliente programó el pedido para |
| 8:00pm | Status updated to complete because time till complete is 60 minutes                       |

#### Ejemplos de Delivery

Para los ejemplos de entrega, asumiremos que el tiempo de conducción entre su tienda y la dirección de entrega se calcula en 10 minutos.

Si un cliente realiza un pedido de entrega a las 7:00 pm que vence inmediatamente

| Tiempo | Acción                                                                                                                                                  |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 7:00pm | Se ha realizado el pedido, estado no confirmado                                                                                                         |
| 7:10pm | Estado actualizado a confirmado porque el tiempo hasta la confirmación es de 10 minutos                                                                 |
| 7:20pm | Estado actualizado a listo porque el tiempo hasta que esté listo es de 10 minutos                                                                       |
| 7:30pm | Estado actualizado a en ruta porque el tiempo hasta estar en ruta es de 10 minutos. Esto también se le mostrará como la hora de recogida del conductor. |
| 7:40pm | El pedido se habrá entregado al cliente ya que el tiempo de conducción es de 10 minutos.                                                                |
| 8:40pm | Pedido marcado como completado porque el tiempo hasta completarlo es de 60 minutos                                                                      |

Si no pudiéramos calcular el tiempo estimado de entrega y el tiempo de recogida del conductor, digamos si faltara el tiempo hasta la ruta, ocurriría lo siguiente:

| Tiempo | Acción                                                                                   |
| ------ | ---------------------------------------------------------------------------------------- |
| 7:00pm | Se ha realizado el pedido, estado no confirmado                                          |
| 7:10pm | Estado actualizado a confirmado porque el tiempo hasta la confirmación es de 10 minutos  |
| 7:20pm | Estado actualizado a listo porque el tiempo hasta que esté listo es de 10 minutos        |
| 7:40pm | Usted marca manualmente el pedido como en ruta para la entrega.                          |
| 7:50pm | El pedido se habrá entregado al cliente ya que el tiempo de conducción es de 10 minutos. |
| 8:50pm | Pedido marcado como completado porque el tiempo hasta completarlo es de 60 minutos       |

Si un cliente realiza un pedido de entrega a las 6:00 pm que vence a las 7:00 pm, ocurriría lo siguiente:

| Tiempo | Acción                                                                                                                                                                                                                               |
| ------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 6:00pm | Se ha realizado el pedido, estado no confirmado                                                                                                                                                                                      |
| 6:10pm | Estado actualizado a confirmado porque el tiempo hasta la confirmación es de 10 minutos                                                                                                                                              |
| 6:40pm | Estado actualizado a listo porque el tiempo de entrega es de 10 minutos y el tiempo hasta que esté en ruta es de 10 minutos, lo que significa que el pedido debe estar listo a esta hora si va a llegar a su cliente a las 7:00 p.m. |
| 6:50pm | Estado actualizado a en ruta porque el tiempo de entrega es de 10 minutos, por lo que tiene que salir de tu tienda en este momento. Este es también el tiempo estimado de recogida del conductor.                                    |
| 7:00pm | El pedido habrá sido entregado al cliente.                                                                                                                                                                                           |
| 8:00pm | Pedido marcado como completado porque el tiempo hasta completarlo es de 60 minutos                                                                                                                                                   |

Si un pedido de entrega está programado para un momento posterior pero no se pudo calcular el tiempo de entrega estimado, entonces el estado listo y en ruta no se actualizará automáticamente.

{% hint style="info" %}
Si alguna vez tiene dudas sobre cómo funcionarán los tiempos de estado automático para su escenario, simplemente piense en cómo funcionaría lógicamente de una manera que tenga sentido para su cliente y para usted. Así es como lo hemos diseñado para que funcione.
{% endhint %}
