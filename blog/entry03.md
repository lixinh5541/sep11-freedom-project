# Entry 3
##### 3/11/26

### What have I learned about Phaser?
##### Movement of sprites
Using the tutorial, I learned that to make sprites you use conditionals to change the velocity of the X values of the sprite. 
```js
if (cursors.left.isDown)
{
    player.setVelocityX(-160);

    player.anims.play('left', true);
}
else if (cursors.right.isDown)
{
    player.setVelocityX(160);

    player.anims.play('right', true);
}
else
{
    player.setVelocityX(0);

    player.anims.play('turn');
}

if (cursors.up.isDown && player.body.touching.down)
{
    player.setVelocityY(-330);
}
```
the numbers inside of `player.setVelocityX();` is the speed of the sprite when the specific key is pressed. A higher value will make the sprite faster and a lower value will make it slower. A negative speed makes the sprite go left because X values go decrease going to the left. When no keys are pressed the velocity will be 0 because its not moving. 
[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
