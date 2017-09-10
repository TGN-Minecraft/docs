# Map Details
At the beggining of the YML you must state the map details.
```
map-details:
  title: 'Alpine Mining'
  world: alpine_mining
  map-version: 1.1
  version: 0.1
  amount-of-map-authors:
    value: 3
    map-authors:
      0: rockymine
      1: DoomRobotBoy
      2: Rasta_Jol
  spectator-spawn:
    x: 66.378
    y: 57
    z: -176.508
```

At the begginng you must state the map name, which can be anything. In this example, it's alpine mining.

Below thet title of the map, you must state the map world, map worlds shouldn't have any spaces. In this example, the world is called alpine_mining.

Below that, you must state the map version and the config version. Don't worry about the config version, just leave it as ```0.1```. The map version
should be ```1.0``` unless there were any changes after the map was released. Then the map version should be ```1.1```

After stating the map version, world and title. You  must state the map authors (aka contributers), ALL CONTRIBUTERS MUST BE LISTED. 

First off you should state the amount of authors. In the example below, it's 3.
```
  amount-of-map-authors:
    value: 3
    map-authors:
      0: rockymine
      1: DoomRobotBoy
      2: Rasta_Jol
```

Then you must list the map authors. The first being ```0:```, the second being ```2```, and so on. Then you must state the current USERNAME of the player.

## Spectator Spawn

Finally, we come to the last part of the map details, which is the spectator spawn. The spectator spawn is where all players spawn at the before a match starts.
```
  spectator-spawn:
    x: 66.378
    y: 57
    z: -176.508
```

Remember to state the coordinates x, y, and z.
