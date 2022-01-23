# Programming Assignment: Getting Rich

### Assignment Description  

In this assignment, you'll implement \tt{MutualFund}MutualFund and \tt{EmployerSponsoredAccount}EmployerSponsoredAccount console app classes using inheritance.

### Why do we care?

Inheritance and the polymorphism we get "for free" when we use inheritance are incredibly powerful object-oriented features. Almost any non-trivial game you build will include some inheritance. Getting practice with inheritance in this assignment will help you implement more complicated class hierarchies in your games as you need them.

### Getting Started

Download the appropriate zip file for your OS below and unzip the file somewhere on your computer.

[Windows Programming Assignment 2 Materials](https://d3c33hcgiwev3.cloudfront.net/mJVWOu7fQ2WVVjru30NlBA_04692e86e6104090b570a6da5970bcf2_2-Windows-Programming-Assignment-2-Materials.zip?Expires=1643068800&Signature=Efnar8cS68i2mws2spLIOkRHf52v9xEaZcCPsDH-4~oArsESoKXaux3VX4mnz3agqa71lGsCHoODJjDWvJUbEIvxPdWcipcg1W9Wg2eNWXorWf9Ihj1Z-83FoH8EFA3Axwr~qN8ecFedxrbqIPq~L4fftQTGwDjLVVFzgmPRzZ8_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)


### Open the project in Visual Studio.

Important: You MUST only add code as indicated by the comments in that file. If you don't, you're virtually guaranteed to fail all the test cases in the automated grader.

### Requirements

For this assignment, you need to implement the \tt{MutualFund}MutualFund and \tt{EmployerSponsoredAccount}EmployerSponsoredAccount classes as shown in the class diagram below:

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/GM5Ddx7MQ6eOQ3cezEOnNw_37b41dcd206a918b7b55bdc9d459a2cf_Getting-Rich-Class-Diagram.png?expiry=1643068800000&hmac=ZoQdRY3YC6VEIGBl5yfcIo3QA03geVFFzljiFzsbyN0)

The Visual Studio project I provided to you stubs for the \tt{MutualFund}MutualFund and \tt{EmployerSponsoredAccount}EmployerSponsoredAccount classes, with lots of the functionality waiting for you to implement it. The project I provided also includes fully-implemented \tt{InvestmentAccount}InvestmentAccount and \tt{SavingsAccount}SavingsAccount classes, as well as a \tt{Program}Program class that tests the \tt{MutualFund}MutualFund and \tt{EmployerSponsoredAccount}EmployerSponsoredAccount classes. You need to make minor modifications to the \tt{InvestmentAccount}InvestmentAccount, \tt{SavingsAccount}SavingsAccount, and \tt{Program}Program classes as indicated in the comments in those classes; I had to comment out some code so that the project I provided you in the zip file compiles. The bulk of your work in this assignment is in the MutualFund.cs and EmployerSponsoredAccount.cs files, though.

How Are Children Different From Their Parents?

InvestmentAccount

The constructor uses the initial deposit to set the \tt{balance}balance field

The \tt{AddMoney}AddMoney method adds the given money to the balance (with error checking)

The \tt{UpdateBalance}UpdateBalance method is abstract, so it doesn't have a body

SavingsAccount

The constructor uses the initial deposit to set the \tt{balance}balance field and uses the provided interest rate to initialize the \tt{interestRate}interestRate field

The \tt{UpdateBalance}UpdateBalance method accrues interest using the \tt{interestRate}interestRate field

MutualFund

The constructor uses the initial deposit to set the balance

The \tt{AddMoney}AddMoney method deducts service charge using the \tt{ServiceChargePercent}ServiceChargePercent constant before changing the balance

The \tt{UpdateBalance}UpdateBalance method updates the balance using the value of the investments in the fund assuming 6% growth

EmployerSponsoredAccount

The constructor uses the initial deposit to set the balance

The \tt{AddMoney}AddMoney method doubles the money being added before adjusting the balance

Helpful Hint

Remember that child classes can call methods in their parent using the \tt{base}base keyword. You should do that as much as possible in your solution. Specifically, if you ever find yourself getting ready to copy code from the parent class and paste it into the child class, there's almost definitely a better way to do what you want. Try to figure the better way out before resorting to copying and pasting.

Required Output Format

The Program.cs file I provided handles all the output correctly. It simply prints Passed or FAILED for each test case that's selected by the user input.

Running Your Code

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

![](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/uygIsI9yRVqoCLCPcgVagw_01ecf389695b278283e9c5a50acdbc9a_Programming-Assignment-2-Multiple-Runs.png?expiry=1643068800000&hmac=CPp6WShlu887Wv8lb9GGHPjreBgfIcmbyQtCYGkKMvY)
  

  If your output doesn't match the image above EXACTLY (no extra words, characters, spaces, or blank lines) you'll fail all the test cases in the automated grader. Of course, you shouldn't get any FAILED output when you run your code!

Mac users: You'll have an extra blank line after the q. That's fine.  

### Test Case Inputs

The automated grader uses the set of test cases that are built into the Program.cs file I provided to you.

### Common Problems

Historically, lots of people post about grading errors on this assignment (because their code is wrong). Here are a couple things you should check:

You have to start with the Visual Studio project I gave you in the assignment materials and add your code in the section indicated. The code I gave you includes the appropriate structure for the automated grader to work. If you don't do this, you'll almost definitely fail all the test cases in the automated grader

I give you an example in this assignment (and all assignments) for what output you should get when you run the code multiple times. Be sure to try that example; if your code doesn't generate output exactly as shown in the example, your code isn't working properly    

### Submitting Your Solution

Go to the folder for your Visual Studio project and zip the MutualFund.cs and EmployerSponsoredAccount.cs files into a zip file. If you're on Windows, use the built-in Windows compression utility (select the files, right click, and Send to a Compressed (zipped) folder); do NOT use WinZip, 7Zip, or any other third-party compression program. I named my zip file ProgrammingAssignment2.zip, but you can name that file anything you want. 

Go to the programming assignment on Coursera and click My submission near the top (next to Instructions). Click the + Create submission button, click the blue button on the left, upload your zip file, and click the Submit button. If the Honor Code popup appears, click the check box, fill in your name if necessary, and click the Continue button. Then wait patiently while the automated grader grades your assignment!

Important: In the past, you've usually submitted your Program.cs file in previous programming assignments; DON'T DO THAT! You need to submit your zip file for this assignment.

### What Is The Automated Grader Telling Me?

If you post about getting errors from the automated grader, be sure to include a screenshot of the grader feedback. You can get to that feedback by clicking the Show grader output link in the Passed? column, then clicking the View grader feedback link that appears when you do that. You'll know you're in the right place when all the characters are either green or red.

Which Posts Will Dr. T Respond To?

I'm happy to try to help people solve problems they're having, but I'll only do that if you provide the appropriate information in your initial post. If you're getting a grader error, you have to provide both the screenshot from the previous section and a screenshot of your code running multiple times (as shown above) on your local computer, including the Press any key message at the end. That Press any key message is important, so be sure to include it
