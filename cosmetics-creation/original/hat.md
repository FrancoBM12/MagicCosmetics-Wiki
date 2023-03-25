---
description: You know how to create a hat in the original way.
---

# Hat

It's a simple thing to create a hat, something like this should suffice.

{% code lineNumbers="true" %}
```yaml
cosmetics:
  mexican_hat:
    permission: 'cosmetics.mexican_hat'
    item:
      display: '&bMexican Hat'
      material: LEATHER_HORSE_ARMOR #hat item
      lore:
        - ''
        - '&6Its very Mexican!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: 10005 #hat model data
    colored: true
    type: HAT
    overlaps: true #If this option is enabled, you can have your helmet and hat equipped at the same time.
```
{% endcode %}
