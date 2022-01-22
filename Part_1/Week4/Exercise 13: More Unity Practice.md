# Exercise 13: More Unity Practice
Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Getting Started

Download the zip file below and unzip the file somewhere on your computer.

*Exercise 13 Materials - iCloud*

### Problem 1 - Create a project and add sprites

Create a new 2D Unity project named Exercise13. Select the Main Camera and change Size to 3. Rename SampleScene to Scene0. Add a Sprites folder in the Project window and use your OS to add the two teddy bear images I provided to that folder. 

### Problem 2 - Add sprites to scene

Drag the green teddy bear from the Sprites folder in the Project window onto the Hierarchy window. 

Create a new Prefabs folder in the Project window and drag the sprite from the Hierarchy window onto the Prefabs folder in the Project window. Rename the prefab to TeddyBear. Rename the game object in the Hierarchy window GreenTeddyBear. Adjust the Position X and Y values in the Transform component of the GreenTeddyBear to move it toward the upper left of the scene.

Drag the TeddyBear prefab from the Project window onto the Hierarchy window. Rename the new game object in the Hierarchy window PurpleTeddyBear. Adjust the Position X and Y values in the Transform component of the PurpleTeddyBear to move it toward the lower left of the scene.

Drag the purple teddy bear from the Sprites folder in the Project window onto the Sprite value of the Sprite Renderer component in the Inspector pane. As you can see, this changes the sprite used by the sprite renderer, turning the teddy bear purple.

### Problem 3 - Make teddy bears move

Select the TeddyBear prefab and add a Rigidbody 2D component. To do this, click the Add Component button near the bottom of the Inspector and select Physics 2D > Rigidbody 2D. Run the game and watch both teddy bears fall. Remove gravity from the game by selecting Edit > Project Settings > Physics 2D from the main menu bar and setting the Y component of Gravity to 0.

Create a new Scripts folder in the Project window and add the TeddyBear.cs file I provided to that folder. Open up the script in Visual Studio and add code below the comment in the Start method to get a teddy bear moving to the right at a reasonable speed. 

Compile your code in Visual Studio to make sure you don't have any compilation errors. Once your build succeeds, close Visual Studio.

Attach the TeddyBear script to your GreenTeddyBear game object and run the game. You'll see that the green teddy bear moves to the right but the purple teddy bear doesn't move.

What we want to do next is apply the changes we made to the GreenTeddyBear game object back on the prefab so that all instances of the prefab share those changes. To do that, go to the Prefab area near the top of the Inspector, click the Overrides dropdown, and click the Apply All button on the right. This applies the changes you made to the instance of the prefab (the game object in the scene) to the prefab itself.

Run the game again. Both teddy bears should now move to the right.

Exercise Solution - iCloud

