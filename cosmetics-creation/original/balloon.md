---
description: Here you will learn how to create a balloon in the original form.
---

# Balloon

Balloons are a bit tricky but not as complicated as backpacks.\
Let's start with a balloon without support from other plugins:

* Cosmetic file:

{% code lineNumbers="true" %}
```yaml
cosmetics:
  balloon:
    permission: 'cosmetics.balloon'
    item:
      display: '&bHot air balloon'
      material: LEATHER_HORSE_ARMOR #balloon item
      lore:
        - ''
        - '&aThis balloon will fly through the skies!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: 10000 #balloon model data
    colored: true
    type: BALLOON
    space: 1 #here you can increase/decrease the height of the balloon
    big-head: false #This option changes the position of the balloon item from the head to the right hand.
    distance: 100 #distance to where the players can see the cosmetic.
    invisible-leash: false #If this option is active the balloon string will not be visible.
    instant-follow: true #The balloon will follow you faster and almost instantaneously.
    rotation: #If you are not going to use this, you can delete the path
      enabled: false #select whether this globe will be able to rotate.
      type: RIGHT #RIGHT, UP, ALL(it's a crazy rotation.)
```
{% endcode %}

* BlockBench file of balloon:

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption><p>Display mode - Transition Y Position</p></figcaption></figure>

Now let's create a backpack with the ModelEngine implementation:

```yaml
cosmetics:
  balloon:
    permission: 'cosmetics.balloon'
    item:
      display: '&bHot air balloon'
      material: LEATHER_HORSE_ARMOR #balloon item
      lore:
        - ''
        - '&aThis balloon will fly through the skies!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: 10000 #balloon model data
    colored: true
    type: BALLOON
    meg: #The model id of the Model Engine plugin. Attention: This will only be seen while you have the balloon equipped, that is, it will not replace the item nor will it be seen in the gui!
      model: custom-model
      colorable-parts: #this is optional if you want all parts of the model to be painted remove this path
        - 'partid1'
        - 'partid2'
      animations: #this path is optional, if you do not set anything it will default to "walk" and "idle". 
        walk: animation-walk
        idle: animation-idle
```

and that's it.

Finally, let's create a dongle with the ItemsAdder custom entities implementation:

```yaml
cosmetics:
  balloon:
    permission: 'cosmetics.balloon'
    item:
      display: '&bHot air balloon'
      material: LEATHER_HORSE_ARMOR #balloon item
      lore:
        - ''
        - '&aThis balloon will fly through the skies!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: 10000 #balloon model data
    colored: true
    type: BALLOON
    ia: #The model id of the ItemsAdder plugin. Attention: This will only be seen while you have the balloon equipped, that is, it will not replace the item nor will it be seen in the gui!
      model: namespace:custom-model
      colorable-parts: #It is not yet ready for ItemsAdder entities - this is optional if you want all parts of the model to be painted remove this path
        - 'partid1'
        - 'partid2'
      animations: #this path is optional, if you do not set anything it will default to "walk" and "idle". 
        walk: animation-walk
        idle: animation-idle
```
