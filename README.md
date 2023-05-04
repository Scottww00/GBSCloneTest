
> http://arcade.makecode.com/#tutorial:https://github.com/calebmamula/cn-ninja-invaders-gbs

### @explicitHints true
# Code Ninjas Unofficial GBS (Ninja Invaders)


```assetjson
{
  "README.md": " ",
  "assets.json": "",
  "images.g.jres": "{\n    \"image1\": {\n        \"data\": \"hwQMABAAAAAADw8AAAAAAADwAAAA8A8AAP//APAPAADwv/0P//8P8P//Ef/////////x/////////9v/////AP//8f////////8R///////wv/0P//8P8AD//wDwDwAAAAAAAADwDwA=\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"displayName\": \"ninja\"\n    },\n    \"P!SN:(/KL=)hR}9=bfH@\": {\n        \"data\": \"hwQQABAAAAAAAAAAAAAAAAAAAAAA/wAAAAAAAP//AAD/AADwjw8AAP//APD4DwAA8PgP8P8AAADwj///DwAAAAD//4gPAAAAAADwiP//AAAAAPD///gPAAAA/w/wjw8AAPCPDwD//wAA8PgPAAD/AAD//wAAAAAAAP8AAAAAAAAAAAAAAAAAAA==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"displayName\": \"ninjaStar\"\n    },\n    \"*\": {\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"dataEncoding\": \"base64\",\n        \"namespace\": \"myImages\"\n    }\n}",
  "images.g.ts": "// Auto-generated code. Do not edit.\nnamespace myImages {\n\n    helpers._registerFactory(\"image\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"image1\":\n            case \"ninja\":return img`\n. . . . f f f f f . . . \n. . . f f f f f f f . . \nf . f f f f f f f f f . \n. f f b f f f f f b f . \nf . f d 1 1 b 1 1 d f . \n. . f f 1 f d f 1 f f . \n. . . f f f f f f f . . \n. . . . f f f f f . . . \n. . . f f f f f f f . . \n. . f f f f f f f f f . \n. . f f f f f f f f f . \n. f . f f f f f f f . f \n. f . f f f f f f f . f \n. . . . f f f f f . . . \n. . . . f f . f f . . . \n. . . f f f . f f f . . \n`;\n            case \"P!SN:(/KL=)hR}9=bfH@\":\n            case \"ninjaStar\":return img`\n. . . f f . . . . . . . . . . . \n. . . f f f f . . . . . . . . . \n. . . . f 8 f f . . . . . f f . \n. . . . f f 8 f . . . f f f f . \n. . . . . f f f . . f f 8 f . . \n. . . . . . f f f f f 8 f f . . \n. . . . . . f 8 8 f f f f . . . \n. . . f f f f 8 8 f . . . . . . \n. . f f 8 f f f f f . . . . . . \n. . f 8 f f . . f f f . . . . . \n. f f f f . . . f 8 f f . . . . \n. f f . . . . . f f 8 f . . . . \n. . . . . . . . . f f f f . . . \n. . . . . . . . . . . f f . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n`;\n        }\n        return null;\n    })\n\n    helpers._registerFactory(\"animation\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n\n        }\n        return null;\n    })\n\n    helpers._registerFactory(\"song\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n\n        }\n        return null;\n    })\n\n}\n// Auto-generated code. Do not edit.\n",
  "main.blocks": "<xml xmlns=\"https://developers.google.com/blockly/xml\"><variables><variable type=\"KIND_SpriteKind\" id=\"K2*z:_rzx9`[e$q8ZC0n\">Player</variable><variable type=\"KIND_SpriteKind\" id=\"VFp=:y%.@*gvR?Xi8u3Q\">Projectile</variable><variable type=\"KIND_SpriteKind\" id=\"KxeS}i?dXx4#:D3vE}w{\">Food</variable><variable type=\"KIND_SpriteKind\" id=\".xw^{:=xiscwN2qYYm:w\">Enemy</variable><variable id=\"spRe;C9SLdL:jzTGm{6H\">mySprite</variable><variable id=\"os[Cf)P,X,yMSHHqVlN(\">mySprite2</variable><variable id=\"`^y]STmkDE$yv*LJDq~}\">projectile</variable><variable id=\"H^emu(|CU(bHXs!MOtGg\">y</variable><variable id=\"uF@8rkprr{!G:HXMN=-H\">alien</variable></variables><block type=\"pxt-on-start\" x=\"0\" y=\"0\"><statement name=\"HANDLER\"><block type=\"gamesetbackgroundcolor\"><value name=\"color\"><shadow type=\"colorindexpicker\"><field name=\"index\">4</field></shadow></value><next><block type=\"variables_set\"><field name=\"VAR\" id=\"spRe;C9SLdL:jzTGm{6H\">mySprite</field><value name=\"VALUE\"><shadow xmlns=\"http://www.w3.org/1999/xhtml\" type=\"math_number\"><field name=\"NUM\">0</field></shadow><block type=\"spritescreate\"><value name=\"img\"><shadow type=\"screen_image_picker\"><field name=\"img\">assets.image`ninja`</field><data>{\"commentRefs\":[],\"fieldData\":{\"img\":\"myImages.image1\"}}</data></shadow></value><value name=\"kind\"><shadow type=\"spritekind\"><field name=\"MEMBER\">Player</field></shadow></value></block></value><next><block type=\"spritesetpos\"><value name=\"sprite\"><block type=\"variables_get\"><field name=\"VAR\" id=\"spRe;C9SLdL:jzTGm{6H\">mySprite</field></block></value><value name=\"x\"><shadow type=\"positionPicker\"><field name=\"index\">76</field></shadow></value><value name=\"y\"><shadow type=\"positionPicker\"><field name=\"index\">101</field></shadow></value><next><block type=\"game_control_sprite\"><mutation xmlns=\"http://www.w3.org/1999/xhtml\" _expanded=\"2\" _input_init=\"true\"></mutation><value name=\"sprite\"><block type=\"variables_get\"><field name=\"VAR\" id=\"spRe;C9SLdL:jzTGm{6H\">mySprite</field></block></value><value name=\"vx\"><shadow type=\"spriteSpeedPicker\"><field name=\"speed\">100</field></shadow></value><value name=\"vy\"><shadow type=\"spriteSpeedPicker\"><field name=\"speed\">0</field></shadow></value><next><block type=\"spritesetsetstayinscreen\"><value name=\"sprite\"><block type=\"variables_get\"><field name=\"VAR\" id=\"spRe;C9SLdL:jzTGm{6H\">mySprite</field></block></value><value name=\"on\"><shadow type=\"toggleOnOff\"><field name=\"on\">true</field></shadow></value><next><block type=\"hudsetScore\"><value name=\"value\"><shadow type=\"math_number\"><field name=\"NUM\">0</field></shadow></value><next><block type=\"hudSetLife\"><value name=\"value\"><shadow type=\"math_number\"><field name=\"NUM\">3</field></shadow></value></block></next></block></next></block></next></block></next></block></next></block></next></block></statement></block><block type=\"gameinterval\" x=\"582\" y=\"0\"><value name=\"period\"><shadow type=\"timePicker\"><field name=\"ms\">1000</field></shadow></value></block><block type=\"keyonevent\" x=\"670\" y=\"270\"><field name=\"button\">controller.A</field><field name=\"event\">ControllerButtonEvent.Pressed</field><statement name=\"HANDLER\"><block type=\"variables_set\"><field name=\"VAR\" id=\"`^y]STmkDE$yv*LJDq~}\">projectile</field><value name=\"VALUE\"><shadow xmlns=\"http://www.w3.org/1999/xhtml\" type=\"math_number\"><field name=\"NUM\">0</field></shadow><block type=\"spritescreateprojectilefromsprite\"><value name=\"img\"><shadow type=\"screen_image_picker\"><field name=\"img\">img`\n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n`</field><data>{\"commentRefs\":[],\"fieldData\":{\"img\":\"{g8l|={8[d#ivD+h=yG4\"}}</data></shadow><block type=\"screen_image_picker\"><field name=\"img\">assets.image`ninjaStar`</field><data>{\"commentRefs\":[],\"fieldData\":{\"img\":\"P!SN:(/KL=)hR}9=bfH@\"}}</data></block></value><value name=\"sprite\"><block type=\"variables_get\"><field name=\"VAR\" id=\"spRe;C9SLdL:jzTGm{6H\">mySprite</field></block></value><value name=\"vx\"><shadow type=\"spriteSpeedPicker\"><field name=\"speed\">0</field></shadow></value><value name=\"vy\"><shadow type=\"spriteSpeedPicker\"><field name=\"speed\">-100</field></shadow></value></block></value></block></statement></block><block type=\"spritesoverlap\" x=\"0\" y=\"431\"><value name=\"HANDLER_DRAG_PARAM_sprite\"><shadow type=\"argument_reporter_custom\"><mutation typename=\"Sprite\"></mutation><field name=\"VALUE\">sprite</field></shadow></value><value name=\"kind\"><shadow type=\"spritekind\"><field name=\"MEMBER\">Projectile</field></shadow></value><value name=\"HANDLER_DRAG_PARAM_otherSprite\"><shadow type=\"argument_reporter_custom\"><mutation typename=\"Sprite\"></mutation><field name=\"VALUE\">otherSprite</field></shadow></value><value name=\"otherKind\"><shadow type=\"spritekind\"><field name=\"MEMBER\">Enemy</field></shadow></value><statement name=\"HANDLER\"><block type=\"spritedestroy2\"><mutation xmlns=\"http://www.w3.org/1999/xhtml\" _expanded=\"2\" _input_init=\"true\"></mutation><field name=\"effect\">effects.spray</field><value name=\"sprite\"><block type=\"argument_reporter_custom\"><mutation typename=\"Sprite\"></mutation><field name=\"VALUE\">otherSprite</field></block></value><value name=\"duration\"><shadow type=\"timePicker\"><field name=\"ms\">200</field></shadow></value><next><block type=\"hudChangeScoreBy\"><value name=\"value\"><shadow type=\"math_number\"><field name=\"NUM\">1</field></shadow></value></block></next></block></statement></block></xml>",
  "main.py": "def on_on_overlap(sprite, otherSprite):\n    sprites.destroy(otherSprite, effects.spray, 200)\n    info.change_score_by(1)\nsprites.on_overlap(SpriteKind.projectile, SpriteKind.food, on_on_overlap)\n\ndef on_a_pressed():\n    global projectile\n    projectile = sprites.create_projectile_from_sprite(img(\"\"\"\n            . . . . . . . 6 6 . . . . . . . \n                    . . . . . . . 6 6 . . . . . . . \n                    . . . . . . 6 6 3 6 . . . . . . \n                    . . . . . . 6 3 3 6 . . . . . . \n                    . . . . . . 6 3 3 6 . . . . . . \n                    . . . . . . 6 3 3 6 . . . . . . \n                    . . . . . 6 6 3 3 3 6 . . . . . \n                    . . . . . 6 3 3 3 3 6 . . . . . \n                    . . . . . 6 3 3 3 3 6 . . . . . \n                    . . . . . 6 3 3 3 3 6 . . . . . \n                    . . . . 6 3 3 3 3 3 6 . . . . . \n                    . . . . 6 3 3 3 3 3 6 . . . . . \n                    . . . . 6 3 3 3 3 3 3 6 . . . . \n                    . . . . 6 3 3 3 3 3 3 6 . . . . \n                    . . . . 6 3 3 3 3 3 3 6 . . . . \n                    . . . . 6 6 6 6 6 6 6 6 . . . .\n        \"\"\"),\n        mySprite,\n        0,\n        -100)\ncontroller.A.on_event(ControllerButtonEvent.PRESSED, on_a_pressed)\n\nmySprite2: Sprite = None\nprojectile: Sprite = None\nmySprite: Sprite = None\nscene.set_background_color(4)\nmySprite = sprites.create(img(\"\"\"\n        . . . . f f f f f . . . \n            . . . f f f f f f f . . \n            f . f f f f f f f f f . \n            . f f b f f f f f b f . \n            f . f d 1 1 b 1 1 d f . \n            . . f f 1 f d f 1 f f . \n            . . . f f f f f f f . . \n            . . . . f f f f f . . . \n            . . . f f f f f f f . . \n            . . f f f f f f f f f . \n            . . f f f f f f f f f . \n            . f . f f f f f f f . f \n            . f . f f f f f f f . f \n            . . . . f f f f f . . . \n            . . . . f f . f f . . . \n            . . . f f f . f f f . .\n    \"\"\"),\n    SpriteKind.player)\nmySprite.set_position(76, 101)\ncontroller.move_sprite(mySprite, 100, 0)\nmySprite.set_stay_in_screen(True)\ninfo.set_score(0)\n\ndef on_update_interval():\n    global mySprite2\n    mySprite2 = sprites.create(img(\"\"\"\n            . . . . . . . 6 . . . . . . . . \n                    . . . . . . 8 6 6 . . . 6 8 . . \n                    . . . e e e 8 8 6 6 . 6 7 8 . . \n                    . . e 2 2 2 2 e 8 6 6 7 6 . . . \n                    . e 2 2 4 4 2 7 7 7 7 7 8 6 . . \n                    . e 2 4 4 2 6 7 7 7 6 7 6 8 8 . \n                    e 2 4 5 2 2 6 7 7 6 2 7 7 6 . . \n                    e 2 4 4 2 2 6 7 6 2 2 6 7 7 6 . \n                    e 2 4 2 2 2 6 6 2 2 2 e 7 7 6 . \n                    e 2 4 2 2 4 2 2 2 4 2 2 e 7 6 . \n                    e 2 4 2 2 2 2 2 2 2 2 2 e c 6 . \n                    e 2 2 2 2 2 2 2 4 e 2 e e c . . \n                    e e 2 e 2 2 4 2 2 e e e c . . . \n                    e e e e 2 e 2 2 e e e c . . . . \n                    e e e 2 e e c e c c c . . . . . \n                    . c c c c c c c . . . . . . . .\n        \"\"\"),\n        SpriteKind.food)\n    mySprite2.set_position(randint(0, 160), 0)\n    mySprite2.vy = 30\ngame.on_update_interval(1000, on_update_interval)\n",
  "main.ts": "controller.A.onEvent(ControllerButtonEvent.Pressed, function () {\n    projectile = sprites.createProjectileFromSprite(assets.image`ninjaStar`, mySprite, 0, -100)\n})\nsprites.onOverlap(SpriteKind.Projectile, SpriteKind.Enemy, function (sprite, otherSprite) {\n    sprites.destroy(otherSprite, effects.spray, 200)\n    info.changeScoreBy(1)\n})\nlet projectile: Sprite = null\nlet mySprite: Sprite = null\nscene.setBackgroundColor(4)\nmySprite = sprites.create(assets.image`ninja`, SpriteKind.Player)\nmySprite.setPosition(76, 101)\ncontroller.moveSprite(mySprite, 100, 0)\nmySprite.setStayInScreen(true)\ninfo.setScore(0)\ninfo.setLife(3)\ngame.onUpdateInterval(1000, function () {\n\t\n})\n",
  "pxt.json": "{\n    \"name\": \"Ninja Invaders - Copy\",\n    \"description\": \"\",\n    \"dependencies\": {\n        \"device\": \"*\"\n    },\n    \"files\": [\n        \"main.blocks\",\n        \"main.ts\",\n        \"README.md\",\n        \"assets.json\",\n        \"main.py\",\n        \"tilemap.g.jres\",\n        \"tilemap.g.ts\",\n        \"images.g.jres\",\n        \"images.g.ts\"\n    ],\n    \"targetVersions\": {\n        \"branch\": \"v1.12.30\",\n        \"tag\": \"v1.12.30\",\n        \"commits\": \"https://github.com/microsoft/pxt-arcade/commits/33228b1cc7e1bea3f728c26a6047bdef35fd2c09\",\n        \"target\": \"1.12.30\",\n        \"pxt\": \"8.5.41\"\n    },\n    \"preferredEditor\": \"blocksprj\"\n}\n",
  "tilemap.g.jres": "{\n    \"transparency16\": {\n        \"data\": \"hwQQABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true\n    },\n    \"*\": {\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"dataEncoding\": \"base64\",\n        \"namespace\": \"myTiles\"\n    }\n}",
  "tilemap.g.ts": "// Auto-generated code. Do not edit.\nnamespace myTiles {\n    //% fixedInstance jres blockIdentity=images._tile\n    export const transparency16 = image.ofBuffer(hex``);\n\n    helpers._registerFactory(\"tile\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"transparency16\":return transparency16;\n        }\n        return null;\n    })\n\n}\n// Auto-generated code. Do not edit.\n"
}






