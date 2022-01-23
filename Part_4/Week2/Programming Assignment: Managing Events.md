#Programming Assignment: Managing Events

You have not submitted. You must earn 80/100 points to pass.

### Assignment Description  

In previous modules and courses, we implemented sub-optimal communications between our objects. In one of our games, our fish needed to know about the existence of the HUD; that doesn't really keep our objects as independent from each other as we'd like. One excellent solution to this problem is to implement an event system, so in this assignment you'll be implementing a simple event system.

More specifically, in this assignment, you'll implement \tt{MessageEvent}MessageEvent, \tt{CountMessageEvent}CountMessageEvent, \tt{Invoker}Invoker, \tt{Listener}Listener, and \tt{EventManager}EventManager classes.

### Why do we care?

Almost every non-trivial game -- at least those that care about good software design -- uses some form of event system. Getting practice with the simple event system in this assignment will help you implement more complicated event systems in your games as you need them.

### Getting Started

Download the appropriate zip file for your OS below and unzip the file somewhere on your computer.

[Windows Programming Assignment 3 Materials](https://d3c33hcgiwev3.cloudfront.net/-wzKPvHgQfSMyj7x4JH0NA_d1f5ae74d697438283641bfbe8a412ae_3-Windows-Programming-Assignment-3-Materials.zip?Expires=1643068800&Signature=Fd4S4MzK7sM~z4rS1HXnVH~tdGxrvZ6MdkkEMfAQ7mqm4c1x-nwQzmIzLcZATt~EPBj~Gq49EbjrntjXP4AdiVAKLssd4pwumKgn7SP9i0mzJGqN8EMijEDYl97lt05UfXqFd2Gb4JECNWscIh0k6KOZvRg7piJOYlbv5M7c44U_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

The contents of the zip file is different from what you've seen in the past, because it contains both Unity materials and a console app project for the autograder.

Unzip the Unity materials zip file somewhere on your computer and open the Unity project in Unity.

### Starting in Unity

For this assignment, you need to implement all the classes as shown in the class diagram below:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/GPpEHbkMTeu6RB25DO3r9g_05cbc10a972872449e98b01572d46749_Managing-Events-Class-Diagram.png?expiry=1643068800000&hmac=LPPVPYSijd74ZH0miiW2-XXGZRDDqo2BDgUnI2dWnVI)

The Unity materials I provided to you contains stubs for the \tt{Invoker}Invoker, \tt{Listener}Listener, and \tt{EventManager}EventManager classes, but you still have lots of work to do to finish implementing those classes (scripts). You also need to create and implement the \tt{MessageEvent}MessageEvent and \tt{CountMessageEvent}CountMessageEvent scripts.

In the class diagram above, the arrow (called an association) from the \tt{Invoker}Invoker class to the \tt{MessageEvent}MessageEvent class indicates that the \tt{Invoker}Invoker class has a \tt{MessageEvent}MessageEvent field named \tt{messageEvent}messageEvent.

Note: You may find that some of the work you did in the Is There Anybody Out There? exercise is useful as you complete this assignment.

Create a \tt{MessageEvent}MessageEvent script that inherits from \tt{UnityEvent}UnityEvent and create a \tt{CountMessageEvent}CountMessageEvent script that inherits from \tt{UnityEvent<int>}UnityEvent<int>. Remember, \tt{UnityEvent}UnityEvent and \tt{UnityEvent<>}UnityEvent<> are in the \tt{UnityEngine.Events}UnityEngine.Events namespace.

In the \tt{EventManager}EventManager script I provided, add code to the \tt{AddNoArgumentInvoker}AddNoArgumentInvoker and \tt{AddNoArgumentListener}AddNoArgumentListener methods to make the appropriate modifications to the provided \tt{noArgumentInvoker}noArgumentInvoker and \tt{noArgumentListener}noArgumentListener fields.

In the \tt{Invoker}Invoker script I provided, declare fields for a \tt{Timer}Timer object and a \tt{MessageEvent}MessageEvent object. Add code to the \tt{Awake}Awake method to create an instance of the \tt{MessageEvent}MessageEvent object in that field. Add code to the \tt{AddNoArgumentListener}AddNoArgumentListener method that adds a \tt{UnityAction}UnityAction delegate as a listener for the \tt{MessageEvent}MessageEvent; remember, \tt{UnityAction}UnityAction is in the \tt{UnityEngine.Events}UnityEngine.Events namespace. Add code to the \tt{Start}Start method to add the \tt{Invoker}Invoker as a no argument invoker in the\tt{EventManager}EventManager, add a Timer component, set its duration to 1 second, and run the timer. Add code to the \tt{Update}Update method to check if the timer has finished; if it has, call the \tt{InvokeNoArgumentEvent}InvokeNoArgumentEvent method and run the timer again. Add code to the \tt{InvokeNoArgumentEvent}InvokeNoArgumentEvent method to invoke the \tt{MessageEvent}MessageEvent.

In the Unity editor, attach the Invoker script to the main camera.

In the \tt{Listener}Listener script I provided, in the \tt{Start}Start method, add code to add the \tt{HandleMessageEvent}HandleMessageEvent method as a no argument listener in the\tt{EventManager}EventManager.

In the Unity editor, attach the Listener script to the main camera.

Run the game. The message should be printed in the Console window every second.

Follow similar steps to add event handling for the one int argument event. I just had the \tt{Invoker}Invoker script increment the value it includes each time it invokes the event, but do whatever you want to provide a different integer each time.

### Moving Over to the Console App

Now that you have your code working in Unity, it's time to move it over into the console app and make sure it will all work fine in the automated grader. Unzip the autograder materials zip file somewhere on your computer and open the Visual Studio solution.

