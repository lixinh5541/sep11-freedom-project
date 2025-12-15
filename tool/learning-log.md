# Tool Learning Log

## Tool: **Phaser**

## Project: **Tetris with shapes**

---

### 10/5/25:
* install phaser with CDN
* width and height propeties set the size of the canvas element
* the canvas element is the rendering context where all the drawings from the code will go into
* the preload funtion is a section of the code and it contains the images that i want to load in
* the create funtion is another section that contains code of creating the images i want to load in
* Game objects(the images) are positioned centered so make the x and y value the center of the canvas
* put the pngs from phaser into a folder so you can access them and actually load them
* to put the code from downloaded zip files, you gotta extract them first

### 12/8/25:
* During part 4 of the tutorial, I learned the dynamic and static physics
* My tetris shapes will be dynamic because they will fall down which requires velocity
* In the tutorial, the code doesn't make the variable for you so I cant just copy and paste
* When loading in sprites, use a sprite sheet and not an image because thats how the sprites have animation
* Phaser supports flipping sprites to save on animation frames
* In order to let objects collide i will need a collider object
* I will try to collide my tetris shapes together with a collider object in my game
* I can change the gravity of the sprite, the higher the gravity, the faster the sprite falls down and when the gravity was at 0, the sprite didnt fall at all
* I in my game the gravity of the shapes will be low and get higher so they fall down faster as the game progress
* In part 7, I learn how to move my little dude or sprite, I reconize that the code has conditionals which is pretty cool
* Phaser has a built in key board manager and I think it means it detects when keys are being pressed which is good because I have no clue how to do that
* The speed of my dude or spirte can be changed with the numbers after the set velocity code

### 12/14/25:
* Repeat value says how many times it will repeat excluding the orginal item
* SetXY sets the coordinates of something you want
* stepX determines the value of how much the X coordinate changes from the each repeat
* In part 8, I add 12 stars that fall out the sky and I can change how bouncy the stars are when they drop
* Maybe the tetris shapes that drop can bounce
* The stars dissapear when the dude touches a star disabling the star so you cant see the star making it seem like the dude picked it up
* In part 9, I start of my declaring a variable for the score
* When the dude picks up a star it increases the score by 10, I remember I did something like that in 9th grade
* How the score is displayed, kinda like the CSS, is written in the create function
* In part 10, I add bombs which have the same physics of the stars being bouncy and dynamic
* If the dude hits a bomb then the game ends but nothing happens and you just cant control the dude no more
* for my game I want a button for the user to retry instead of reloading the page so I gotta learn how to do that
* countactive is used to count the number of stars and when its 0, it spawns a bomb
* Finished the tutorial




<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
