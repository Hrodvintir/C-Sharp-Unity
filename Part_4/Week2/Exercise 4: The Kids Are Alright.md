# Exercise 4: The Kids Are Alright

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 – Create a console project and a parent class

Start up your IDE and create a new Console Application project named Exercise4. Save the project in a reasonable location on the computer. Build the project.

Add a class called \tt{Kid}Kid to your solution by following the IDE-specific instructions below.

MonoDevelop: Make sure the Solution pad is visible in your IDE; if it's not, select View > Pads > Solution from the menu bar at the top of the IDE. Right click the project name (it’s in bold, near the top of the Solution pad) and select Add > New File… Now select Empty Class template in the middle pane of the dialog, change the Name of the class to Kid, then click the New button. You can see in the Solution pad that the new class has been added to your project.

Visual Studio: Right click the project name (it’s in bold, near the top) in the Solution pane and select Add > New Item… Now select Class in the middle pane of the dialog, change the Name of the class to Kid, then click the Add button. You can see in the Solution pane that the new class has been added to your project.

Add a \tt{PrintMessage}PrintMessage method to your \tt{Kid}Kid class; be sure to mark the method virtual. In the body of the method, print some message.

In the \tt{Main}Main method of the Program.cs file, create a \tt{Kid}Kid object and tell it to print its message.

### Problem 2 – Add child class

Add a child class for a specialized kid: disobedient, artistic, friendly, whatever you want. Override the \tt{PrintMessage}PrintMessage method to print a different message.

In the \tt{Main}Main method of the Program.cs file, create an instance of the new child class and tell it to print its message.

### Problem 3 – Add another child class

Add another child class for a different specialized kid. Override the \tt{PrintMessage}PrintMessage method to print a different message.

In the \tt{Main}Main method of the Program.cs file, create an instance of the new child class and tell it to print its message.

### Exercise Solution

[MonoDevelop Exercise 4 Solution](https://d3c33hcgiwev3.cloudfront.net/_678d072887270c4cfc7cd524ec81e9e0_2-1-MonoDevelop-Exercise-4-Solution.zip?Expires=1643068800&Signature=XMjmQRI~E~8VcWeaHcw4A-eP9gQAS2LvKdulg-VqhWiyuwkbAX1VMeIyY3ynkROC2oEGDaCi58hwVxRrkdyx5tuKEPmNDa97sXTo3NogxuLSiTfcIXZjKbi3BfPom-Ypb-XYVxz06l3NVCZMXFr~G8tX3AK2ENNEyd3Wf07iztI_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

[Visual Studio Exercise 4 Solution](https://d3c33hcgiwev3.cloudfront.net/_0b14790f71436d4b375b11ed1b74c628_2-1-Visual-Studio-Exercise-4-Solution.zip?Expires=1643068800&Signature=Tmo5eGtWNqHJX2qKFIFKFkGB71ieKPIOU7Nw0vLTBV85FKPLx3YwcYqC4hJWH5ovcxLSifhGT7LUeYgcKbKEXtFAjHz6CnOu1A~qhRhZWO4YZRIkLHqrb~htHRj4tK6PIoDNEDUzuSBl-EoaFWHZxQX~ogMxNAG9WzWMf2-q05s_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
