---
description: >-
  Cómo configurar su clave API. Esto se utiliza para conectar su configuración
  de impresión en línea a su aplicación PushPrinter y a su impresora de recibos.
---

# Impresión - Clave API

1. Inicie sesión en su cuenta de Pidello en admin.pidello.com y vaya a Configuración>Sistema>Impresión de recibos>Crear impresora.

![](../../.gitbook/assets/1-create-printer.png)

2. Asigne un nombre a la impresora, idealmente use el mismo nombre que la configuración en PushPrinter para evitar confusiones. También recomendamos activar "Pedidos de impresión automática" y "Reservas de impresión automática".

![](<../../.gitbook/assets/untitled (2).png>)

3\. Ahora seleccione 'Configuración de la impresora' y asegúrese de que:

* 'Método de impresión' - está configurado en ESCPOS
* 'Tipo de impresión ESCPOS': está configurado en 'Imagen ESCPOS'.

{% hint style="warning" %}
**NOTA** - En el caso de que su impresora no admita la impresora de imágenes (no imprime correctamente o imprime muy lentamente), cambie esto a 'Solo texto ESCPOS'.
{% endhint %}

![](<../../.gitbook/assets/untitled-1 (2).png>)

4. Desplácese hasta la parte inferior de la pantalla y presione el botón "Guardar".
5. Luego resalte la clave API > haga clic derecho > copiar al portapapeles.

![](<../../.gitbook/assets/untitled-2 (3).png>)

6\. Pegue la clave API en el campo API correspondiente en PushPrinter.
