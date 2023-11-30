---
description: >-
  Aprenda a instalar y configurar la impresión de pedidos para dispositivos
  Android con nuestro software de impresión
---

# Configurar la impresión para Android

Nuestro sistema le permite imprimir manualmente y automáticamente nuevos pedidos. Esta guía le mostrará cómo configurar la impresión de pedidos y solucionar problemas.&#x20;

|| Estaremos encantados de configurar su impresora de forma remota. Sabemos que este es un paso que puede hacer tropezar a muchas personas debido a que cada impresora es un poco diferente. Póngase en contacto con nosotros si necesita ayuda.

## Requerimientos

* Un dispositivo Android con Android 1.4 o superior
* Una impresora compatible con ESC/POS
* Última versión de PushPrinter que se puede descargar [aquí.](https://pushprinter.com/)

## Proceso de Configuración

### Crear una configuración de impresora

1.  Visite el panel de su restaurante y navegue hasta "Configuración > Impresión de recibos > Crear impresora"\\

    <figure><img src="../../.gitbook/assets/image (1) (2).png" alt=""><figcaption></figcaption></figure>
2. Complete lo siguiente:
   * Nombre de la impresora
   * Vaya a Configuración de la impresora y asegúrese de que el Método de impresión sea "ESCPOS" y el Tipo de impresión sea Imagen ESCPOS. (Tenga en cuenta que es posible que algunas impresoras más antiguas no admitan este método y en estos casos se puede utilizar ESCPOS Text Only.
   * La configuración de papel predeterminada funciona para la mayoría de las impresoras. Si la impresión de prueba corta el borde del texto, ajuste el factor de escala del papel a 1,7 y vuelva a realizar la prueba.

![Printer Settings for Android](../../.gitbook/assets/printer-settings.png)

3\. Una vez realizada toda la configuración de la impresora, haga clic en "Guardar".

4\. Después de crearlo, obtendrá una clave API única para conectarse a él. Mantenga esta pantalla abierta ya que pronto necesitará copiar su clave API.

![](<../../.gitbook/assets/image (6).png>)

### Instalar la impresora 'PushPrinter'

1. Descargue PushPrinter desde Playstore, o haga clic en este [link](https://www.pushprinter.com)
2. Después de que se haya instalado correctamente, PushPrinter se abrirá automáticamente

### Configure la impresora 'PushPrinter'

1. Presione el "Engranaje de configuración" y seleccione Predeterminado.

## ![](<../../.gitbook/assets/image (15).png>)

![](<../../.gitbook/assets/image (2) (2).png>)

2\. Presione el signo "+" en la parte superior para configurar un servicio de impresión. Asegúrese de que la impresora esté encendida.

![](../../.gitbook/assets/push3.png)

3\. Empareje el dispositivo Android con la impresora a través de Bluetooth.

![](<../../.gitbook/assets/image (10).png>)

4\. Una vez que se haya conectado correctamente, se enviará una impresión de prueba a la impresora.

<img src="../../.gitbook/assets/image (11).png" alt="" data-size="original">

5\. Complete los detalles de la impresora, como el nombre de la impresora, la clave API y el número de copias.&#x20;

Nota: Si le solicita un código PIN, a menudo es “0000” o “1234”.

![](<../../.gitbook/assets/image (13).png>)

* La API se puede encontrar en la configuración de la impresora del restaurante. (Configuración > Impresión de recibos)
* Asegúrese de que la API sea correcta.

6\. Una vez que se hayan completado todos los detalles, verifique el estado de la impresora en la configuración de su restaurante. Asegúrate de que aparezca como conectado.

![](<../../.gitbook/assets/image (7) (1).png>)

### Impresión de prueba

Visita tu página de pedidos. Seleccione un pedido, debajo de la barra de selección de acción, seleccione imprimir. Recomendamos imprimir pedidos cortos y largos para garantizar que no se corte nada verticalmente. Si ha habilitado la impresión automática para esta configuración de impresión, realice un pedido y pruebe la impresión automática.

![](<../../.gitbook/assets/image (5).png>)

## Solución de problemas

#### Contáctanos

Hemos configurado con éxito cientos de impresoras y es muy probable que podamos ahorrarle muchos dolores de cabeza, así que no dude en contactarnos.

#### Lados Cortados

Comience reduciendo el factor de escala del papel a 1,7 y pruebe la impresión nuevamente. Ajustar hasta que encaje.

#### Clave API Inválida

La clave API que ingresó no se corresponde con ninguna de sus configuraciones de impresión. Verifique su clave API.

#### No puede autenticarse

Comprueba tu conexión a Internet o vuelve a intentarlo en breve.

#### La impresión no funciona aunque todo está configurado correctamente

Asegúrese de que Android detecte su impresora. Intente reiniciar su dispositivo. Intente imprimir en su impresora desde otros programas de su PC, como su navegador.
