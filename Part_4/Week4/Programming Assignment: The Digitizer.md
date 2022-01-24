# Programming Assignment: The Digitizer

### Assignment Description  

As you saw in the Feed the Teddies lectures, the C# \tt{Dictionary}Dictionary class is a very useful collection class. I use dictionaries in three separate places in that small game, so you should realize that dictionaries are very common in the games we develop.

In this assignment, you'll implement a \tt{Digitizer}Digitizer console app class that provides useful functionality using a \tt{Dictionary}Dictionary.

### Why do we care?

Because dictionaries are so common in game development, getting some practice using them will help you improve your game development skills.

### Getting Started

Download the appropriate zip file for your OS below and unzip the file somewhere on your computer.

[Windows Programming Assignment 4 Materials](https://d3c33hcgiwev3.cloudfront.net/xOIZ4aPDRTuiGeGjwzU7qg_d45bab2523f6414cb215442c9ce9365c_4-Windows-Programming-Assignment-4-Materials.zip?Expires=1643068800&Signature=HpeKkEqP-mWhqVbfLewaN7S3bJbKDgbO~sHLvsjGAXM347f-fd1gl77BDXCgPMRZ6u7BJnzRihUfYszHG2pgRf9rC1IqyUttSkdzWohdh-~0WOru4e98FE-P5X03GZsRFMVQPGOxSu8UOlBwqrdOkKpVqbgJKZR0062vLg3h-w0_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

Open the project in Visual Studio. 

### Requirements

For this assignment, you need to implement a \tt{Digitizer}Digitizer class. The Visual Studio project I provided to you contains the \tt{Digitizer}Digitizer class (with comments included where you should be adding code) and a \tt{Program}Program class that tests the \tt{Digitizer}Digitizer class. You shouldn't change the Program.cs file at all (if you do, you'll break the automated grader), all your work in this assignment is in the Digitizer.cs file.

The big idea is that we can use the \tt{Digitizer}Digitizer class to convert from strings for digit names (like zero, one, etc.) to the actual numeric digit (like 0, 1, etc.). This is a great problem for a \tt{Dictionary}Dictionary, so that's how you should solve the problem.

You'll need to add code to declare and create an object for your \tt{Dictionary}Dictionary field, add code to the constructor to populate the dictionary with the mappings between the strings for digit names and the corresponding numeric digits (zero through nine, inclusive), and add code to the \tt{ConvertWordToDigit}ConvertWordToDigit method to return the corresponding numeric digit for valid strings for digit names or -1 for invalid digit names (like bob).

You code should handle mixed case strings properly, so the \tt{ConvertWordToDigit}ConvertWordToDigit method should return 1 for strings one, One, oNe, onE, ONe, oNE, and ONE.

Helpful Hint: To help meet that last requirement, read the \tt{String}String documentation to see how to convert string to lower or upper case.

### Required Output Format

The Program.cs file I provided handles all the output correctly. It simply prints the numeric digit for the string provided in the user input.

### Running Your Code

Because of the code I included to work with the automated grader on Coursera, when you run your program the command prompt window will open and it will sit there doing nothing. To make your code run, type in a string and press the <Enter> key; your code should then run so you can check your output. 

For example, your input could be
```
\tt{zero}zero
```
to convert that string to 0.

You can actually run your code again if you want to by typing in a string and pressing the <Enter> key again. When you’re ready to stop running your code, type q (for quit).

Here's what running the code multiple times with different inputs should look like (though none of your test cases should fail!). The first line is the test case number, the second line is your output line, and so on:  
```
\tt{zero}zero

\tt{0}0

\tt{One}One

\tt{1}1

\tt{tWo}tWo

\tt{2}2

\tt{bob}bob

\tt{-1}−1

\tt{q}q
```
Important Note: The Coursera formatting makes it look like there's a blank line between each of the lines above, but there's not. The above output should be exactly 9 lines of input/output.

The image below shows my console window when I run the code multiple times as described above:
  
![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/KDEewOEDQV6xHsDhA8FeKQ_5994eca6c743f2627bd5f67962703c46_Programming-Assignment-4-Multiple-Runs.png?expiry=1643068800000&hmac=hRD4n3xxfZRUFB_gxFrq_onslLqA4gNyc-wIZOtVUoU)
  
If your output doesn't match the image above EXACTLY (no extra words, characters, spaces, or blank lines) you'll fail all the test cases in the automated grader.

Mac users: You'll have an extra blank line after the q. That's fine.  

### Test Case Inputs

The autograder uses the following set of test case inputs to test your code (1 test case per line):
```
\tt{zero}zero

\tt{One}One

\tt{tWo}tWo

\tt{three}three

\tt{four}four

five
\tt{six}six

\tt{seven}seven 

\tt{nine}nine

\tt{bob}bob
```
You should figure out what the expected results are for each test case input and make sure your code is generating those expected results in the required format before submitting your code for grading.

###Common Problems

Historically, lots of people post about grading errors on this assignment (because their code is wrong). Here are a couple things you should check:

 - You have to start with the Visual Studio project I gave you in the assignment materials and add your code as indicated. The code I gave you includes the appropriate structure for the automated grader to work. If you don't do this, you'll almost definitely fail all the test cases in the automated grader

 - I give you an example in this assignment (and all assignments) for what output you should get when you run the code multiple times. Be sure to try that example; if your code doesn't generate output exactly as shown in the example, your code isn't working properly    

### Submitting Your Solution

Go to the programming assignment on Coursera and click My submission near the top (next to Instructions). Click the + Create submission button, click the blue button on the left, upload your Digitizer.cs file, and click the Submit button. If the Honor Code popup appears, click the check box, fill in your name if necessary, and click the Continue button. Then wait patiently while the automated grader grades your assignment!

Important: In the past, you've usually submitted your Program.cs file in previous programming assignments; DON'T DO THAT! You need to submit your Digitizer.cs file for this assignment.

### What Is The Automated Grader Telling Me?

If you post about getting errors from the automated grader, be sure to include a screenshot of the grader feedback. You can get to that feedback by clicking the Show grader output link in the Passed? column, then clicking the View grader feedback link that appears when you do that. You'll know you're in the right place when all the characters are either green or red.

Which Posts Will Dr. T Respond To?

I'm happy to try to help people solve problems they're having, but I'll only do that if you provide the appropriate information in your initial post. If you're getting a grader error, you have to provide both the screenshot from the previous section and a screenshot of your code running multiple times (as shown above) on your local computer, including the Press any key message at the end. That Press any key message is important, so be sure to include it