```






```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    projectile = sprites.createProjectileFromSprite(img`
        . . . . . . . 6 6 . . . . . . .
        . . . . . . . 6 6 . . . . . . .
        . . . . . . 6 6 3 6 . . . . . .
        . . . . . . 6 3 3 6 . . . . . .
        . . . . . . 6 3 3 6 . . . . . .
        . . . . . . 6 3 3 6 . . . . . .
        . . . . . 6 6 3 3 3 6 . . . . .
        . . . . . 6 3 3 3 3 6 . . . . .
        . . . . . 6 3 3 3 3 6 . . . . .
        . . . . . 6 3 3 3 3 6 . . . . .
        . . . . 6 3 3 3 3 3 6 . . . . .
        . . . . 6 3 3 3 3 3 6 . . . . .
        . . . . 6 3 3 3 3 3 3 6 . . . .
        . . . . 6 3 3 3 3 3 3 6 . . . .
        . . . . 6 3 3 3 3 3 3 6 . . . .
        . . . . 6 6 6 6 6 6 6 6 . . . .
        `, mySprite, 0, -100)
})
sprites.onOverlap(SpriteKind.Projectile, SpriteKind.Enemy, function (sprite, otherSprite) {
    sprites.destroy(otherSprite, effects.spray, 200)
    info.changeScoreBy(1)
})
mySprite.setKind(SpriteKind.Player)
sprite.setKind(SpriteKind.Player)
let mySprite: Sprite = null
scene.setBackgroundColor(4)
mySprite = sprites.create(assets.image`ninja`, SpriteKind.Player)
mySprite.setPosition(76, 101)
controller.moveSprite(mySprite, 100, 0)
mySprite.setStayInScreen(true)
info.setScore(0)
game.onUpdateInterval(1000, function () {
     alien = sprites.createProjectileFromSide()
    alien.setKind(SpriteKind.Enemy)
    alien.setPosition(randint(0, 160), 0)
})
mySprite.setPosition(randint(0, 10), 0)