The Visual Studio project I provided to you has stubs for the \tt{Invoker}Invoker, \tt{Listener}Listener, and \tt{EventManager}EventManager classes; you'll replace those files with the ones you developed in Unity soon.  The project I provided also includes a fully-implemented \tt{Program}Program class that tests the classes you've implemented.

Note: The autograder materials I've provided will compile, but if you run the project as it was provided it will crash. You need to add your classes to the project before you'll be able to run the code without crashing.

Copy the following files, AND ONLY THE FOLLOWING FILES, into the same folder as the Program.cs file in the console app project: MessageEvent.cs, CountMessageEvent.cs, Invoker.cs, Listener.cs, and EventManager.cs. Confirm that you want to overwrite the Invoker.cs, Listener.cs, and EventManager.cs files when prompted to do so. Do NOT copy the Timer script over; doing that will break the automated grader.

You should now be able to build and run the solution as discussed below.

### Required Output Format

The Program.cs  and the stub I provided for the \tt{Listener}Listener class handle all the output correctly. The output is simply Passed or FAILED for each test case that's selected by the user input.

### Running Your Code

Because of the code I included to work with the automated grader on Coursera, when you run your program the command prompt window will open and it will sit there doing nothing. To make your code run, type in a test case number (1 through 10, inclusive) and press the <Enter> key; your code should then run so you can check your output. 

For example, your input could be
```
\tt{3}3
```
to run the third test case.

You can actually run your code again if you want to by typing in a test case number and pressing the <Enter> key again. When you’re ready to stop running your code, type q (for quit).

Here's what running the code multiple times with different inputs should look like (though none of your test cases should fail!). The first line is the test case number, the second line is your output line, and so on:  
```
\tt{1}1

\tt{Passed}Passed

\tt{2}2

\tt{FAILED}FAILED

\tt{q}q
```
Important Note: The Coursera formatting makes it look like there's a blank line between each of the lines above, but there's not. The above output should be exactly 5 lines of input/output.

The image below shows my console window when I run the code multiple times as described above:
  
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/T-oi1edMTQOqItXnTJ0D-Q_3624d8ed27143bb0683760e5b8f11ffd_Programming-Assignment-3-Multiple-Runs.png?expiry=1643068800000&hmac=SI9CbjtlmS7SlBfgutSBpCsnwgx0j3LqslCWJ3j_6wY)

  
If your output doesn't match the image above EXACTLY (no extra words, characters, spaces, or blank lines) you'll fail all the test cases in the automated grader. Of course, you shouldn't get any FAILED output when you run your code!

Mac users: You'll have an extra blank line after the q. That's fine.  

### Test Case Inputs

The automated grader uses the set of test cases that are built into the Program.cs file I provided to you.

### Common Problems

Historically, lots of people post about grading errors on this assignment (because their code is wrong). Here are a couple things you should check:

You have to start with the assignment materials I gave you and add your code as described above. The code I gave you includes the appropriate structure for the automated grader to work. If you don't do this, you'll almost definitely fail all the test cases in the automated grader

I give you an example in this assignment (and all assignments) for what output you should get when you run the code multiple times. Be sure to try that example; if your code doesn't generate output exactly as shown in the example, your code isn't working properly    

### Submitting Your Solution

Go to the folder for your autograder Visual Studio project and zip the following files, AND ONLY THE FOLLOWING FILES, into a zip file:  MessageEvent.cs, CountMessageEvent.cs, Invoker.cs, Listener.cs, and EventManager.cs. If you're on Windows, use the built-in Windows compression utility (select the files, right click, and Send to a Compressed (zipped) folder); do NOT use WinZip, 7Zip, or any other third-party compression program. I named my zip file ProgrammingAssignment3.zip, but you can name that file anything you want. 

Go to the programming assignment on Coursera and click My submission near the top (next to Instructions). Click the + Create submission button, click the blue button on the left, upload your zip file, and click the Submit button. If the Honor Code popup appears, click the check box, fill in your name if necessary, and click the Continue button. Then wait patiently while the automated grader grades your assignment!

Important: In the past, you've usually submitted your Program.cs file in previous programming assignments; DON'T DO THAT! You need to submit your zip file for this assignment.

### What Is The Automated Grader Telling Me?

If you post about getting errors from the automated grader, be sure to include a screenshot of the grader feedback. You can get to that feedback by clicking the Show grader output link in the Passed? column, then clicking the View grader feedback link that appears when you do that. You'll know you're in the right place when all the characters are either green or red.

Which Posts Will Dr. T Respond To?

I'm happy to try to help people solve problems they're having, but I'll only do that if you provide the appropriate information in your initial post. If you're getting a grader error, you have to provide both the screenshot from the previous section and a screenshot of your code running multiple times (as shown above) on your local computer, including the Press any key message at the end. That Press any key message is important, so be sure to include it

### For the Curious

You might be wondering how we can use Unity classes in a console app for the autograder. That's what the UnityEngine.dll that's included in the Visual Studio solution is for.

That dll implements mock objects for some of the Unity classes. From Wikipedia: "In object-oriented programming, mock objects are simulated objects that mimic the behavior of real objects in controlled ways, most often as part of a software testing initiative. A programmer typically creates a mock object to test the behavior of some other object, in much the same way that a car designer uses a crash test dummy to simulate the dynamic behavior of a human in vehicle impacts." I wrote code that provides the appropriate interfaces (and some minimal functionality) for the classes in the \tt{UnityEngine}UnityEngine and \tt{UnityEngine.Events}UnityEngine.Events namespaces you should have used for your solution.


  
  
