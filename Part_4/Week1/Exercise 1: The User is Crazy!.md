# Exercise 1: The User is Crazy!

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 – Get user input

Start up your IDE and create a new Console Application project named Exercise1. Save the project in a reasonable location on the computer.

Add code to the \tt{Main}Main method to prompt for and read in an integer score from the user.

Run your code with a normal input, non-integer input (Bob, say), and a number larger than the maximum integer (2,147,483,647). See how the program throws exceptions for the second two inputs. You can use Ctrl+C in the Command Prompt window to get past the exception.

### Problem 2 – Add try and catch blocks

Put the prompting and reading in code inside a try block.

Add a catch block for a \tt{FormatException}FormatException, printing an appropriate error message inside the catch block. Run your code with non-integer input; you should see the error message.

Add a catch block for an \tt{OverflowException}OverflowException, printing an appropriate error message inside the catch block. Run your code with a number larger than the maximum integer (2,147,483,647); you should see the error message.

### Problem 3 – Add a finally block

Add a finally block that prints a message.

Run your code with a normal input, non-integer input (Bob, say), and a number larger than the maximum integer (2,147,483,647). The error messages for the two invalid inputs should still be displayed and in the message from the finally block should be displayed for all three inputs.

### Exercise Solution

[MonoDevelop Exercise 1 Solution](https://d3c33hcgiwev3.cloudfront.net/_a78ea3d55af0b05ccbc981c5a89e3d00_1-2-MonoDevelop-Exercise-1-Solution.zip?Expires=1643068800&Signature=ZY~XwDaavhiD8BHOZw5v-QQ7b4q0Hz0ZwO9VGpoTOFejpCvjPiPFoScC6Newg7g1Y9EmhVLHEt83R-xqIHLcCM-KZHMMX4XmPS~lL79rvmKlkXeH-7IsHM6XFkWNYbHL7Gsoja34owrp0FcUDH4G-LTvD2Z8Sgj2AmMBoP8ln~c_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

[Visual Studio Exercise 1 Solution](https://d3c33hcgiwev3.cloudfront.net/_07be70ecc3ae0515383d39810101636f_1-2-Visual-Studio-Exercise-1-Solution.zip?Expires=1643068800&Signature=bbuV6ZNkmv8leJgFVSWeo7bB2rJOBX6hYuAH9qwZAcQOh9y29S3fqq3CtQf1a6lhK6alWvxNcfvSEr6dVvDQDa7RQT~gYgssMqt-bPRGLg0UErqJvAGJT4AuDmJZKTa7cmdzrxUZZIwNPhs4EpTFI8sAILDiWksxxcKraRJTo9k_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
