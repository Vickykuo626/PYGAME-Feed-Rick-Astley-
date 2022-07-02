# PYGAME_basics-2
### Python_Game: 利用PYGAME module 自己創造的小遊戲

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
import pygame
import random

pygame.init()#遊戲模組啟動
WINDOW_WIDTH,WINDOW_HEIGHT=1000,600
displayscreen=pygame.display.set_mode((WINDOW_WIDTH,WINDOW_HEIGHT))#產生畫布
pygame.display.set_caption("Feed Rick Astley!!")

```
```python
player_image=pygame.image.load("rick.png")
player_rect=player_image.get_rect()
player_rect.center=(WINDOW_WIDTH//2,WINDOW_HEIGHT-40)

coin_image=pygame.image.load("FFF.png")
coin_rect=coin_image.get_rect()
coin_rect.x=random.randint(32,WINDOW_WIDTH-32)
coin_rect.y=67
```
**_5. Game Assets:_**:<br>
[Icon Archive](https://iconarchive.com/) : provide lots of game charators to download<br>
[Leshy SFMaker](https://www.leshylabs.com/apps/sfMaker/): download game music ,and can also create music by yourself

<img src="https://github.com/Vickykuo626/PYGAME_basics-2/blob/main/1234.PNG" width="400" height="300" alt="2.py program screenshot"><br>
