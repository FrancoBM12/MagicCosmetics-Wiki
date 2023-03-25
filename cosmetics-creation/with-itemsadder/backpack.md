---
description: Learn how to create a backpack in the ItemsAdder way.
---

# Backpack

Creating a backpack starts to become a bit more tedious and more so when it comes to first-person backpacks.

This is how a normal backpack is created:

* cosmetic file:

{% code lineNumbers="true" %}
```yaml
  creeper_backpack:
    permission: 'cosmetics.creeper_backpack'
    item:
      display: '&bCreeper backpack'
      item-adder: 'backpack' #item id from the backpack that everyone will see.
      lore:
        - ''
        - '&aSupport the creepers!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: -1 #model data is not required here.
    colored: true
    type: BAG
    distance: 100 #distance to where the players can see the backpack.
```
{% endcode %}

* BlockBench file:\


<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption><p>Edit mode - Check Position</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (6).png" alt=""><figcaption><p>Display mode - Check Y Position</p></figcaption></figure>

This is how a first person backpack is created:

* cosmetic file:

```yaml
  creeper_backpack:
    permission: 'cosmetics.creeper_backpack'
    item:
      display: '&bCreeper backpack'
      item-adder: 'backpack' #item id from the backpack that everyone will see.
      lore:
        - ''
        - '&aSupport the creepers!'
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: -1 #model data is not required here.
      for-me: 'item-adder;backpack_self' #item-adder;<id> - If this path is set, this item or modeldata will be displayed for the player who is using it, while the others will see the one that is already set. Remember, this path can use either number(modeldata) or id(itemsadder)
    colored: true
    type: BAG
    distance: 100 #distance to where the players can see the backpack.
    height: 3 #This is the height at which the backpack item will be set for the player himself.
```

* BlockBench file:

<figure><img src="../../.gitbook/assets/image (8).png" alt=""><figcaption><p>Edit Mode - Check Position</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (9).png" alt=""><figcaption><p>Display Mode - Position</p></figcaption></figure>

Finally, it remains to show the last option for the backpack:

```yaml
    space: 30 #if the player's yaw exceeds this number the backpack disappears and if not it will not be visible again (only affects the client and not others) If you don't want the backpack to disappear when its yaw changes, delete this path or leave it at 0.
```

<figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption><p>Here it still does not exceed the space it was given.</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption><p>Here the space has already passed, so only the backpack will be invisible to the player who is wearing it, once he/she looks up again and does not exceed the number, it will be returned.</p></figcaption></figure>

