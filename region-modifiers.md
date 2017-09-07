# Region Modifiers 

In the YML you are allowed to modify certain regions. 

Here's an example

```  modified-regions:
    amount-of-regions:
      value: 2
    0:
      type: cylinder
      center: 
        x: 42.609
        y: 27
        z: 321.488
      radius: 15
      height: 7
      modifier:
        build: false
        attack: true
        entry: true
      team: all
      message: '&cYou may not build in this team''s spawn!'
    1:
      type: cylinder
      center:
        x: -41.373
        y: 27
        z: -1.0
      radius: 15
      height: 7
      modifier:
        build: false
        attack: true
        entry: true
      team: all
      message: '&cYou may not build in this team''s spawn!'
```

In the example you can see at the top, the amount of regions. 
It is important that you state how many regions there are.

Go down one and you'll see ```0:```. You must use our common integer scale (0, 1, 2) to state the region ID.

Go down further and you see the type.
Currently there is only one type, Cylinder. 
You must state the coordiants for the center of the cylinder.
You must also state the radius & height. 

Below that you see 
```       modifier:
        build: false
        attack: true
        entry: true 
        ```
These are the current set of what you can modify. You can select if a player can build, attack/PVP and/or enter the region. 
```false``` means don't allow and ```true``` means allow. In this example players are not allowed to build.

```     team: all
      message: '&cYou may not build in this team''s spawn!'```

This section means what team this takes effect on. Remember to use the team colour only! If this effects all users, put ```team: all```
This message section is for when a player does an action which is set to false. You can send a message and you may use colour codes.

We have planned more modifiers & new types soon, so get excited for that.