```

```blockconfig.global
 myEnemy = sprites.createProjectileFromSide(img`
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    `, 50, 50)
```



## Introduction @showdialog
In this tutorial, you will create your very own video game. Enemies will be falling from the sky, and it's up to you to shoot them before they can reach you. Follow the instructions, but feel free to be creative and add custom details. Click Ok to get started!
![Game Example](https://raw.githubusercontent.com/CalebMamula/cn-ninja-invaders-gbs/master/images./ninja-invader-gif.gif)
## GBS: Ninja Invasion Step 1
### Making Our Background  


First up, our game needs a background. Grab a ``||scene:set background color||`` block from the ``||scene:Scene|`` dropdown and place it inside our ``||loops:on start||`` container already on the screen.


Click the grey bubble in the ``||scene: set background color||`` block and select a color to use as a background.


Chcek the Game Window on the right side of the screen to see the selected background color appear!


Click **Next** to go to the next step.


## GBS: Ninja Invasion Step 2
### Add Our Player Sprite


Now we are going to create our main character. Use a ``||variables:set [mySprite] to||`` block from the ``||sprites:Sprites||`` dropdown and place it at the bottom of the ``||loops: on start||`` container.


Click the grey oval and select the ninja picture under **My Assets**. Feel free to change this sprite and make it your own.


Make sure to change the name of your sprite by clicking on **mySprite** and pressing **Rename variable**. Change the name to Ninja, or something else if you'd like. Just remember what you chose.


## GBS: Ninja Invasion Step 3
### Code Movement


To move our ninja we need to use a ``||controller:move [mySprite] with buttons||`` block. Place this at the bottom of the ``||loops:on start||`` container.


We need to tell the game which sprite we want to move. Make sure to change **mySprite** to **Ninja**. This means the arrow keys and WASD can now move the ninja. Try it out!




## GBS: Ninja Invasion Step 4
### Restrict Movement
Did you notice your character can go off screen? To fix this we are going to use ``||sprites:set [mySprite] stay in screen |``. Once again, be sure to change **mySprite** to **Ninja**.


Next, we need our character to only go back and forth. First, grab ``||sprites:set position||`` from ``||sprites:Sprites||``. Look back to our ``||controller:Controller||`` block we placed in the previous step and change the x to 75 and the y to 100. (Numbers do not need to be exact)


We also need to stop the player from moving up and down. First click the + button on the right side on the block. Now, change the vy box on the ``||controller:move||`` block to 0.


## GBS: Ninja Invasion Step 5
### Spawning The Enemies Part 1
To spawn our enemies go to ``||game:Game||`` and pull the ``||game:on game update every||`` onto the editor. This is a container, so you can place it anywhere you'd like. The code we place here will run on a repeating timer.


Now we are going to create our enemy. Use a ``||variables:set [myEnemy] to||`` block from the ``||sprites:Sprites||`` dropdown and place it in the ``||game:on game update every||`` container.


Click the grey oval and select a sprite of your choice from **Gallery**.


At the end of the ``||variables:myEnemy|`` block, change the (vx) to 0 and the (vy) to 30. This will make our sprites go straight down. Also make sure to change the name of your sprite by clicking on **myEnemy** and pressing **Rename variable**. Pick any name that fits your new enemy.


## GBS: Ninja Invasion Step 6
### Spawning The Enemies Part 2


We will now use a ``||sprites:set [mySprite] position to||`` block into the ``||game:on game update every||`` container to make all enemies start at the top of the screen. Change **mySprite** to the name of your enemy.


Under ``||math:Math||`` grab a ``||math:pick random||`` block and place it into the x oval of our ``||sprites:set  [mySprite] position to ||`` block. Change the 10 to 160. Now any number can be picked between 0 and 160.


Notice how many enemies are coming down? We can change this by modifying the number at the top of the container. Instead of 500 ms, try 1 second (1000 ms).


Final thing for our enemies, we need to change their kind. Grab a ``||sprites:set [mySprite] kind to||`` block and choose Enemy. We will need this later on. Don't forget to set which sprite we are affecting.


## GBS: Ninja Invasion Step 7
### Ready, Aim, FIRE!
Now we are going to code our projectiles. To start, we are going to need a new container. Let's use the ``||controller:On A button pressed||``. This can be placed anywhere on the coding area. Code we place in this new container will run when we hit the space bar.


In this container we are going to place a ``||variables:set [projectile] to||`` block from the ``||sprites:Sprites||`` dropdown. *


At the end of the ``||variables:projectile||`` block we just placed in, change the (vx) to 0 and the (vy) to -100. This will make our sprites go straight up at a good speed.


Click the grey oval and either select a picture from **Gallery**, select the shuriken under **My Assets**, or quickly design your own. Keep it simple.


Change the **mySprite** to the name of your player, that way it will look like your player is firing the shots.


Open the game and try it out. Our character can now shoot projectiles when you press space.


## GBS: Ninja Invasion Step 8
### Destroy The Enemies Part 1


Almost done. For our next step, go to ``||sprites:Sprites||`` and grab the ``||sprites: on sprite of kind [Player] overlaps otherSprite of kind [Player]||``.


Change the first ``||sprites:Player||`` to ``||sprites:Projectile||``, and the second ``||sprites:Player||`` to ``||sprites:Enemy||``.


Now when our **Projectile** hits the **Enemy**, the code we place in this container will run.
```
## GBS: Ninja Invasion Step 9
### Destroy The Enemies Part 2
Place a ``||sprites:destroy [mySprite]||`` block inside our new overlap container. Drag an ``||variables:otherSprite||`` oval where it says ``||variables:mySprite||`` (This is found at the top of our ``||sprites:overlap||`` container).


Now click the + button on the new destroy block. Pick a fun effect and try it out. It is recommended to change the duration time to either 100 ms or 200 ms.


Last but not least, go to ``||info:Info||`` and grab a ``||info:change score by||`` block. Place this in our overlap container.


Try the game out! When you are ready, move on to the final step.


## GBS: Ninja Invasion Step 10
### ``||variables:C||`` ``||controller:u||`` ``||loops:s||`` ``||animation:t||`` ``||logic:o||`` ``||sprites:m||`` ``||music:i||`` ``||math:z||`` ``||scene:e||``
**The tutorial is finished, but now it's time to customize. Here are a few examples of things to try:**


-Put a dialog box or splash screen for game instructions.


-Customize the sprites and background to your liking. It's your game! (The fill option in the sprite editor can speed this process up)


-Put sound effects in the game for even more fun!


-Allow a way to win. Add a timer, add lives, or some combination. Maybe a highscore? Be creative!


-Add animations. For example, make the projectiles spin or change color as they fly.


-Make a new type of enemy. Maybe something that moves faster? Perhaps harder to kill?


*Decide with your Sensei on which customizations you want to make to your game. When you are ready, click **Done**.*



