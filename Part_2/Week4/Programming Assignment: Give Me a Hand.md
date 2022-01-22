# Programming Assignment: Give Me a Hand

### Assignment Description

Now that you’ve learned about Lists, you realize that you could use a List to hold a hand of cards. Once you have the cards in your hand, you could look at them to count how many cards you have of each suit.

In this assignment, you'll read in how many cards should be in the hand, add that many cards to a List (by calling the GetCard method I provided), process the List to determine how many cards of each suit you have, then print out that information.

### Getting Started

Download the appropriate zip file for your OS below and unzip the file somewhere on your computer.

*Windows Programming Assignment 3 Materials*

Open the project from the extracted location in Visual Studio. Do NOT try to open the project from within the zip file.

Important: You MUST only add code as indicated by the comments in the project. If you don't, you're virtually guaranteed to fail all the test cases in the automated grader.

### Requirements

The code I’ve provided reads in the number of cards to put in the hand and stores it in a numCards variable. Your code must call the GetCard method the appropriate number of times and store the Card the method returns in a List variable. Once you’ve added the appropriate number of cards the List, you need to count how many cards of each suit are in the List and print that result.

You can read the documentation for the classes included in the ConsoleCards dll by double-clicking the index file in the Help folder in the extracted location for the zip file. Do NOT try to open the index file from within the zip file.

Your solution must do the following:

·        Store the cards in a List

·        Count the number of cards you have of each suit

·        Print the counts of each suit as described below

For example, if you have 1 club, 1 diamond, 0 hearts, and 3 spades in the array, your output should be the following on a single line (be sure to include a newline at the end):
```
C1 D1 H0 S3
```

We’d typically label our output to tell the user what the output means, but that will just confuse the automated grader. You must print ONLY the values described above in your output, with the values appearing on a single line with a single space between them.

### Running Your Code

Because of the code I included to work with the automated grader on Coursera, when you run your program the command prompt window will open and it will sit there doing nothing. To make your code run, type in a test case number (1 to 10, inclusive) and press the <Enter> key; your code should then run so you can check your output. For example, your input could be: 
```
1
```
You can actually run your code again if you want to by typing in a test case number (1 to 10, inclusive)  and pressing the <Enter> key again. When you’re ready to stop running your code, type q (for quit).

 Here's what running the code multiple times with different inputs should look like (remember, you're including a newline at the end of each of your output lines). The first line is the test case number input, the second line is your output line, and so on:
```
1

C1 D1 H0 S3

2

C5 D0 H0 S0

q
```
Important Note: The Coursera formatting makes it look like there's a blank line between each of the lines above, but there's not. The above output should be exactly 5 lines of output.

Test Case Inputs

The autograder uses the following set of test case inputs to test your code (1 test case per line):
```
Test Case 1: 2 of Clubs, 3 of Diamonds, 4 of Spades, 10 of Spades, Ace of Spades

Test Case 2: 2 of Clubs, 3 of Clubs, 4 of Clubs, 10 of Clubs, Ace of Clubs

Test Case 3: 10 or Diamonds, Ace of Diamonds

Test Case 4: 2 of Hearts, 3 of Hearts, 4 of Hearts, 5 of Hearts, 6 of Hearts, 7 of Hearts, 8 of Hearts

Test Case 5: No cards to put in hand

Test Case 6: 10 of Clubs, Jack of Clubs, Queen of Clubs, King of Clubs, Ace of Clubs

Test Case 7: Queen of Hearts

Test Case 8: Jack of Clubs, Jack of Diamonds, Jack of Hearts, Jack of Spades

Test Case 9: 2 of Spades, 3 of Spades, 4 of Spades, 5 of Spades, 6 of Spades, 7 of Spades, 8 of Spades, 9 of Spades, 10 of Spades

Test Case 10: 2 of Clubs, 3 of Diamonds, 4 of Hearts, 5 of Spades
```
You should figure out what the expected results are for each test case input and make sure your code is generating those expected results in the required format before submitting your code for grading.

### Submitting Your Solution

Go to the programming assignment on Coursera and click My submission near the top (next to Instructions). Click the + Create submission button, click the blue button on the left, upload your Program.cs file, and click the Submit button. If the Honor Code popup appears, click the check box, fill in your name if necessary, and click the Continue button. Then wait patiently while the automated grader grades your assignment!

### What Is The Automated Grader Telling Me?

If you post about getting errors from the automated grader, be sure to include a screenshot of the grader feedback. You can get to that feedback by clicking the Show grader output link in the Passed? column, then clicking the View grader feedback link that appears when you do that. You'll know you're in the right place when all the characters are either green or red.

### What If I Upload the Wrong File?

If you upload the wrong file, you'll almost definitely get compilation errors. The most common mistake people make is uploading the .sln file; if you do that, you'll get something like the following:
