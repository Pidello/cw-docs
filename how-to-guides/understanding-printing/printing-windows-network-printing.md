---
description: Cómo guía para imprimir con una impresora de red
---

# Impresión - Impresión en red de Windows

## **Impresión en Red**

1. Vaya al Panel de control de Windows

![](<../../.gitbook/assets/untitled (1).png>)

2\. Abrir dispositivos e impresoras

![](../../.gitbook/assets/untitled-1.png)

3\. Haga clic derecho y seleccione 'Propiedades de la impresora'

![](<../../.gitbook/assets/untitled-2 (5).png>)

4\. Si su impresora no aparece, utilice estas instrucciones para configurarla [Configuración de la impresora.](printing-add-a-printer-to-windows.md)

5\. Para probar que la impresora está funcionando, presione Imprimir página de prueba.

![](<../../.gitbook/assets/untitled-3 (1).png>)

6\. Si la página de prueba no se imprime. Luego conecte e instale la impresora correctamente. Por favor mira: [Configuración de la impresora](https://www.notion.so/cloudwaitresswiki/Printing-Add-a-printer-18689e4654fe4978b20aeb82b581d81e).

7\. Abra la aplicación del programa PushPrinter para Windows.

8\. Vaya al engranaje de 'configuración' y seleccione el perfil de proveedor predeterminado de la lista desplegable.

![](<../../.gitbook/assets/untitled-4 (2).png>)

9\. Habilite 'Iniciar automáticamente PushPrinter'. (Esto permite que la aplicación se inicie automáticamente al reiniciar su máquina).

10\. Presione el botón de la impresora

![](../../.gitbook/assets/untitled-6.png)

11\. Usando el botón Crear Impresora, cree una impresora.

![](<../../.gitbook/assets/untitled-7 (4).png>)

12\. Agregue configuraciones, incluida la clave API de la impresora recién creada.

{% hint style="info" %}
**Para una impresora de red:**

* Nombra la impresora.
* Agregar impresora API (que se encuentra en la configuración de la impresora de la tienda),
* Establecer número de copias
* Agregue la dirección IP de la impresora y configure el puerto en 9100).
{% endhint %}

![](<../../.gitbook/assets/untitled-8 (3).png>)

{% hint style="danger" %}
**NOTE:**

**Printer name** - This is the name that the printer will show inside of CloudWaitress.

**API Key** - This needs to be copied from the printer settings inside of CloudWaitress.

**Number of copies** - This will determine how many copies of the are printed.

**Printing type** - This needs to be set to Windows Shared Printer (ESCPOS) for this to work.

**Windows Share Printer Name** - This must match EXACTLY the shared printer name that was added before. You should avoid spaces and special characters.
{% endhint %}

13\. Test print

14\. Create printer

15\. Go to your store and place a test order.
