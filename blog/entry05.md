# Entry 5
##### 4/20/26

## What have I learned about my tool
### Images 
When I used `this.add.rect`, I couldn't make them collide with physics and that's when I looked and found an alternative called image. Images made more properties that could be changed and had physics that I needed for my game. 
``` js
shape = this.physics.add.image(250, 25, 'block');
shape.setDisplaySize(100, 100);
shape.setTint(0xff0000);
shape.setCollideWorldBounds(true);
```
I had already established my variable and I added physics to it using an image. This allowed me to do stuff like colliding with the world borders which basically means they cannot go outside the canvas. Some other things I did were changing the color and size of the image. This worked way better than rectangles and images can also have velocity which made it easier to move them. 

### Collisions 
To add collisions to my game, I made the shapes that fell down get pushed into an array. Then I went through the entire array and made the new shape collide with what is in the array.
```js
landedShapes.forEach(landed => {
scene.physics.add.collider(shape, landed);
});
```
LandedShapes is the array name and the code, `.forEach`, loops through every element in the array. With every element, `scene.physics.add.collider` it adds a collider between the new shape and all the existing landed shapes and it just stops them from passing through one another. 
## How I finished my MVP
#### (Preview)[https://lixinh5541.github.io/sep11-freedom-project/]
#### (Code)[https://github.com/lixinh5541/sep11-freedom-project/blob/main/index.html]
Along the way of making my MVP, I faced a lot of challenges that I normally google to see if there's any code that could be a solution for my problem however I just couldn't find solutions to some problems and turned to ai. A problem I faced was with using `this.add.rect` and I searched and found images on this [page](https://docs.phaser.io/phaser/concepts/gameobjects/image). However when I first tried to use it, it had no color and i couldnt do anything to add color to it. This is where I turned to ai it gave me this code:
```js
const g = this.make.graphics({ x: 0, y: 0, add: false });
g.fillStyle(0xffffff);
g.fillRect(0, 0, 100, 100);
g.generateTexture('block', 100, 100);
```
Ai explained that the issue was it was missing textures so that's why it was black and didn't look like anything. I asked ai to explain to me what each line of code meant and it told me `this.make.graphics` creates a mini canvas where I can make my texture and the `false` part was to make it not get added to the scene so it wont be visable. `.fillStyle` just sets the initial color to white and `.fillRect` makes a rectangle. This all comes together with `.generateTexture` which creates the texture and names it block so it could be used elsewhere like my images. 
## EDP (Engineering Design Process)
I think I am just finished with step 5, creating a prototype, as I completed my MVP which is not my finished product but it works. Now im on step 6-7, test and evaluate the prototype and improve as needed, because I need to see what else is there I can improve on my game and make it better. 
## skills
### Time Management
With the MVP deadline coming up, I was shocked and panicking because I overestimated myself with what I can do. This was when I started to prioritize doing my MVP and removing certain parts that were unnecessary to my game. Although there are still many features I'd like to add, having a playable game was the most important thing and I prioritized my time to get that MVP done. This meant i spent more time coding but also used my time on more important aspects in my game rather than perfecting one so i can use my time more wisely. 
### Growth mindset
Although I was making my game, there were things I didn't know how to do that prevented me from doing so. This made me realize that making my MVP should also be a time for me to grow. Even though I spent time learning, there was much i didnt know that can help me work towards my MVP. I spent my time coding my game but also learning new stuff too which contributed to my growth mindset as im not perfect and there are things i still have to learn even if i took time to prepare myself. 
[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
