---
description: Here you will find the guide to create a cosmetic of any kind.
---

# Cosmetics creation

Here you can find out how to create a cosmetic\
Either without any plugin that supports modified items\
or on the contrary, know how to create cosmetics with this type of plugins such as ItemsAdder or Oraxen.

Different types of cosmetics have unique options that are not shared. This time I will show you the options that are shared by all cosmetics.

```yaml
cosmetics:
  test_balloon: #this will be the id of the cosmetic
    permission: 'cosmetics.test_balloon' #to use the permission, you must have the permissions option enabled in the config.
    item:
      display: '&btest balloon' #name that the cosmetic item will have
      texture: 'here' #in case your item is a head, you can choose the texture of the head with this path!
      material: LEATHER_HORSE_ARMOR #cosmetic material if you use ItemsAdder you can delete this path
      #if you use the ItemsAdder or Oraxen plugin you can just put the name of your item here and it will suffice
      item-adder: balloon #optional
      oraxen: balloon #optional
      lore: #lore of the item if you don't want it to have a lore you can delete the path
      - ''
      - '&cfirst'
      - ''
      unbreakable: true #select if the item will be unbreakable!
      glow: true #selects whether the item will have a glow effect.
      hide-attributes: true #select if the item will hide the attributes.
      modeldata: 10030 #here goes the model data of the item if the item is from the ItemsAdder or Oraxen plugin it will skip this.
      color: '#004F71' #Set the default color of the cosmetic (in case you want one).
    colored: false #select if the cosmetic will be colorable
    type: BALLOON #select the type of cosmetic
    hide-menu: false #It will make the cosmetic visible or not in the menu.
    use-emote: false #This is used to specify if you want a cosmetic to be shown when using an ItemsAdder emote. By default it is disabled.
```

And, these are all options that are shared among all types of cosmetics.
