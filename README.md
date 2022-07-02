# PYGAME_basics-2
# Python_Game: 利用PYGAME module 自己創造的小遊戲

**_1. References_**
   1. Pygame Page: http://pygame.org
   2. documentation: http://pygame.org/docs/ref/
   

**_2. What is PYGAME_**:
   * Pygame provides "Display,Sound,Image,Text,Event" to create games
   * Pygame can create 2-D games
   * Pygame detects users using "Keyboard, jjoystick,mouse" to control the games
   * Pygame provides lots of built-in game objects to create the games <br><br>

**_3.PYGame Basics_**:
| code | Description |
|:-----:|:----------:|
| _1.py_ | Create my game surface, game loop and drawing.|
| _2.py_ | Blit text, font, sound and image objects.   |
| _3.py_ | Getting uuser keyboard and collision dection.|

**_4. Code snippet_**
```python
#Create game display
import pygame
pygame.init()
WINDOW_WIDTH,WINDOW_HEIGHT=800,600
displayscreen=pygame.display.set_mode((WINDOW_WIDTH,WINDOW_HEIGHT))
pygame.display.set_caption("My first pygame!")

```
```python
#built image object and setting its rec
player_image=pygame.image.load("angry_bird.png")
player_rect=player_image.get_rect()
player_rect.left=32
player_rect.centery=WINDOW_HEIGHT//2
displayscreen.blit(player_image,player_rect)
```
**_5. Game Assets:_**:<br>
[Icon Archive](https://iconarchive.com/) : provide lots of game charators to download<br>
[Leshy SFMaker](https://www.leshylabs.com/apps/sfMaker/): download game music ,and can also create music by yourself

<img src="" width="400" height="300" alt="2.py program screenshot"><br>
