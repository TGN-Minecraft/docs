# Inventory Layout

Our inventory setup in the YML is slightly different to what you may be expecting, so make sure to read this carefully.
```
player-inventory:
  hotbar:
    amount: 7
    0:
      item: iron sword
      auto-repair: true
      amount-of-enchantements: 1
      enchantments:
        0:
          type: sharpness
          level: 1
      amount: 1
    1:
      item: bow
      amount-of-enchantements: 0
      enchantments:
      auto-repair: true
      amount: 1
    2:
      item: diamond pickaxe
      amount-of-enchantements: 0
      enchantments:
      auto-repair: true
      amount: 1
    3:
      item: golden apple
      amount-of-enchantements: 0
      enchantments:
      auto-repair: false
      amount: 3
    4:
      item: stone
      amount-of-enchantements: 0
      enchantments:
      auto-repair: false  
      amount: 64
    5:
      item: wood
      amount-of-enchantements: 0
      enchantments:
      auto-repair: false
      amount: 64
    6:
      item: steak
      amount-of-enchantements: 0
      enchantments:
      auto-repair: false
      amount: 32

inventory:
  amount: 1
  0:
    value: 28
    item: arrow
    amount-of-enchantements: 0
    enchantments:
    auto-repair: false
    amount: 64
```

## The HotBar

First off, you must state how many items are going to be in the player's hotbar.
Then you must put the items into a list ```0:``` being slot one and ```1:``` being slot two.

## Item Breakdown

```
      item: iron sword
      auto-repair: true
      amount-of-enchantements: 1
      enchantments:
        0:
          type: sharpness
          level: 1
      amount: 1
```

First off, you must state the item name, a list of item names can be found [here](https://tgn-minecraft.github.io/docs/items).

If you want more items added, please submit an issues ticket inside the docs repository. 

State if the item is to automatically repair, and then say the number of enchantments. (If there are no enchants, put 0.)

If there is an enchantment please follow the layout
```
      enchantments:
        0:
          type: sharpness
          level: 1
```

Put ```0:``` as the first enchantment, then state type, and what level of enchantment you want it to be. 

Reference [here](https://tgn-minecraft.github.io/docs/enchantments) with the list of enchantments.

If there are more than one enchantment repeat the format except change the top number.
