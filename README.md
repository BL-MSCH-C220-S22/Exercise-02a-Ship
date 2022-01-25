# Exercise-02a-Ship

Exercise for MSCH-C220

A demonstration of this exercise is available at [https://youtu.be/rVAZ---1Aus](https://youtu.be/rVAZ---1Aus)

This exercise is the first opportunity for you to get your feet wet with Godot. It will explore the first step to creating an Arcade Space Shooter: a player-controlled character. We will be exploring key bindings; adding a sprite to our game; vectors, velocity, and acceleration; and our first physics body: KinematicBody2D.

First, be sure you have downloaded and installed the appropriate version of [Godot 3.4.2](https://godotengine.org/download) for your computer. Most likely, you will want the 64-bit version (only install the 32-bit version if the 64-bit doesn't run). Godot will download as a zip file. **Be sure to extract the application from the zip file and copy it to an appropriate location.**

Godot is currently not code-signed on the Mac, so if you are running it on a Mac, the first time you run it, you will need to right-click on the application and Open (and then indicate that you want to open it). Subsequently, it should open normally.

Fork the repository associated with this exercise. When that process has completed, make sure that the top of the repository reads [your username]/Exercise-02a-Ship. Edit the LICENSE and replace BL-MSCH-C220-S22 with your full name. Commit your changes.

Press the green "Code" button and select "Open in GitHub Desktop". Allow the browser to open (or install) GitHub Desktop. Once GitHub Desktop has loaded, you should see a window labeled "Clone a Repository" asking you for a Local Path on your computer where the project should be copied. Choose a location where you will keep the repositories for this class. Make sure the Local Path ends with "Exercise-02a-Ship" and then press the "Clone" button. GitHub Desktop will now download a copy of the repository to the location you indicated.

Open Godot. In the Project Manager, tap the "Import" button. Tap "Browse" and navigate to the repository folder. Select the project.godot file and tap "Open".

You should now see an empty Godot project. These are the requirements:

  - Create a new 2D scene. Rename the root Node2D node "Game"
  - Create key mappings:
    - w: forward
    - a: left
    - d: right
    - space: shoot
    - esc: menu
  - Create a new KinematicBody2D node as a child of Game. Rename it "Player"
  - Position Player at x=512, y=300
  - Add a Sprite node as a child of Player. Drag res://Assets/Player.png from the FileSystem panel to the Inspector panel: Texture
  - Add a script to Player. Save it as res://Player/Player.gd
    - The ship should be able to accelerate 5.0 per cycle through `_physics_process`. The max speed should be 400.00. It should rotate a 5 degree increments. Its position should wrap when it gets to the edge of the window. 
  - Create a singleton script called res://Global.gd. Set it to autoload. If the player presses the "menu" key, quit the game
 
We will, of course, need to deal with collisions, shooting, explosions, damage, and other weapon types later. If the ship is able to accelerate and turn (and wrap to the other side of the screen) when you are done, you have completed the exercise.

In GitHub Desktop, you should now see several files highlighted. Add a Summary message at the bottom of that panel (something like "Creates ship and sets up key bindings"), and push the "Commit to master" button. On the right side of the top, black panel, you should see a button labeled "Push origin". Press that now.

If you return to and refresh your GitHub repository page, you should now see that your files have been changed (with a new date).

Now edit the README.md file. When you have finished editing, commit your changes, and then turn in the URL of the main repository page (https://github.com/[username]/Exercise-02a-Ship (Links to an external site.)) on Canvas.

The final state of the file should be as follows (replacing my information with yours):
```
# Exercise-02a-Ship

Exercise for MSCH-C220

A user-controlled ship for a space-shooter game. Created in Godot.

## Implementation

Created using [Godot 3.4.2](https://godotengine.org/download)

Assets are provided by [Kenney.nl](https://kenney.nl/assets/space-shooter-extension), provided under a [CC0 1.0 Public Domain License](https://creativecommons.org/publicdomain/zero/1.0/).

## References
None

## Future Development
None

## Created by
Jason Francis
```
