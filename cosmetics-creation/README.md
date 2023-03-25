---
description: Aquí encontrarás el como crear cosméticos de cualquier tipo.
---

# Creación de cosméticos

Aquí podrás encontrar como crear un cosmético.\
También sin ningún plugin que tenga soporte de objetos modificados\
o por lo contrario, saber como crear cosméticos con este tipo de plugins como ItemsAdder y Oraxen.

Diferentes tipos de cosméticos tienen opciones únicas que no son compartidas. Ahora mismo, te enseñaremos las opciones compartidas con todos los cosméticos.

```yaml
cosmetics:
  test_balloon: #Esta será la id del cosmético
    permission: 'cosmetics.test_balloon' #Para usar permisos, debes de tener la opción de permisos habilitada en la configuración.
    item:
      display: '&btest balloon' #Nombre que tendrá el cosmético
      texture: 'here' #En caso de que su objeto sea una cabeza, puede seleccionar la textura de la cabeza desde esta sección.
      material: LEATHER_HORSE_ARMOR #Material del cosmético, si usa ItemsAdder puede borrar esto.
      #Si usa ItemsAdder o Oraxen, puede simplemente poner el nombre del objeto aquí.
      item-adder: balloon #Opcional
      oraxen: balloon #Opcional
      lore: #Lore del item, si no quiere ponerle lore, puede borrar esta sección.
      - ''
      - '&cfirst'
      - ''
      unbreakable: true #Hace el objeto irrompible.
      glow: true #El objeto tendrá el efecto de glow.
      hide-attributes: true #Esconde los atributos del objeto.
      modeldata: 10030 #Aquí va el Custom Model Data del objeto, si usas ItemsAdder o Oraxen puede saltarselo.
      color: '#004F71' #Color por defecto del cosmético (en caso de que quiera uno).
    colored: false #Hace que el objeto pueda tintarse.
    type: BALLOON #Tipo de cosmético
    hide-menu: false #Hace el cosmético visible o no en el menú.
    use-emote: false #Esto es usado específicamente si quieres que el objeto sea visible usando una animación de ItemsAdder. Por defecto, aparecerá en 'false'.
```

Y estos son todas las opciones que son compartidas con todo los tipos de cosméticos.
