---
description: You know how to create a spray in the oraxen way.
---

# Spray

A spray is quite simple, in fact it is as simple as hats.

{% code lineNumbers="true" %}
```yaml
cosmetics:
  spray:
    permission: 'cosmetics.spray'
    item:
      display: '&bSpray'
      oraxen: 'spray_item' #spray item id
      lore:
        - ''
        - '&aThis spray is the best!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: -1 #model data is not required here.
    colored: true
    type: SPRAY
    url: 'https://localhost/img_url.png' #here there are 2 options, you put a url of an image or you type the name of an image you have in plugins/MagicCosmetics/sprays/
    item-image: false #This applies to sprays that are items and not images (they do not require the path url). If this option is activated, it will take the item displayed in the menu as an image.
```
{% endcode %}
