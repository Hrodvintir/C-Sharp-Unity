# Exercise 7: Finally, A Driving Game

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 - Create a project and add a sprite

Create a new 2D Unity project named Exercise7. Rename the SampleScene as Scene0. Add a new Sprites folder and use your Operating System to copy a sprite of your choosing into that folder. Drag the sprite into the Hierarchy window to create a game object in the scene. Run the game and watch nothing happen.

### Problem 2 - Drive horizontally

Create a new Scripts folder and create a new C# script in that folder called Driver. Open the new script in Visual Studio and add a documentation comment for the class. The Driver class (script) drives the game object based on keyboard input.

Add a constant called MoveUnitsPerSecond to store how many units your game object moves per second below the line that starts public class. Delete the Start method from the script. Add code to the body of the Update method to save the value on the Horizontal input axis (already provided in the default Unity project) into a variable called horizontalInput and to check if that value is non-zero. If there is input on that axis, change the x position of the game object (using a local variable as usual). The appropriate amount to change the x position is horizontalInput * MoveUnitsPerSecond * Time.deltaTime. The Keyboard Processing lecture covers keyboard input processing in detail.

Attach the Driver script to your game object in the Hierarchy window and run the game to drive horizontally.

### Problem 3 - Drive vertically

Add code to the body of the Update method to handle input on the Vertical input axis (already provided in the default Unity project) to change the y position of the game object.

Run the game to drive vertically (and horizontally if you'd like).
Exercise Solution

