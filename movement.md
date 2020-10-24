Movement class should manage the possibilities, where a character can move and handle all animations regarding the character model

```python
import pygame

class Movement:
    def __init__(self, aDirection, aAnimation, speed, aPosition, aSize, screen):
        self.direction = aDirection  # [up,down,left,right,stand]
        self.loadSprites(aAnimation)
        self.speed = speed
        self.position = aPosition  # [x,y]
        self.size = aSize  # [width,height]
        self.steps = [0, 0, 0, 0, 0]  # [#up,#down,#left,#right,#stand]
        self.screen = screen

    def loadSprites(self, aAnimation):  # perhaps load from a folder
        for i in range(len(aAnimation)):
            for j in range(len(aAnimation[i])):
                self.animation[i][j] = pygame.image.load(aAnimation[i][j])  # load sprites into array for animation

    def move(self, aDirection):
        # key input sets aDirection
        if aDirection[0]:  # top
            self.direction = [1, 0, 0, 0, 0]
            self.position[1] -= self.speed
            self.stepsUp += 1
        if aDirection[1]:  # down
            self.direction = [0, 1, 0, 0, 0]
            self.position[1] += self.speed
            self.stepsDown += 1
        if aDirection[2]:  # left
            self.direction = [0, 0, 1, 0, 0]
            self.position[0] -= self.speed
            self.stepsLeft += 1
        if aDirection[3]:  # right
            self.direction = [0, 0, 0, 1, 0]
            self.position[0] += self.speed
            self.stepsRight += 1

    def resetSteps(self):
        self.stepsUp = 0
        self.stepsDown = 0
        self.stepsLeft = 0
        self.stepsRigth = 0
        self.stand = 0

    def stand(self):
        self.direction = [0, 0, 0, 0, 1]
        self.resetSteps()

    def draw(self, aOffset):  # method is called in the draw loop
        # reset counter for drawloop
        for i in self.steps:
            if self.steps[i] == 60:
                self.steps[i] = 0

        # animations for each direction
        for x in range(len(self.direction)):
            if self.direction[x] == 1:
                self.screen.blit(self.animation[x][self.steps[x] // 5],(self.position[0] - aOffset[0], self.position[1] - aOffset[1]))

       
```