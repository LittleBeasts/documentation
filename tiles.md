## General
A tile is a sprite with a fixed dimension and set properties.

### Properties
Dimension: The dimension should fit into a full HD grid. So dimensions could be: 

| Dimensions | Rows | Columns |
| :--------- | :--: | ------: |
| 40 x 40 px |  27  |   48    |
| 60 x 60 px |  18  |   32    |
| 80 x 80 px | 13,5 |   24    |
| 90 x 90 px |  12  |   21,3  |


***


**Properties of a tile:**

**passable** (boolean): Can a charakter cross the tile

**movement speed** (int): How fast can a charakter pass a tile

**image** (string): the location of the image file

**z-index** (int): on which z-coordinate is the tile

**x,y-location** (int, int): location on the screen, or map


```python
class Tile:
  def __init__(self, passable, moveSpeed, sprite, zIndex, aPosition)
    self.passable = passable #boolean
    self.moveSpeed = moveSpeed #int
    self.sprite = pygame.image.load(sprite) #String (location of sprite)
    self.zIndex = zIndex #position on z axis
    self.position = aPosition #(x,y)-position
  
  def draw(self, aOffset)
    screen.blit(self.sprite, (self.position[0]-aOffset[0], self.position[1]-aOffset[1])

```

