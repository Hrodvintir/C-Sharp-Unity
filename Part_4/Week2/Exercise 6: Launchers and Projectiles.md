# Exercise 6: Launchers and Projectiles

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Getting Started

Download the zip file below and unzip the file somewhere on your computer.

[Exercise 6 Materials](https://d3c33hcgiwev3.cloudfront.net/_17192f9c0cc46adf6dcea3ba9bea641d_2-3-Exercise-6-Materials.zip?Expires=1643068800&Signature=gAYwYKc~wNZJHiLEw-4AUH-4zpJLfSDrB1sHV7OqBLhppm19cPRJMEQQChbg16Pry97f9bNjDTqg1Hr9YnyCMNyVjp7KDbRH7nVSKQHjWT3EJA-JtsNt~rOZIYQbrOtEUu3E82JUk2rjTXEyoMUphGFcFrp01dwigfosB6rFBUg_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

Open the project in Unity. You can do this by navigating to the Exercise6\Assets\scenes folder and double clicking scene0.

Look at the Launcher and Projectile scripts; those are the roots of the launcher and projectile class hierarchies. Look at the ChainsawLauncher and ChainsawProjectile scripts to see how those child classes implement the initial functionality. Note that I selected the ChainsawLauncher prefab, then populated the \tt{prefabProjectile}prefabProjectile field in the Inspector by dragging the ChainsawProjectile prefab from the Project window onto that field.

### Problem 1 – Add pirate launcher and projectile

Use the pirate launcher and projectile sprites to create PirateLauncher and PirateProjectile prefabs. Be sure to add a Rigidbody2D component to the PirateProjectile prefab. 

Make sure you set the Sorting Layer in the Sprite Renderer component of those prefabs to Launcher and Projectile, respectively. This makes sure the projectile is rendered under the launcher, which looks better as the launcher fire projectiles.

Create PirateLauncher and PirateProjectile scripts and edit them to make the launcher firing rate twice as fast (cooldown half as long) as the ChainsawLauncher and the impulse force for the projectile 3 times as strong as for the ChainsawProjectile. 

Add a PirateLauncher prefab to the Hierarchy window and run the game to make sure your implementation works correctly.

### Problem 2 – Add zombie launcher and projectile

Do what you did in the previous step, this time adding a zombie launcher and projectile. Make the launcher fire twice as fast as the pirate launcher and make the impulse force for the projectile 3 times as strong as for the pirate projectile (brains go really fast <grin>).

Add a ZombieLauncher prefab to the Hierarchy window and run the game to make sure your implementation works correctly.

### Problem 3 – Add a launcher spawner

Delete all the launcher game objects from the Hierarchy window. Create a new LauncherSpawner script in the scripts folder and drag the script onto the main camera. Open the script in your IDE.

Add a documentation comment at the top of the class and add fields for the three launcher prefabs and a spawn timer. Populate the prefab fields in the Inspector. You'll probably also need other fields to implement the behavior described below.

Add code to the \tt{Start}Start method to add a Timer component (put it in the field you just declared), set its duration to 5 seconds, and run it.

Add code to the \tt{Update}Update method to check if the spawn timer is finished. If it is, re-run the spawn timer and spawn the appropriate launcher. Here's the required spawn order: ChainsawLauncher, PirateLauncher, and ZombieLauncher. Once all 3 launchers are spawned, don't spawn any more launchers.

When you run your code, be patient; it will be 5 seconds before the chainsaw launcher is spawned.

### Exercise Solution
  
[Exercise 6 Solution](https://d3c33hcgiwev3.cloudfront.net/_b3c73de4d92ebb791609ff3d195a7eab_2-3-Exercise-6-Solution.zip?Expires=1643068800&Signature=csVnpBg-qwngDS~ZgEWpWJMjU3x-THAFqwe9wnlozgzCqKrcHZXlyorp-QQitiUle9k-SJdIi~27uknxSfQkkvqcgEr2FNc5R8t8YDcONx3FWTDK9an4dIUt8Ni9lhuKp8VTB7pIiu1CX8rZc9GuGEzmEhjNbZyc9nnmRr562eg_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
