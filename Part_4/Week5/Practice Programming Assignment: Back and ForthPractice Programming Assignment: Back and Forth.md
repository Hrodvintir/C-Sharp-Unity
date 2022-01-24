# Practice Programming Assignment: Back and Forth

### Assignment Description  

In this module, you learned about developing Unity classes; of course, you've been adding functionality to Unity classes (scripts) lots in the previous modules and courses in the Specialization!

In this assignment, you'll implement a Mover class that moves a game object back and forth.

### Why do we care?

This assignment gives you more practice implementing functionality in Unity, and it's also the first programming assignment that actually uses Unity in the autograder.

### Getting Started

Download the appropriate zip file for your OS below and unzip the file somewhere on your computer.

[Windows Programming Assignment 3 Materials](https://d3c33hcgiwev3.cloudfront.net/L1hHQxFpRDOYR0MRaTQzCg_f0b0bf110231402c8b436dcf516a7ff1_5-Windows-Programming-Assignment-3-Materials.zip?Expires=1643155200&Signature=FtYN0WPQ2wFla3WRIs0QQaE3wKj52ehRRgIMjF8kcMFOlXCFQ9ZCoZOajZyvVqJSS0IE5PWo9hR8Dtb~G9YnRkoonNFWW9fF-xuXzjXXOM~jcSsXv5UJKJvfd1uf9YmOhAZCehgLzRzzvcgDuMcrWM7-VUDVWzUaCAsqPtZnsU4_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

The contents of the zip file is different from what you've seen in the past, because it contains both Unity materials and a console app project for the autograder.

Unzip the Unity materials zip file somewhere on your computer and open the Unity project in Unity.

### Starting in Unity

All your work for this assignment is in the Mover.cs file; don't change ANY of the code in the other files I've provided to you.

For this assignment, you'll be adding functionality to the Start and Update methods in the provided Mover class stub to implement the required functionality. 

What is the required functionality? When the game starts, the game object the Mover script is attached to starts moving to the right. After (approximately) 1 second, the game object starts moving to the left instead. After another (approximately) 1 second, the game object starts moving to the right again instead. The game object keeps changing direction every second until the game is stopped.

The Unity materials I provided to you contains a stub for the Mover class, but you still have lots of work to do to finish implementing that class (script). 

In the Mover script I provided, add code to the Start method to add a Timer component, set its duration to the TimerDuration constant I provided, and run the timer. Add code to the Update method to check if the timer has finished; if it has, multiply the directionMultiplier field by -1 and run the timer again. After the code you just added, add code to move the game object using the directionMultiplier field, the MoveAmountPerSecond constant I provided, and Time.deltaTime. 

Note: The big idea behind the directionMultiplier field is that if it's set to 1 the game object will move to the right and if it's -1 the game object will move to the left. Given that idea, you should be able to figure out how to use the directionMultiplier field when you're moving the game object.

Run the game. The game object the Mover script is attached to should move back and forth on the screen, changing direction approximately every second.

### Moving Over to the Console App

Now that you have your code working in Unity, it's time to move it over into the console app and make sure it will all work fine in the automated grader. Unzip the autograder materials zip file somewhere on your computer and open the Visual Studio solution.

The Visual Studio project I provided to you has a stub for the Mover class; you'll replace that file with the one you developed in Unity soon.  The project I provided also includes a fully-implemented Program class that tests the classes you've implemented.

Although you can build and run the Visual Studio solution at this point, it will crash on all the test cases except for Test Case 1. Following the steps in the next paragraph will fix that.

Copy the following file, AND ONLY THE FOLLOWING FILE, into the same folder as the Program.cs file in the console app project: Mover.cs. Confirm that you want to overwrite the Mover.cs file when prompted to do so. Do NOT copy the Timer script over; doing that will break the automated grader.

Build the solution in Visual Studio. You should now be able to run the solution as discussed below.

### Required Output Format

The Program  class I provided handles all the output correctly. The output is simply Passed or FAILED for each test case that's selected by the user input.

### Running Your Code

Because of the code I included to work with the automated grader on Coursera, when you run your program the command prompt window will open and it will sit there doing nothing. To make your code run, type in a test case number (1 through 10, inclusive) and press the <Enter> key; your code should then run so you can check your output. 

For example, your input could be
```
3
```
to run the third test case.

You can actually run your code again if you want to by typing in a test case number and pressing the <Enter> key again. When you’re ready to stop running your code, type q (for quit).

Here's what running the code multiple times with different inputs should look like (though none of your test cases should fail!). The first line is the test case number, the second line is your output line, and so on:  
```
1

Passed

2

FAILED

q
```
Important Note: The Coursera formatting makes it look like there's a blank line between each of the lines above, but there's not. The above output should be exactly 5 lines of input/output.

The image below shows my console window when I run the code multiple times as described above:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/lf2nsvbvR5K9p7L273eSIw_753fb2c901084d6a9c24e8c88006f4f1_3-Programming-Assignment-3-Multiple-Runs.png?expiry=1643155200000&hmac=zKWDOBijees20naOFGQ1VpzjuX_FpYatPeDINNuj504)
  
