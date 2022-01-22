# Shipbuilding 101 Unity Project

### Unity Projects

In previous versions of this course, this Unity project was a required, graded, peer reviewed assignment. Unfortunately, the peer review process became unworkable for this project.  

I strongly encourage you to complete this project. It gives you good experience developing a Unity game using the concepts you’ve learned in this and previous modules.

### Project Description  

You've decided to build a simplified version of the classic arcade game Asteroids. You won't actually complete the full version of the game until the course following this one, but game developers typically break their game development into a number of increments. This Unity project is the first increment in your development of this game.

In this project, you'll implement the ship for the game. Ship functionality will include thrusting, rotating, and screen wrapping.

### Why do we care?

Because it's cool to actually build a real game, even a simple one! This project is the first increment in your implementation of a simplified version of Asteroids, and it also lets you use almost everything you've learned in the course.

### Learning Goals

The learning goals for this assignment include many of the learning objectives from all the modules in the course. From Module 4, the learning goal is:

● Create a Unity game that processes keyboard input.

### Starting the Assignment

Download the zip file below and unzip the file somewhere on your computer.

*Shipbuilding 101 Unity Project Materials*

The zip file contains the following materials: a GameInitializer script, a ScreenUtils script, and detailed step-by-step instructions for completing the project.

### Implementation Steps

  It actually takes a surprising amount of work to get a functional Asteroids ship in your game. That's why I've provided detailed step-by-step instructions in the zip file above for you to follow if you'd like to have a "guided development experience" for this project.
  Of course, you're also welcome to implement your solution without following those instructions, but you still need to implement all the required functionality for the assignment. Specifically, your solution needs to:

 - Let the player apply thrust using the space bar to move the ship. The thrust has to be applied in the direction the ship is facing, and the ship should accelerate appropriately based on physics

 - Let the player rotate the ship using the left button to rotate counter-clockwise and the right button to rotate clockwise

 - Screen wrap the ship. For example, when the ship leaves the bottom of the game window it should re-appear at the top of the game window. Make sure you handle all 4 edges of the game window as well as the corners, where you might have to wrap the ship both vertically and horizontally

### Using Different Controls

You might think that the controls I've selected for the game (space to thrust, left/right to rotate) should be different controls instead. You might also think you should implement different controls you like better in your solution. Feel free to use whatever controls you prefer.

### Screen Wrapping

Caution: Even if the screen wrapping is working properly, so a player could play the built game and screen wrapping would work perfectly, it may not seem to be working in the Unity Editor. The best thing to do is to build the game and play the built game. If, however, you want to just stay in the editor, double click the Main Camera in the Hierarchy window, then use Ctrl + Middle Mouse Wheel to zoom in on the Scene view until the box that shows the edges of the camera view just disappears from view.

### Testing Your Game

Here are the rubrics we used in previous versions of the course to confirm that the game functioned correctly:

1. Ship is in the scene when the game starts

2. Thrust is applied when the space bar is pressed or held

3. Thrust is applied in the direction the ship is facing

4. The ship rotates counter-clockwise when the left key is pressed or held and the ship rotates clockwise when the right key is pressed or held

5. The ship screen wraps properly. Wrapping should work correctly for the left, right, top, and bottom sides as well as all four corners. 

### Project Solution

The following download provides my solution to the project:

*Shipbuilding 101 Unity Project Solution*
