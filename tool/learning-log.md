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

<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
