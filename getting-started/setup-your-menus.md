---
description: >-
  Para aceptar pedidos en línea, debe configurar su menú en línea. Puede crear y
  administrar todos sus menús en la sección "Menús" en el panel del restaurante.
---

# Configura tu menú

{% embed url="https://youtu.be/Nyyr2vwB1Io" %}
Menu setup video tutorial
{% endembed %}

## Proceso de configuración

Los menús están organizados en una estructura de árbol. Los menús contienen categorías y las categorías contienen platos. El proceso de configuración general es el siguiente.

1. Crear Menú
2. Crear todas las categorías bajo el menú.
3. Crear platillos bajo las categorías.
4. Cree conjuntos de opciones para agregar personalización a los platillos.
5. Cree etiquetas de platillos para resaltar los atributos de platillos particulares.

{% hint style="info" %}
Probablemente solo necesitarás un menú. Múltiples menús son útiles si ciertos elementos están restringidos de manera particular. Es posible que necesites crear un menú de "Desayuno" o un menú de "Entrega" según tus requisitos.
{% endhint %}

## Ejemplo de estructura de Menú

```
- Menú: Menú Principal
-- Categoría: Pizzas
---- Platillo: Jamón y queso
---- Platillo: Margarita
---- Platillo: Vegetariana Suprema
-- Categoría: Complementos
---- Platillo: Alitas
---- Platillo: Papas fritas
-- Categoría: Bebidas
---- Platillo: Té Helado
---- Platillo: Coca Cola
---- Platillo: Agua
```

## Menús

Estos representan sus menús de la vida real. Muchas tiendas tienen un solo menú principal que siempre está disponible. Otros pueden tener un menú de almuerzo y cena o un menú solo para recoger. Necesitarás al menos un menú para que tu tienda online funcione.

La disponibilidad del menú puede depender de ciertas condiciones, como tipos de pedidos (a recoger, entregas a domicilio o consumo en el restaurante), horarios de los pedidos (al momento o solo pedidos programados). También pueden restringirse a determinados días y horarios.

{% hint style="info" %}
Si solo tiene un menú disponible, no es necesario imponerle restricciones. Puede restringir el sistema globalmente a sus reglas comerciales y el menú funcionará de acuerdo con eso. Solo es necesario restringir un menú a ciertas condiciones si tiene varios menús
{% endhint %}

## Categorías

Las categorías representan una subsección de un menú y constan de platos. Por ejemplo, si tiene un menú estándar, sus categorías podrían incluir:

* Entradas
* Principales
* Complementos
* Bebidas
* Postres

{% hint style="info" %}
En algunos casos, es posible que necesites crear un menú independiente en lugar de utilizar una categoría. Por ejemplo, si tiene muchas categorías diferentes de bebidas, como licores, vinos, cervezas, refrescos, etc., es posible que desee crear un menú de bebidas separado para todas esas categorías en lugar de agregarlo a su menú de alimentos.
{% endhint %}

## Dishes

Dishes represent actual items that can be purchased. There are 2 types of dishes.

#### Standard Dishes

A standard dish works as you would expect. You would use it to create items such:

* Ham sandwich
* Veggie pizza
* Vanilla ice-cream

**Dish Ingredients**

Standard dishes can contain a list of ingredients. The purpose of this is to allow customers to easily remove certain ingredients. A customer can remove the desired ingredients when they select the dish.

#### Combo Dishes

Combos are a special type of dish that contain other dishes. It allows you to create a list of choices for customers to select various standard dishes. For example, you can create:

* Choose 3 pizzas, 2 sides and 2 drinks
* Choose a burger, side and drink

To do this you will first need to have created some standard dishes. Then when creating your combo, you can create 4 choices, 3 pizza choices and one drink choice. You can then assign dish choices to the pizzas and drinks for customers to choose from.

{% hint style="info" %}
Combo dishes cannot contain option sets or ingredients directly. Instead when a customer chooses a standard dish within a combo, if the chosen standard dish has any option sets assigned to it, a user can customize it accordingly.
{% endhint %}

#### Dish Availability & Status

There are 3 statuses available for a dish. They are:

* Hidden - hides dish from the menu
* Available - shows dish from the menu and allows ordering
* Out of stock - prevents ordering and shows out of stock on the dish

In the admin dashboard, you can edit the status of a dish by checking the tickbox on the left of it. Then select the desired status from the popup menu.

## Option Sets

All **dish customization is done using option sets**. Option sets are a configurable set of options that can be assigned to any number of dishes. With option sets, you are able to create requirements such as:

* Select your pizza crust
* Select one or more sauces
* Select at least 4 toppings

{% hint style="info" %}
To learn how to create an option set that meets your requirements, read the descriptions of each of the settings available when creating an option set. Each setting is explained in detail. Alternatively, watch our menu setup video above to see us create the above examples.
{% endhint %}

## Dish Tags

Tags allow you to highly particular attributes about a dish with a fully customizable visual indicator. You can create tags for attributes such as:

* Spicy
* Vegan
* Gluten free

## Common Menu Problems

### **No menu or categories showing under the store**

For your menu to display in your online store, make sure to add at least one category and one dish to it.

### **Dish images to large**

We highly recommend that you use the website [https://www.birme.net](https://www.birme.net) or [https://tinypng.com/](https://tinypng.com/) to optimize all your images. Given that the maximum image width is only around 600 pixels, it's best to make sure all your images are no wider than that. This is going to help significantly with your page load time especially for mobile customers.
