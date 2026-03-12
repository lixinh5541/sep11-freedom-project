# Entry 3
##### 3/11/26

## What have I learned about Phaser?
### Movement of sprites
Using the [tutorial](https://phaser.io/tutorials/making-your-first-phaser-3-game/part1) on Phaser, I learned that to make sprites you use conditionals to change the velocity of the X values of the sprite. 
```js
if (cursors.left.isDown)
{
    player.setVelocityX(-160);
}
else if (cursors.right.isDown)
{
    player.setVelocityX(160);
}
else
{
    player.setVelocityX(0);
}

if (cursors.up.isDown && player.body.touching.down)
{
    player.setVelocityY(-330);
}
```
the numbers inside of `player.setVelocityX();` is the speed of the sprite when the specific key is pressed. A higher value will make the sprite faster and a lower value will make it slower. A negative X speed makes the sprite go left because X values go decrease going to the left. When no keys are pressed the velocity will be 0 because its not moving. 

### Bombs
I learned about some properties you can add on to some varibles like making them bouncy and deadly.
```js
        var bomb = bombs.create(x, 16, 'bomb');
        bomb.setBounce(1);
        bomb.setCollideWorldBounds(true);
        bomb.setVelocity(Phaser.Math.Between(-200, 200), 20);
```
1. The first line creates the varible and makes them drop down from the sky at random X values
2. `.setBounce();` makes the variable, bombs, bounce
3. `.setCollideWorldBounds(true);` makes the bombs bounce off the walls of the canvas so it wont go off the screen
4. The last line picks a random speed for the balls to move but makes the bombs drop at the same speed of 20

```js
function hitBomb (player, bomb)
{
    this.physics.pause();
    player.setTint(0xff0000);
    gameOver = true;
```
The function runs when the player variable touches the bomb and it just stops the game by puasing all the physica and setting `gameOver` to be true. `.setTint();` just changes the color of the variable and in my exmaple makes him go red.
### Whats next
* I want to more properties to add to my shapes in my tetris game to make it more unique
* Im going to learn how to end the game after the blocks reach a certern height
* I have to learn how to change the variable that is being moved by the user
* Im going to learn how do delete certain parts of variables 

[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
