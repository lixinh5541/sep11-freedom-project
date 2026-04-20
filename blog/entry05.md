# Entry 5
##### 4/20/26

## What have I learned about my tool
### Images 
When i used `this.add.rect`, I couldnt make them collide with physics and thats when I looked and found an alternetive called image. Images made more properties that could be changed and had physics that i needed for my game. 
``` js
shape = this.physics.add.image(250, 25, 'block');
shape.setDisplaySize(100, 100);
shape.setTint(0xff0000);
shape.setCollideWorldBounds(true);
```
I had already established my variable and I added physics to it using image. This allowed me to do stuff like colliding with the world borders which basically means they cannot go outside the canvas. Some other things I did were changing the color and size of the image. This worked way better than rectangles and images can also have velocity which made it easier to move them. 

### Collisions 
To add collisions to my game, I made the shapes that fell down get pushed into an array. Then i went trough the entire array and make the new shape collide with what is in the array.
```js
landedShapes.forEach(landed => {
scene.physics.add.collider(shape, landed);
});
```
LandedShapes is the array name and the code, `.forEach`, loops through every element in the array. With every element, `scene.physics.add.collider` it adds a collider between the new shape and all the existing landed shapes and it just stops them from passing through one another. 
## How I finished my MVP
Along the way of making my MVP, I faced a lot of challenges that I normally google to see if theres any code that could be a solutions for my problem however I just couldnt find solutions to some problems and turned to ai. A problem I faced was with using `this.add.rect` and I searched and found images on this [page](https://docs.phaser.io/phaser/concepts/gameobjects/image). However when i first tried to use it, it had no color and i couldnt do anything to add color to it. This is where I turned to ai it gave me this code:
```js
const g = this.make.graphics({ x: 0, y: 0, add: false });
g.fillStyle(0xffffff);
g.fillRect(0, 0, 100, 100);
g.generateTexture('block', 100, 100);
```
Ai explained that the issue was it was missing textures so thats why it was black and didnt look like anything. I asked ai to explain to me what each line of code meant and it told me `this.make.graphics` creates a mini canvas where I can make my texture and the `false` part was to make it not get added to the scene so it wont be visable. `.fillStyle` just sets the initial color to white and `.fillRect` makes a rectangle. This all comes together with `.generateTexture` which creates the texture and names it block so it could be used elsewhere like my images. 

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
