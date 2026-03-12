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
the numbers inside of `player.setVelocityX();` is the speed of the sprite when the specific key is pressed. A higher value will make the sprite faster and a lower value will make it slower. A negative X speed makes the sprite go left because X values go decrease going to the left. When no keys are pressed the velocity will be 0 because it's not moving. 

### Bombs
I learned about some properties you can add on to some variables like making them bouncy and deadly.
```js
        var bomb = bombs.create(x, 16, 'bomb');
        bomb.setBounce(1);
        bomb.setCollideWorldBounds(true);
        bomb.setVelocity(Phaser.Math.Between(-200, 200), 20);
```
1. The first line creates the variable and makes them drop down from the sky at random X values
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
The function runs when the player variable touches the bomb and it just stops the game by pausing all the physics and setting `gameOver` to be true. `.setTint();` just changes the color of the variable and in my example makes it go red.
## What's next
* I want to more properties to add to my shapes in my tetris game to make it more unique
* I'm going to learn how to end the game after the blocks reach a certain height
* I have to learn how to change the variable that is being moved by the user
* I'm going to learn how to delete certain parts of variables

## Engineering Design Process (EDP)
I believe that I am on step 2, researching the problem, and step 3, Brainstorm possible solutions, of the EDP. I'm definitely still learning about how Phaser works, which is researching the problem but as I learn, I think about how I'm going to include the code into my project. This makes me think I'm in the midpoint of step 2 to 3 because I am thinking about possible solutions on how to create my project as well as learning new code. 

## Skills
### How to learn
I can't just copy and paste code from the tutorial because that won't help me learn. I have to actually learn what the code does and not just for that specific moment. I do this by changing the code from the tutorial to my liking. This builds on my ability to learn because If i can change the code to be what i want then that means i would have learned how to use that piece of code. 

### Organization
I have to do learning logs every week to report what I learned about my code which helps me with my organization because I have to do that learning in my own free time. The thing about the learning logs is that there's no reminder and i dont work on it in class that much. This means I have to set something to remind me to do the learning logs in which I use Google. Since I work on it at home, I also use Google to see which days i dont have a lot of homework so I can work on learning my code. This helps with my organization a lot because I organize my tasks into specific dates.  


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)


