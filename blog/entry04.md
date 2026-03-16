# Entry 4
##### 3/16/26

### How have I progressed
I started to make my game however there is still a bunch of stuff that I have to learn while I make the game. To learn more code that i can potentially use, i browse through the [Phaser Documentation](https://docs.phaser.io/phaser/concepts/geometry) and [examples from Phaser](https://phaser.io/examples/v3.85.0). If I need something really specific that I cannot find, I search it up on google. Some things I learned are adding text and different shapes and I have already used them to start making my game. 
#### Text
To make sure users dont confuse my creation as a tetris rip off i used text to add a title. I positioned it in the top middle of the canvas and made it big so users could see. I learned code code from the [Phaser Documentation](https://docs.phaser.io/phaser/concepts/geometry). This is my code:
```js
this.add.text(300, 0, "LITRIS", {
    fontSize: "48px",
    fill: "#ffffff",
});
```
This just adds "LITRIS" on the top of the screen and I set the size to be big because it's a title and I made it white to complement my dark background. 

#### Shapes 
It took me a while to do shapes because my whole game revolved around shapes. I looked through phaser's information and found many ways to add shapes. Since shapes were so important I used AI to suggest which one I should use to make sure the code supports what I'm going to do to it and it settled on the code I found from the [examples on Phaser](https://phaser.io/examples/v3.85.0). Here is the code:
```js
let rectangle = this.add.rectangle(300, 300, 300, 200, 0xff0000);
let circle = this.add.ellipse(400, 300, 200, 100, 0x00ff00);
```
I made the shapes into variables because I will manipulate their properties later on and now I have two shapes, a rectangle and an ellipse. 
## My progress:
![](../tool/start-project.png)

### EDP
I am currently on step 4 and 5 in the engineering design process which is to plan the most promising solution and create a prototype. I have already created a plan for the MVP and the beyond MVP for my project. I have also started to create the MVP and made little progress as you could see my code above. I think I'm going to be at step 5 for a decent amount of time before step 6 which is to test and evaluate the prototype because I still have a long way to go before completing my MVP. 

### Skills 
#### Embracing failure
The project is not easy for me and everytime i code there's always a problem but that's okay because I always find a solution. When I was making shapes for my game, it wouldn't work at all and I see my classmates' progress so far and it makes me fail even worse. However i didnt let it discourage me and i eventually found my problem which was i was using an outdated version of phaser. Failing made me learn that tons of things can go wrong with your code and sometimes it's not even your code. 

#### Time management
I'm already struggling to keep up with the work of my classes so having a project that I have to do on my own without constant reminders has left me to have to improve. I use google task to see the assignments i have due and set them to specific dates so i have time to work on my project. This has helped me do tasks more effectively and I prioritize important and urgent things first and try to do them early so I have time to work on my game. 

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)


