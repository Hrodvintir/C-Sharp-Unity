# Unity Project: Wacky Breakout Increment 5

### Unity Projects

In previous versions of this course, this Unity project was a required, graded, peer reviewed assignment. Unfortunately, the peer review process became unworkable for this project.  

I strongly encourage you to complete this project. It gives you good experience developing a Unity game using the concepts you’ve learned in this and previous modules (and courses).

### Project Description

For this project, you're continuing your work on your Wacky Breakout game. 

As a reminder, a more detailed requirements specification for the game is included below; you should definitely download and read it.

[Wacky Breakout Requirements Specification](https://d3c33hcgiwev3.cloudfront.net/JaTGihkCSESkxooZAhhEyw_fb55d6a76ff7498e92decd038b9bbaf1_Wacky-Breakout-Requirements-Specification.pdf?Expires=1643068800&Signature=jRVh-Y-zVKmncNnWtEnZaTR0VpLpp3gu3fcpBK3dQfWr7vWoQ3zK8Gb5PTHQ12oH8YLcjWTd0H8hBsiIuKugxR-8o8WwJ9t~nzUtpVbn630V~FF3tt7qGSo~JAjdrLwq0Bze6T8VevNAyLe5~iXB8C8pO0MnDkdSA-o-A9tYRmE_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

You won't actually complete the full version of the game until the end of this course, but game developers typically break their game development into a number of increments. This project is the fifth increment in your development of this game.

In this project, you'll refactor your game to use event handling wherever possible. This doesn't change the functionality of the game, but it does lead to a much better object-oriented design. In addition, you'll add the following functionality:

The Freezer and Speedup blocks should implement their freezing and speeding up functionality. Numbers to control how long each of those effects last (2 seconds for both) and how much the balls in the game speed up (twice their original speed) need to be stored in and used from the configuration data file. NOTE: if a Speedup block is destroyed while a speedup is already in effect, 2 seconds should be added to the duration of the effect but the speed of the balls shouldn’t be increased. A Freezer block simply extends the time the paddle is frozen by another 2 seconds if the paddle is already frozen

### Why do we care?

Because this project is the fifth increment in your implementation of Wacky Breakout, and it lets you use what you've learned in the previous specialization courses and what you've learned in this module (hint: the effect block functionality should be implemented using events and event handlers and all the refactoring uses events and event handlers).

### Starting the Assignment

Download the zip file below and unzip the file somewhere on your computer.

[Wacky Breakout Increment 5 Materials](https://d3c33hcgiwev3.cloudfront.net/wyCtXYnHRdGgrV2Jx1XR_g_97df516fc49d465881cced7051d165f1_3-Wacky-Breakout-Increment-5-Materials.zip?Expires=1643068800&Signature=JQ~0GqSxxx9Sqxdcm3TKUT04aiBaO2aA-cQUAol8JBQ1j3wEJ2W8Yr~elSAcuG2nODJ5CtUngKzUjKeGdDJMV~nUExFw72LAZUw8XCKAH6F1BCP9grmlEylUybZw7i1c9u-O-VrZ8G6-K-4L16r2Xq4h0OozaYiED5eR-TYSvdA_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

The zip file contains a variety of useful resources for you to use on this project.

### Implementation Steps

I've provided detailed step-by-step instructions in the zip file above for you to follow if you'd like to have a "guided development experience" for this project.

Of course, you're also welcome to implement your solution without following those instructions, but you still need to implement all the required functionality for the project. Specifically, your solution needs to meet the requirements listed in the Project Description above.

### Testing Your Game

Here are some rubrics you can use to confirm that the game functions correctly:

1. The Freezer effect works properly

2. The Speedup effect works properly

Although the refactoring to use event handling doesn't have any visible effect on the game functionality, you should be sure to do that as well.

### Project Solution

The following download provides my solution to the project:

[Wacky Breakout Increment 5 Solution](https://d3c33hcgiwev3.cloudfront.net/DS6tIUWjTx6urSFFo88eNQ_19e1ab95be5b4dc0bd2df3c95140daf1_3-Wacky-Breakout-Increment-5-Solution.zip?Expires=1643068800&Signature=XAnvjODLz6Uh2C5CgqJEg9o4tisN93CLlZ7GgHJ9fZNzJ1rle8ieJNlYIlITX1O2CfUPAIh-vlMXdJaqlEwSWtrLqf4aKeV5rxefuX8ck2k-D8pJ8DrOo8Xo5WhbPWjdkk7NgPfUeNv0ZMpKFVkKCstppyVdnS2KTEOmmX0mB2s_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
