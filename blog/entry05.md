# Entry 5
##### 4/20/26

## What have I learned about my tool
### Images 
When i used `rect`, I couldnt make them collide with physics and thats when I looked and found an alternetive called image. Images made more properties that could be changed and had physics that i needed for my game. 
``` js
shape = this.physics.add.image(250, 25, 'block');
shape.setDisplaySize(100, 100);
shape.setTint(0xff0000);
shape.setCollideWorldBounds(true);
```
I had already established my variable and I added physics to it using image. This allowed me to do stuff like colliding with the world borders which basically means they cannot go outside the canvas. Some other things I did were changing the color and size of the image. This worked way better than rectangles and images can also have velocity which made it easier to move them. 


[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
