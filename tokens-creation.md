# Tokens creation

Here you will understand the creation of the tokens that complement the plugin very well.

{% code title="tokens.yml" overflow="wrap" lineNumbers="true" %}
```yaml
tokens:
  test_token: #token id
    item: #the format is similar to that of cosmetics.
      display: '&6Simple token'
      amount: 1
      material: LEATHER_HORSE_ARMOR
      lore:
        - ''
        - '&9Redeem the simple token!'
        - ''
      unbreakable: true
      glow: false
      hide-attributes: true
      modeldata: 10006
    cosmetic: cosmetic-id #the cosmetic you will get for redeeming this token.
    type: ALL #It is used to exchange a token to get a random cosmetic from a specific category of cosmetics.
    exchangeable: true #If this is active the cosmetic to token exchange will work.
```
{% endcode %}

### How does the type on tokens work?

These types are available:

* HAT
* BAG
* WALKING\_STICK
* BALLOON
* SPRAY
* ALL

When using this, you should take this into account:

* The token will get the cosmetics of the category you choose and will only choose the cosmetics you do not have unlocked.
* When you want to change your cosmetic that you redeemed using this token, you will not be able to do so unless you create a new token specifying the cosmetic id.
* It is necessary to have the cosmetic path set, as it will take the icon that will be displayed in the token exchange menu, when you click on the cosmetic it will give you a random cosmetic according to the type you chose.
