# Exercise 5: I Like to Move It Move It

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Getting Started

Download the zip file below and unzip the file somewhere on your computer.

[Exercise 5 Materials](https://d3c33hcgiwev3.cloudfront.net/_0af73c255c279187fbc413400498edb5_2-2-Exercise-5-Materials.zip?Expires=1643068800&Signature=CNk8njDWe4AU0mjb20y-kZ8G4b2Mj1QgSmmBed~gpQMA-FR6Vxqh6KQ5nK564JByfeo6P4ZI4-l1nRFqzL4TssqeFKK0rSOo0jCX7mtkQlRg8HiCx3Bc9TU8t~3M6rvjifmW9chiAiUGZFXlzGWleTY4GC-1p2Jzkn4ewmEzKDs_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

Open the project in Unity. You can do this by navigating to the Exercise5\Assets\scenes folder and double clicking scene0.

### Problem 1 – Add green ball child class and prefab

Drag the sprite for the green ball onto the Hierarchy window, rename it to GreenBall, and add a Rigidbody 2D component to it. Drag it onto the prefabs folder in the Project window to turn it into a prefab.

Create a new GreenBall script in the scripts folder and drag the script onto the prefab. Open the script in your IDE.

Add a documentation comment at the top of the class and make the \tt{GreenBall}GreenBall class a child class of the \tt{Ball}Ball class.

There are 3 important things to note about the \tt{Ball}Ball class:

 - The \tt{impulseVector}impulseVector field is protected so child classes can see it and change its value

 - The \tt{Start}Start method is virtual and protected so child classes can see it and override it

 - The \tt{PrintMessage}PrintMessage method is virtual and protected so child classes can see it and override it

We're going to make the green ball move up instead of left and print a different message.

Go back to the \tt{GreenBall}GreenBall class. Add the keywords \tt{override}override and \tt{protected}protected before \tt{void}void for the \tt{Start}Start method. In the \tt{Start}Start method, change the x and y components of the \tt{impulseVector}impulseVector field so the ball will go straight up. Add the following line of code next: \tt{base\!\!.\!\!Start\!\!();}base.Start();. This calls the \tt{Start}Start method in the parent class.

Delete the \tt{Update}Update method.

Override the \tt{PrintMessage}PrintMessage method to print a new message.

When the \tt{Start}Start method in the \tt{GreenBall}GreenBall class is called by the Unity engine, it sets the \tt{impulseVector}impulseVector field and calls the \tt{Start}Start method in the \tt{Ball}Ball class. That method gets the ball moving, then calls the \tt{PrintMessage}PrintMessage method that you overrode in the \tt{GreenBall}GreenBall class.

The calls to the \tt{Start}Start method and the \tt{PrintMessage}PrintMessage method behave in class-specific ways -- polymorphism in action!

### Problem 2 – Add red ball child class and prefab

Drag the sprite for the red ball onto the Hierarchy window, rename it to RedBall, and add a Rigidbody 2D component to it. Drag it onto the prefabs folder in the Project window to turn it into a prefab.

Create a new RedBall script in the scripts folder and drag the script onto the prefab. Open the script in your IDE.

Add a documentation comment at the top of the class and make the \tt{RedBall}RedBall class a child class of the \tt{Ball}Ball class.

We're going to make the red ball move left just like the ball does, but it will print a different message.

Delete the \tt{Start}Start and \tt{Update}Update methods.

Override the \tt{PrintMessage}PrintMessage method to print a new message.

When the \tt{Start}Start method in the \tt{RedBall}RedBall class is called by the Unity engine, it calls the \tt{Start}Start method that the \tt{RedBall}RedBall class inherited from the \tt{Ball}Ball class. That method gets the ball moving, then calls the \tt{PrintMessage}PrintMessage method that you overrode in the \tt{RedBall}RedBall class.

### Problem 3 – Add a ball spawner

Delete all the ball game objects from the Hierarchy window. Create a new BallSpawner script in the scripts folder and drag the script onto the main camera. Open the script in your IDE.

Add a documentation comment at the top of the class and add fields for the three ball prefabs and a spawn timer. Populate the prefab fields in the Inspector.

Add code to the \tt{Start}Start method to add a Timer component (put it in the field you just declared), set its duration to 1 second, and run it.

Add code to the \tt{Update}Update method to check if the spawn timer is finished. If it is, re-run the spawn timer and randomly spawn one of the 3 balls.

### Exercise Solution

[Exercise 5 Solution](https://d3c33hcgiwev3.cloudfront.net/_b5d188122552789ebdab489a7c45f2c2_2-2-Exercise-5-Solution.zip?Expires=1643068800&Signature=imNuDz0IJ4-3p-u5BdSPgLBa2NmwOhqPsW2dEbgDXJx1jXbBMk-LpS8fbqBMjCbGF69HHSu0Sn-P9M32Fv~VoUeg6lmryaVLgysGD-TTR2yAJ4dKSR7oiJW8kveoC6LrsHyuJaCuW~J~pwAieAlmLbz7rOO5G5M78Z9VO8UPEcQ_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