If your output doesn't match the image above EXACTLY (no extra words, characters, spaces, or blank lines) you'll fail all the test cases in the automated grader. Of course, you shouldn't get any FAILED output when you run your code!

Mac users: You may or may not have an extra blank line after the q. That's fine.  

### Test Case Inputs

The automated grader uses the set of test cases that are built into the Program.cs file I provided to you.

### Common Problems

Historically, lots of people post about grading errors on this assignment (because their code is wrong). Here are a couple things you should check:

You have to start with the assignment materials I gave you and add your code as described above. The code I gave you includes the appropriate structure for the automated grader to work. If you don't do this, you'll almost definitely fail all the test cases in the automated grader

I give you an example in this assignment (and all assignments) for what output you should get when you run the code multiple times. Be sure to try that example; if your code doesn't generate output exactly as shown in the example, your code isn't working properly    

### Submitting Your Solution

Go to the programming assignment on Coursera and click My submission near the top (next to Instructions). Click the + Create submission button, click the blue button on the left, upload the Mover.cs file from the folder for your autograder Visual Studio project, and click the Submit button. If the Honor Code popup appears, click the check box, fill in your name if necessary, and click the Continue button. Then wait patiently while the automated grader grades your assignment!

Important: In the past, you've usually submitted your Program.cs file in previous programming assignments; DON'T DO THAT! You need to submit your Mover.cs file for this assignment.

### What Is The Automated Grader Telling Me?

If you post about getting errors from the automated grader, be sure to include a screenshot of the grader feedback. You can get to that feedback by clicking the Show grader output link in the Passed? column, then clicking the View grader feedback link that appears when you do that. You'll know you're in the right place when all the characters are either green or red.

### What If I Upload the Wrong File?

If you upload the wrong file, you'll almost definitely get compilation errors. The most common mistake people make is uploading the .sln file; if you do that, you'll get something like the following:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/hWPCagG8SGGjwmoBvFhh8Q_4ed4b7a62ab34228a316597281a59d97_Solution-File-Uploaded-Error.png?expiry=1643155200000&hmac=e5MQhUiwIFFK8uSoN6GtCeGv2519VYJHmfc6OyUFAz0)
  
If that happens, go back and upload the correct file.

Which Posts Will Dr. T Respond To?

I'm happy to try to help people solve problems they're having, but I'll only do that if you provide the appropriate information in your initial post. If you're getting a grader error, you have to provide both the screenshot of the grader feedback and a screenshot of your code running multiple times (as shown above) on your local computer, including the Press any key message at the end. That Press any key message is important, so be sure to include it.

For the Curious

You might be wondering how we can use Unity classes in a console app for the autograder. That's what the UnityEngine.dll that's included in the Visual Studio solution is for.

That dll implements mock objects for some of the Unity classes. From Wikipedia: "In object-oriented programming, mock objects are simulated objects that mimic the behavior of real objects in controlled ways, most often as part of a software testing initiative. A programmer typically creates a mock object to test the behavior of some other object, in much the same way that a car designer uses a crash test dummy to simulate the dynamic behavior of a human in vehicle impacts." I wrote code that provides the appropriate interfaces (and some minimal functionality) for the classes in the UnityEngine namespace you should have used for your solution. 
