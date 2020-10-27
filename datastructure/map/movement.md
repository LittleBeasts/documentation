Movement is handled by the litiEngine. 

For movement animation the correct sprites need to be imported to the game.litidata via the utiLITI software.
The sprites then can be imported when the "Creature" is instanced.
```JAVA
private Player() {
           super("characterSprite");
       }
```
A creature is a so called movable. So it has an update function which handles redraws.
```JAVA
    public void update() {

    }
``` 
To move a creature it needs a movement controller. The controller is added to the creature which needs controller input with the LITIengine command 'addController'. 
```JAVA
this.addController(new PlatformingMovementController<>(this)); 
```
There are different kinds of controllers with different functionallity provided by the LITIengine.

The last factor for movement is the camera. In the LITIengine there are different camera options, we will mostly lock our camera to the player movements.
```JAVA
Camera camera = new PositionLockCamera(Player.instance());
        camera.setClampToMap(true);
        camera.setZoom(0.2f,0);
        Game.world().setCamera(camera);
```
