# Manual de configuración de Uber Direct

## **Requiremientos**

Para habilitar las entregas de Uber, el restaurante debe tener todo lo siguiente:

* Stripe Connect
* Restaurante de los siguientes países:
  * Australia
  * New Zealand

## Habilitando Uber

Uber DaaS es una forma confiable y conveniente de recibir tu comida de manera rápida y eficiente. Aquí se explica cómo habilitarlo:

1. En el Panel de administración, haga clic en Configuración > Integraciones, busque la tarjeta Uber Delivery Management y haga clic en ella.

<figure><img src="../.gitbook/assets/Screen Shot 2023-05-10 at 9.52.37 AM.png" alt=""><figcaption></figcaption></figure>

2. Se abrirá una ventana emergente y completará la información. Clic en Guardar.

<figure><img src="../.gitbook/assets/Screen Shot 2023-05-10 at 9.56.08 AM.png" alt=""><figcaption></figcaption></figure>

3. Establecer Uber como entrega predeterminada

Una vez que haya habilitado Uber DaaS, puede seleccionar el Proveedor de entrega predeterminado en Configuración > Servicios > Entregas (como se muestra en la imagen a continuación).

<figure><img src="../.gitbook/assets/Screen Shot 2023-05-10 at 9.47.12 AM.png" alt=""><figcaption></figcaption></figure>

### Notas:

* Asegúrese de que su fuente de datos de mapas sea Google Maps. Vaya a Configuración > Sistema > Ubicación > Fuente de datos del mapa.

<figure><img src="../.gitbook/assets/Uber Screenshot 2023-05-09 at 6.38.47 PM.png" alt=""><figcaption></figcaption></figure>

* La moneda debe coincidir con la ubicación del país y la disponibilidad del país de Uber. Vaya a Configuración > Sistema > General > Moneda.

<figure><img src="../.gitbook/assets/Uber Screenshot 2023-05-09 at 6.41.14 PM.png" alt=""><figcaption></figcaption></figure>

* Uber requiere un número de teléfono válido de su tienda (debe tener el código del país). Vaya a Configuración > Sistema > Ubicación > Número de teléfono.

<figure><img src="../.gitbook/assets/Uber Screenshot 2023-05-09 at 6.43.23 PM.png" alt=""><figcaption></figcaption></figure>

## Detalles de pago

Una vez que un cliente realiza un pedido, Uber (si está configurado como proveedor de entrega predeterminado en el Panel de administración) se mostrará como proveedor de entrega.

<figure><img src="../.gitbook/assets/Screenshot 2023-05-09 at 7.06.03 PM.png" alt=""><figcaption></figcaption></figure>

**La estimación de entrega proporcionará:**

**Proveedor de entrega:** que es Uber

**Tarifa estimada:** la tarifa total

**Propinas:** ingresadas por el usuario y se enviarán directamente al conductor de Uber

**Tiempo estimado de entrega:** tiempo desde ahora hasta la entrega

**El Método de Pago aceptable será el siguiente:**

**Tarjeta de crédito:** si está habilitada y se proporciona el ID de cuenta de Stripe Connect

**Pago de Apple | Google Pay (Stripe) -** si está habilitado

## Flujo de trabajo de pedidos

Una vez que el cliente realizó el pedido, en el Panel de administración, la miniatura del pedido se reemplazará por el logotipo de Uber (lo que indica que utilizará Uber).

#### Orden: SIN CONFIRMAR

<figure><img src="../.gitbook/assets/Screenshot 2023-05-09 at 7.44.43 PM.png" alt=""><figcaption></figcaption></figure>

#### Orden: CONFIRMADO

El pedido **DEBE** pasar al estado **CONFIRMADO** para activar la solicitud de entrega de Uber.

Una vez que el pedido esté configurado como CONFIRMADO, la URL de seguimiento de entrega estará disponible tanto en el ADMIN como en el CLIENTE.

<figure><img src="../.gitbook/assets/Untitled (7).png" alt=""><figcaption><p>Vista de orden de administrador</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Untitled (4).png" alt=""><figcaption><p>Vista de pedido del cliente</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Untitled (5).png" alt=""><figcaption><p>Captura de pantalla de muestra de la URL de seguimiento</p></figcaption></figure>

<figure><img src="../.gitbook/assets/Untitled (6).png" alt=""><figcaption><p>SMS enviado por Uber al destinatario.</p></figcaption></figure>

#### Orden: LISTO

<figure><img src="../.gitbook/assets/Untitled (9).png" alt=""><figcaption><p>Customer Order View</p></figcaption></figure>

Se espera que el conductor todavía esté en camino al restaurante o esté esperando en el restaurante.

#### Orden: EN RUTA

<figure><img src="../.gitbook/assets/Untitled (10).png" alt=""><figcaption><p>Admin Order View</p></figcaption></figure>

#### Orden: CANCELADA

Si el Pedido se cancela (iniciado por el cliente o la tienda), la entrega Uber también se cancelará automáticamente.
