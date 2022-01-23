# Unity Project: Wacky Breakout Increment 1
### Unity Projects

In previous versions of this course, a similar Unity project was a required, graded, peer reviewed assignment. Unfortunately, the peer review process became unworkable for this project.  

I strongly encourage you to complete this project. It gives you good experience developing a Unity game using the concepts you’ve learned in this and previous modules (and courses).

### Project Description

You've decided to build a wacky version of the classic arcade game Breakout (we'll call it Wacky Breakout), with the following major differences:

 - The game will spawn an additional ball periodically, so you’ll generally have multiple balls in play at any given time  

 - Balls will have a specific lifetime, after which they’ll disappear

 - There will be several different block types, including blocks that are essentially effect activators

 - You’ll have a menu system that includes a main menu to select between play, help, and quitting the game; a difficulty menu to select difficulty; a help menu to describe the controls and rules to the player; and a pause menu.

A more detailed requirements specification for the game is included below; you should definitely download and read it.

[Wacky Breakout Requirements Specification](https://d3c33hcgiwev3.cloudfront.net/2FcDyGFtT6-XA8hhbX-vPg_810f2485b1a64774b8a9f14e68d3cff1_Wacky-Breakout-Requirements-Specification.pdf?Expires=1643068800&Signature=CkeUD1XG7hpucc6THlmUy0hlMMlnQE5wBXA9DaytnRXMQyCXQTscRBRPqD6Xdp3vFMpQAlb76lJ6O5y6rXFOecv7B~nHEFRYH6CwVqpWifiJUxdMkqaM4nekEbMWlTwiK7u~PYxKPd3lGlfCjtAeew2qk0BvzOArkxMDtuKMVKs_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

You won't actually complete the full version of the game until the end of the following course, but game developers typically break their game development into a number of increments. This project is the first increment of the six increments in your development of this game.

In this project, you'll start implementing basic gameplay.

### Why do we care?

Because it's fun to build games and this will be the second variant of an arcade game you'll complete in the Specialization! This project is the first increment in your implementation of Wacky Breakout, and it lets you use what you've learned in the modules in this and previous Specialization courses.

### Starting the Assignment

Download the zip file below and unzip the file somewhere on your computer.

[Wacky Breakout Increment 1 Materials](https://d3c33hcgiwev3.cloudfront.net/6rnPeq9LT6S5z3qvS5-kXA_21707a5a64f241a58e114ec51f33d9f1_3-Wacky-Breakout-Increment-1-Materials.zip?Expires=1643068800&Signature=Y5Xx6-qSuWjfWZLKJhtS5HAHo0AydOr1fxJHCyp7assStsTrwgqyduhGDMxFGksly0f00eIfKDZqnGawOB1I9TWKLPROfLMh4RMCvmWdJnGsb1~vbEouenugoTYWeV2Nhvprzgx6GZi8kYSzwm1LmNYPX9ZraWyY~sbk07zT12E_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

The zip file contains the following materials: a number of scripts and detailed step-by-step instructions for completing the project.

### Implementation Steps

I've provided detailed step-by-step instructions in the zip file above for you to follow if you'd like to have a "guided development experience" for this project.

Of course, you're also welcome to implement your solution without following those instructions, but you still need to implement all the required functionality for the project. Specifically, your solution needs to:

 - Let the player move the paddle horizontally using the left (to move left!) and right keys. The paddle shouldn't leave the playfield. It's fine if the A and D keys also move the paddle left and right

 - Let the player hit the ball with the paddle, aiming the ball using the contact point with the paddle

### Using Different Controls

You might think that the controls I've selected for the game (left/right to move the paddle) should be different controls instead. You might also think you should implement different controls you like better in your solution. Feel free to use whatever controls you prefer.

### Testing Your Game

Here are some rubrics you can use to confirm that the game functions correctly:

1. Paddle moves left and right based on left and right key input

2. Paddle is clamped to stay in playfield

3. Ball bounces off paddle at an angle based on where the ball hit the paddle

### Project Solution

The following download provides my solution to the project:

[Wacky Breakout Increment 1](https://d3c33hcgiwev3.cloudfront.net/qhUMXD0jRSOVDFw9I7UjNw_3c56e01592e747e083615d3b7b33e6f1_3-Wacky-Breakout-Increment-1-Solution.zip?Expires=1643068800&Signature=KCXNpJjj7Wo4S-H-stU86ZwnHbZifNM7ynJmxiXWnBKgPzsDieGZkQpMd2xaGZjNLyzU4YVpDWqxgpLpQcnYgIsx4j8wOT-cvgTJaFmb2TB5pGqWAOc2~igZsk9xlpicDf1of-dZIgXTOY-2Wet3cB7LjtlIDse08hCjWQRBWiI_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
