# Entry 1
##### 10/10/25
### Choosing a Topic
At the start, I got inspired and wanted to make an app that I can acutally use in real life to benefit me so I can impress everyone with my own app. I thought of a calorie tracker because it can help me gain some weight but I decided tp scrap that idea since i felt it would be boring. I will work on this project for the entire year so I knew i needed something that will actually intrest me into making so I dont slack off. Games immedialtelty came to mind and so i brainstormed of a game i can make that will be awesome to show my friends. This led me to want to make a tetris spin off because everyone knows tetris so it would be impressive to show people and i liked playing tetris a lot aswell. In the end, my plan was to create a game similar to tetris but with colored shapes like circles, triangles, and sqaures falling down and to clear them, the shapes must touch from one side to another with matching colors.

### Choosing the tool
Since I thought of my idea before choosing a tool, I was able quickly find tools that specialized in my type of game. The two I debated on using was [Phaser](https://phaser.io/) and [gDevelop](https://gdevelop.io/zh-cn) since both speacialized in games but i choose Phaser as it focused on 2D games. To start off, I watched a couple youtube videos from the Phaser website to see if it was right for me. I saw someone made a pokemon remix using Phaser and i thought it was so cool so I went to tinker with it. 

### Tinkering 
I tried to install Phaser but it was really confusing. Following the guides on the website did not help until I realized I can just copy and paste a line of code apparently called a CDN which I had also used last year. From there I used the website's tutorial to learn the basics of Phaser by reading through what every new line of code do. After i read the code and what it does, to help me better understand and remember, I would try to write the code without copy and paste and not looking at it. But for some reason my output was different from theirs. When i looked at my code, it seemed firmiliar and loooked like it was trying to use a png i did not have. Thats when I had my second breakthrough and discovered i needed assets, which were just pngs, which were given to me through the website. I downloaded the [assets](../tool/assets) into my IDE and everything was good. Here is the code i learned:
```js
<!DOCTYPE html>
<html>
<head>
    <script src="//cdn.jsdelivr.net/npm/phaser@3.86.0/dist/phaser.js">

    </script>

</head>
<body>

    <script>
   var config = {
    type: Phaser.AUTO,
    width: 800,
    height: 600,
    scene: {
        preload: preload,
        create: create,
        update: update
    }
};

var game = new Phaser.Game(config);

function preload ()
{
    this.load.image('sky', 'assets/sky.png');
    this.load.image('ground', 'assets/platform.png');
    this.load.image('star', 'assets/star.png');
    this.load.image('bomb', 'assets/bomb.png');
    this.load.image('platform', 'assets/platform.png');     
    this.load.spritesheet('dude',
        'assets/dude.png',
        { frameWidth: 32, frameHeight: 48 }
    );
}
var platforms;

function create ()
{
    this.add.image(400, 300, 'sky');

    platforms = this.physics.add.staticGroup();

    platforms.create(400, 568, 'ground').setScale(2).refreshBody();

    platforms.create(600, 400, 'ground');
    platforms.create(50, 250, 'ground');
    platforms.create(750, 220, 'ground');
}

function update ()
{
}
    </script>

</body>
</html>
```

### EDP
### Skills 

[Next](entry02.md)

[Home](../README.md)
