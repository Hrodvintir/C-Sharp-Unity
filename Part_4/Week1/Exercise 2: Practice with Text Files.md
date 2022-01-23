# Exercise 2: Practice with Text Files

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 – Create a console project and a text file

Start up your IDE and create a new Console Application project named Exercise2. Save the project in a reasonable location on the computer. Build the project.

Use Notepad++, Notepad, or some other application to create a text file. Add four lines of text to the file – whatever you want! Save the file in the bin\Debug folder of your project.

### Problem 2 – Read in and echo the file

Read the lines in from the file and echo them to the console. Be sure to use try, catch, and finally blocks as appropriate. Don’t hard-code how many lines are in the file, use a while loop to keep reading from the file until the \tt{ReadLine}ReadLine method returns null.

Hint: You’ll need to add a using directive for the \tt{System.IO}System.IO namespace to get access to the \tt{StreamReader}StreamReader class.

### Problem 3 – Output a file with the even-numbered lines

Print the even-numbered (the second and fourth) lines from the input file to an output file. Be sure to use try, catch, and finally blocks as appropriate. Don’t hard-code how many lines you’ll be outputting, use some other more reasonable approach.

Open up your output file in the bin\Debug folder of your project to make sure your solution worked correctly.

Hint 1: If you save the lines from the input file in a \tt{List}List as you read them in, you can use a for loop to output the even-numbered lines to the output file.

Hint 2: MonoDevelop users will need to add a using directive for the \tt{System.Collections.Generic}System.Collections.Generic namespace to get access to the \tt{List}List class.

## Exercise Solution

[MonoDevelop Exercise 2 Solution](https://d3c33hcgiwev3.cloudfront.net/_6b3aef817f5ed4fd7a3a3ad6ecbd5ab7_1-3-MonoDevelop-Exercise-2-Solution.zip?Expires=1643068800&Signature=XM-w65J3rapVHvTNNtg03K67cYU8cOag5j0O2D~W7nu-lCYyFsSqLkMDUa~iWeH8LIo7ImCow3FowxAhPCYpuHZmtOwz79nwNZkeo2rDFn0kKyQKId-rL5QNf3-NSq3amTNPjnAK2UXIh8t89HfRU6L44QE~J~MNo4Bc8F2IuHE_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

[Visual Studio Exercise 2 Solution](https://d3c33hcgiwev3.cloudfront.net/_e5b658f902d6e6f6cd982d0ad6673dd1_1-3-Visual-Studio-Exercise-2-Solution.zip?Expires=1643068800&Signature=ESFQuEKnfMO1xIhEAIw2JD7OKvLitxq0mQrB5Q3xUQ1lhmrioSZqdI3tJJejPqmdLcL2W0vWXiMvx5UwOlchwtTckV5ClTIL0XBhOQckkpX7ZgZe7yPMkWj7irIYLsYzq65-X6h3lxVAG-45P6RuscpTDJ~sJ9gw7J6ewoo8RAk_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
