# Teams & Monuments

Setting out the amount of teams & monuments is crucial as it's one of the core feature of the game.

```
teams:
  amount-of-teams: 2
  0:
    spawn:
      x: -41.373
      y: 27
      z: -176.508
    title: Red Team
    colour: red
    amount-of-monuments: 2
    monuments:
      0:
        name: East
        location:
          x: 22.459
          y: 35
          z: -69.428
      1:
        name: West
        location: 
          x: -19.7
          y: 33
          z: -94.4
  1:
    spawn: 
      x: 42.609
      y: 27
      z: 321.488
    title: Blue Team
    colour: blue
    amount-of-monuments: 2
    monuments:
      0:
        name: East
        location: 
          x: 20.374
          y: 33
          z: 239.398
      1:
        name: West
        location: 
          x: -21.628
          y: 35
          z: 214.481
```

# Teams

```
teams:
  amount-of-teams: 2
  0:
    spawn:
      x: -41.373
      y: 27
      z: -176.508
    title: Red Team
    colour: red
    amount-of-monuments: 2
```
First of you're meant to state how many teams there are, you may state upto 7 teams. 
It should look something like this:
```
  amount-of-teams: 2
```
The value may be slightly different depending on your team.

After you state the amount, you must list the teams.
```
  0:
    spawn:
      x: -41.373
      y: 27
      z: -176.508
    title: Red Team
    colour: red
```

The first team should be ```0```. The second team should be ```1:```, etc.

Then you must state the location of the spawn. Make sure to state the X, Y, Z.
```
      x: -41.373
      y: 27
      z: -176.508
```
After that, you must state the team title & colour.

The title of the team can be anything and you can use any colour as long as it's in [this list](https://tgn-minecraft.github.io/docs/colours)
```
    title: Red Team
    colour: red
```

## Monuments

After stating the team name, it's spawn and colour, you must state how many monuments that team has. Teams can have upto 6 monuments.
```
    amount-of-monuments: 2
    monuments:
      0:
        name: East
        location: 
          x: 20.374
          y: 33
          z: 239.398
      1:
        name: West
        location: 
          x: -21.628
          y: 35
          z: 214.481
```
Under that list the monuments, the first being ```0:``` and the second being ```1:```, etc. 

Under that state the monument's name. Monuments can be called anything. Under the monument's name state the location of the obsidian block. 
Remember to include the coordinates x,y and z. Repeat for the second, third, fourth, etc. Monument. 

## Max amount of monuments per team.

Here's a table for the maximum of monuments per team depending on how many teams there are.

Amount of Teams | Max Amount of Monuments
2 Teams | 6 Monuments
3 Teams | 5 Monuments
4 Teams | 3 Monuments
5 Teams | 1 Monuments
6 Teams | 1 Monument
7 Teams | 1 Monument
