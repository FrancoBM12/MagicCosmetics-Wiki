---
description: You know how to create a hat in the oraxen way.
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
      oraxen: 'mex_hat' #hat item id
      lore:
        - ''
        - '&6Its very Mexican!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: -1 #model data is not required here.
    colored: true
    type: HAT
    overlaps: true #If this option is enabled, you can have your helmet and hat equipped at the same time.
```
{% endcode %}
