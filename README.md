# pingPong
from pygame import * 

in_width = 700
win_height = 500
window = display.set_mode((win_width, win_height))
display.set_caption('123')

class GameSprite(sprite.Sprite):
    def __init__(self, player_image, player_x, player_y, size_x, size_y, player_speed):
        sprite.Sprite.__init__(self)



finish = False 

game = True

speed_x = 3
speed_y = 2

while game:
    if finish != True:
        ball.rect.x += speed_x
        ball.rect.y += speed_y


    for e in event.get():
        if e.type == QUIT:
            game = False


display.update()
