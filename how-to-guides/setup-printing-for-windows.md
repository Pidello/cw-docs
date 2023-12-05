---
description: >-
  Aprenda a instalar y configurar la impresión de pedidos para dispositivos
  Windows con nuestro software de impresión
---

# Setup Printing For Windows

Nuestro sistema le permite imprimir manualmente y automáticamente nuevos pedidos. Esta guía le mostrará cómo configurar la impresión de pedidos y solucionar problemas.

|| Estaremos encantados de configurar su impresora de forma remota. Sabemos que este es un paso que puede hacer tropezar a muchas personas debido a que cada impresora es un poco diferente. Por favor póngase en contacto con nosotros si necesita ayuda

Para obtener instrucciones paso a paso según el método de impresión. Utilice las siguientes instrucciones. Vale la pena señalar que, para la mayoría de situaciones, recomendamos utilizar el método de Impresión compartida de Windows;

{% content-ref url="understanding-printing/printing-api-key.md" %}
[printing-api-key.md](understanding-printing/printing-api-key.md)
{% endcontent-ref %}

{% content-ref url="understanding-printing/printing-windows-shared-printing.md" %}
[printing-windows-shared-printing.md](understanding-printing/printing-windows-shared-printing.md)
{% endcontent-ref %}

{% content-ref url="understanding-printing/printing-windows-network-printing.md" %}
[printing-windows-network-printing.md](understanding-printing/printing-windows-network-printing.md)
{% endcontent-ref %}

## Requerimientos

* Windows 7/8/10 ya sea de 32 o 64 bits
* Una impresora compatible con Windows con los controladores instalados
* Última versión de PushPrinter que se puede descargar [aquí](https://pushprinter.com/)

## Proceso de configuración

### Verifique que los controladores de la impresora estén instalados y funcionando

1. Si sus controladores se instalaron correctamente, su impresora se mostrará en su PC en "Panel de control > Hardware y sonido > Dispositivos e impresoras".&#x20;
2. Haga clic derecho en su impresora y seleccione "Propiedades"
3. En la parte inferior izquierda, presione "Imprimir página de prueba".
4. Verifique que la página de prueba se imprimió correctamente

Si esto tiene éxito, su impresora funcionará bien. Si no puede encontrar su impresora o no funciona, reinstale el controlador nuevamente.

### Tome nota de los tamaños de papel disponible

Este paso es ligeramente diferente para todas las impresoras. Algunas impresoras proporcionan su propia herramienta de configuración donde puede ver los tamaños de papel disponibles.

De forma predeterminada, puede encontrar esta información en el cuadro de diálogo "Propiedades" de su impresora, como se describe en el paso anterior. A veces, esto se encuentra en la pestaña "Configuración del dispositivo" en las propiedades de su impresora.

Otras veces puede seleccionar "Preferencias" en la parte inferior de la ventana emergente de propiedades de la impresora y luego seleccionar "Avanzado" en la parte inferior nuevamente.

Consulte la imagen a continuación para ver cómo se vería.

![Printer paper size settings](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_1vcnqy8.png)

Tome nota de los tamaños de papel disponibles, ya que probablemente tendrá que probar algunos para que funcione perfectamente.

### Crear una configuración de impresora

1. Visite el panel de control de su restaurante y navegue hasta "Configuración > Impresión de recibos".
2. Presione el botón "Nueva impresora" y complete las opciones necesarias
3. En la pestaña "Configuración del papel", configure el ancho y el alto del papel de acuerdo con el tamaño de papel más grande disponible para su impresora, como se indicó en el paso anterior. Saliendo de la imagen de arriba, ingresaríamos un ancho de "72" y un alto de "210".&#x20;
4. Recomendamos encarecidamente comenzar con un tamaño de fuente de "18" y un margen de papel de "0".&#x20;
5. Cree la configuración de impresión. Después de crearlo, obtendrá una clave API única para conectarse a él. Mantenga esta pantalla abierta ya que pronto necesitará copiar su clave API

![Printer API key](https://storage.crisp.chat/users/helpdesk/website/e903fdb8557a9800/image\_bnxer6.png)

|| Los tamaños de papel ingresados en la configuración de su impresora deben coincidir con la configuración de tamaño de papel de Windows tal como se establece en las opciones del controlador de la impresora. Si la impresión es incorrecta o está torcida, deberá probar los otros tamaños, desde el más grande al más pequeño. Al cambiar los tamaños en la configuración de la impresora, asegúrese de cambiarlo en la configuración del controlador de impresora de Windows.

### Instalar PushPrinter

1. Descarga PushPrinter desde el siguiente enlace&#x20;
2. Ejecute el instalador, recibirá una advertencia de que la aplicación no está verificada, continúe con la instalación&#x20;
3. Después de que se haya instalado correctamente, PushPrinter se abrirá automáticamente

### Configure PushPrinter

1. Lo primero que probablemente querrá hacer es alternar el interruptor de "Inicio automático" para que se conecte y se inicie cuando se inicie su PC. Actívelo seleccionando el "Engranaje de configuración" y marcando el botón "Iniciar automáticamente PushPrinter" (imagen 1.1).
2. Presione la pestaña "Icono de impresora" en la parte superior para configurar un servicio de impresión.&#x20;
3. Presione el botón "Crear impresora" (imagen 1.2).&#x20;
4. Copie y pegue la clave API para la impresora que creó hace 2 pasos&#x20;
5. Establezca el número de copias a imprimir y seleccione su impresora&#x20;
6. Presione el botón de inicio y asegúrese de que diga conectado en la parte inferior

![Imagen 1.1 - Botón 'Iniciar PushPrinter automáticamente'](../.gitbook/assets/pushprinter-settings.png)

![Imagen 1.2 - 'Crear impresora'](../.gitbook/assets/create-printer-pushprinter.png)

### Prueba de impresión

Visita tu página de pedidos. Seleccione un pedido, debajo de la barra de selección de acción, seleccione imprimir. Recomendamos imprimir pedidos cortos y largos para garantizar que no se corte nada verticalmente. Si ha habilitado la impresión automática para esta configuración de impresión, realice un pedido y pruebe la impresión automática.

## Solución de problemas

#### Contáctanos

Hemos configurado con éxito cientos de impresoras y es muy probable que podamos ahorrarle muchos dolores de cabeza, así que no dude en contactarnos.

#### Lados cortado

Comience reduciendo los valores de margen o ancho del papel en la configuración de su impresora en su panel de administración. Eventualmente calibrarás un ancho y margen adecuados. También puedes ajustar el tamaño de fuente a algo más pequeño. Puede obtener el ancho de papel correcto en la configuración de su impresora de Windows como se ve en la guía anterior.

**El final del recibo no sale completo.**

En la configuración de su impresora de Windows. Configure la opción "Alimentar línea después de imprimir" en un valor alto para permitir que la impresora avance algunas líneas adicionales.

**Clave API no válida**

La clave API que ingresó no se corresponde con ninguna de sus configuraciones de impresión. Verifique su clave API

**No puede autenticarse**

Comprueba tu conexión a Internet o vuelve a intentarlo en breve

**La impresora no se detecta en Windows**

Debe encontrar el controlador correcto para su impresora, siempre que esté disponible para Windows. Intente buscar en Google el nombre de su impresora seguido de las palabras "controlador de Windows {inserte su versión de Windows}"

**La impresión no funciona aunque todo está configurado correctamente**

Asegúrese de que Windows detecte su impresora. Intente reiniciar su impresora o PC. Intente imprimir en su impresora desde otros programas de su PC, como su navegador.
