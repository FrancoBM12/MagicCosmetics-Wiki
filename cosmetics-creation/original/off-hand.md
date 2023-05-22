---
description: You know how to create a off hand in the original way.
---

# Mano alterna

It is as simple to create an off hand cosmetic as it is to create a hat.\
This is one such example:

{% code lineNumbers="true" %}
```yaml
cosmetics:
  magic_off_hand:
    permission: 'cosmetics.magic_offhand'
    item:
      display: '&bMagic OffHand'
      material: LEATHER_HORSE_ARMOR #off_hand item
      lore:
        - ''
        - '&6Its very Magic!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: 10005 #off_hand model data
    colored: true
    type: WALKING_STICK
    overlaps: true #If this option is enabled, you can have your off hand item and off hand cosmetic equipped at the same time.
```
{% endcode %}
