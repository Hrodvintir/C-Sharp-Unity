# Programming Assignment: Who Is It?

### Assignment Description  

The key part of this assignment is reading a csv string from a file, extracting the values from the string, and saving those values into fields in a class. You'll also add properties to the class so that consumers of the class can get those values.

In this assignment, you'll implement a \tt{PersonalData}PersonalData console app class that does that.

### Why do we care?

Because we regularly use files to store game tuning information, then process that information when we run our games. You'll use (or have used) these same ideas as you complete the optional Wacky Breakout Increment 1 Unity project.

### Getting Started

Download the appropriate zip file for your OS below and unzip the file somewhere on your computer.

[Windows Programming Assignment 1 Materials](https://d3c33hcgiwev3.cloudfront.net/6nFsAgNrSA6xbAIDa2gO2Q_536660853c954909b8aba8472549b24d_1-Windows-Programming-Assignment-1-Materials.zip?Expires=1643068800&Signature=ImM8RKkeDajhf85PloHylnFL4-JgoOOtEC4FmTRL0V-9cqXa2ab6qkByGQrJl27LcKY~erZbUzcr37rg9hYAcivqW8zbV1t9ATklwKXTCr57SF1kb3wdWCyBvvBJsaUiWj9Zl4xZNN0m1LiYIj48czlFjjpTe7hINVpfzWQYI~A_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

***Important: You MUST only add code as indicated by the comments in that file. If you don't, you're virtually guaranteed to fail all the test cases in the automated grader.***

### Requirements

For this assignment, you need to implement a \tt{PersonalData}PersonalData class as shown in the class diagram below:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/dqmJM0aZROepiTNGmSTnGw_ef84ccb0c436c9b084fde84278050552_PersonalData-Class-Diagram.png?expiry=1643068800000&hmac=miAodmt-SiyluK2hMKoKRIO-DVz-ViLcXchY_mRO85o)

The Visual Studio project I provided to you contains the \tt{PersonalData}PersonalData class (with the constructor and properties unimplemented) and a \tt{Program}Program class that tests the \tt{PersonalData}PersonalData class. You shouldn't change the Program.cs file at all (if you do, you'll break the automated grader), all your work in this assignment is in the PersonalData.cs file.

The class diagram above (and the code I provided) doesn't include the fields you'll need to include in the \tt{PersonalData}PersonalData class; figuring those out on your own is part of the assignment. Note that the only method is the constructor, which has a parameter for the name of the file that contains the data you need to use to populate the fields.

The input file contains a single csv string containing the data you'll store in your PersonalData object. The format of that string is:

<first name>,<middle name>,<last name>,<street address>,<city>,<state>,<postal code>,<country>,<phone number>

Take a look at the ValidData.txt file included in the materials zip file to see what it looks like with "real" data.

The best approach is to implement the constructor and the \tt{FirstName}FirstName property first (to pass test case 2), then implement the \tt{MiddleName}MiddleName property (to pass test case 3), and so on. Make sure you initialize all your fields to "" to pass test case 1.

### Required Output Format

The Program.cs file I provided handles all the output correctly. It simply prints Passed or FAILED for each test case that's selected by the user input.

### Running Your Code

Because of the code I included to work with the automated grader on Coursera, when you run your program the command prompt window will open and it will sit there doing nothing. To make your code run, type in a test case number (1 through 10, inclusive), a comma, and a file name and press the <Enter> key; your code should then run so you can check your output. 

For example, your input could be

\tt{3,ValidData.txt}3,ValidData.txt

to run the third test case.

You can actually run your code again if you want to by typing in a test case number, a comma, and a file name and pressing the <Enter> key again. When you’re ready to stop running your code, type q (for quit).

Here's what running the code multiple times with different inputs should look like (though none of your test cases should fail!). The first line is the test case number, the second line is your output line, and so on:  
```
\tt{1,InvalidFileName.txt}1,InvalidFileName.txt

\tt{Passed}Passed

\tt{2,ValidData.txt}2,ValidData.txt

\tt{FAILED}FAILED

\tt{q}q
```
Important Note: The Coursera formatting makes it look like there's a blank line between each of the lines above, but there's not. The above output should be exactly 5 lines of input/output.

The image below shows my console window when I run the code multiple times as described above:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/2I4zm_xHSv2OM5v8Rzr9lQ_6a41b0b05630f327255e186462cf701c_Programming-Assignment-1-Multiple-Runs.png?expiry=1643068800000&hmac=2fJ8TT1xwa2mLmf450jZ8e58ChcugrgHxnEp8g4Ujg8)

 If your output doesn't match the image above EXACTLY (no extra words, characters, spaces, or blank lines) you'll fail all the test cases in the automated grader. Of course, you shouldn't get any FAILED output when you run your code!

Mac users: You'll have an extra blank line after the q. That's fine.  

### Test Case Inputs

The automated grader uses the set of test cases that are built into the Program.cs file I provided to you.

### Common Problems

Historically, lots of people post about grading errors on this assignment (because their code is wrong). Here are a couple things you should check:

 - You have to start with the Visual Studio project I gave you in the assignment materials and add your code in the section indicated. The code I gave you includes the appropriate structure for the automated grader to work. If you don't do this, you'll almost definitely fail all the test cases in the automated grader

 - I give you an example in this assignment (and all assignments) for what output you should get when you run the code multiple times. Be sure to try that example; if your code doesn't generate output exactly as shown in the example, your code isn't working properly    

### Submitting Your Solution

Go to the programming assignment on Coursera and click My submission near the top (next to Instructions). Click the + Create submission button, click the blue button on the left, upload your PersonalData.cs file, and click the Submit button. If the Honor Code popup appears, click the check box, fill in your name if necessary, and click the Continue button. Then wait patiently while the automated grader grades your assignment!

Important: In the past, you've usually submitted your Program.cs file in previous programming assignments; DON'T DO THAT! You need to submit your PersonalData.cs file for this assignment.

### What Is The Automated Grader Telling Me?

If you post about getting errors from the automated grader, be sure to include a screenshot of the grader feedback. You can get to that feedback by clicking the Show grader output link in the Passed? column, then clicking the View grader feedback link that appears when you do that. You'll know you're in the right place when all the characters are either green or red.

Which Posts Will Dr. T Respond To?

I'm happy to try to help people solve problems they're having, but I'll only do that if you provide the appropriate information in your initial post. If you're getting a grader error, you have to provide both the screenshot from the previous section and a screenshot of your code running multiple times (as shown above) on your local computer, including the Press any key message at the end. That Press any key message is important, so be sure to include it 
