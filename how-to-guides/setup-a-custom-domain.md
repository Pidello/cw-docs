---
description: >-
  Aprenda cómo conectar su propio nombre de dominio personalizado a su tienda en
  línea para una mejor marca y SEO
---

# Configurar un dominio personalizado

## Proceso de configuración

1. En el panel del restaurante, consulte "Configuración > Sitio web > Dominios > Dominio personalizado".
2. Ingrese su nombre de dominio y presione guardar
3. Vaya al panel de administración de su dominio donde registró su dominio.&#x20;
4. Acceda a sus registros DNS y agregue los registros DNS que se enumeran a continuación&#x20;
5. Después de agregar los registros DNS, espere 10 minutos para que surta efecto&#x20;
6. Luego presione el botón "Generar certificado SSL" en la configuración de su dominio personalizado.

Si su configuración de DNS ha entrado en vigor, indicará que el certificado SSL se ha generado correctamente. Una vez generado, se podrá acceder a su sitio con su nombre de dominio personalizado. Si no puede generar el certificado, espere más tiempo para que la configuración de DNS surta efecto.

## Registro DNS para agregar

| Tipo de Registro | Host                          | Value         |
| ---------------- | ----------------------------- | ------------- |
| A Record         | www / ordena / Cualquier cosa | 35.238.2 .132 |

{% hint style="info" %}
El valor del host es el subdominio de su dominio que su cliente deberá visitar para acceder al sitio. Si el valor del host es "pedido" y su dominio es "negocio.com", entonces la URL de su tienda será "pedido.negocio.com".
{% endhint %}

{% hint style="warning" %}
Si utiliza "www" como valor de host, agregue también el siguiente registro
{% endhint %}

| Tipo de Registro | Host       | Value         |
| ---------------- | ---------- | ------------- |
| A Record         | @ / Blanco | 35.238.2 .132 |

Configurar esto garantizará que si alguien escribe su dominio raíz, es decir, ejemplo.com, será redirigido a www.ejemplo.com.
