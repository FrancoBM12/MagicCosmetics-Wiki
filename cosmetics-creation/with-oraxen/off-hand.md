---
description: You know how to create a off hand in the oraxen way.
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
      oraxen: 'magic_offhand' #off_hand item id
      lore:
        - ''
        - '&6Its very Magic!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: -1 #model data is not required here.
    colored: true
    type: WALKING_STICK
    overlaps: true #If this option is enabled, you can have your off hand item and off hand cosmetic equipped at the same time.
```
{% endcode %}
