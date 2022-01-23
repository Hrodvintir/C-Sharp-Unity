# Exercise 11: The Loud Bouncer

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 - Getting started

Note: This exercise is Exercise 10 with a sound effect added. Download the solution to that exercise and use it as your starting point for this exercise.

### Problem 2 - Adding an audio clip and source

Add an audio folder to the Project window and copy an audio file (I used a short wav file) into the audio folder.

Select the Bouncer game object in the Hierarchy window and add an Audio Source component to it. Drag your audio clip from the Project window onto the AudioClip for the new Audio Source component. Uncheck the Play On Awake check box so the sound doesn't play when the Bouncer is added to the scene.

### Problem 3 - Playing the sound

Add a field to the Bouncer class to store a reference to the AudioSource component and initialize the field in the Start method.

Add code to the Bouncer OnCollisionEnter2D method to play the sound effect.

When you run your game, you should hear your sound effect every time the Bouncer hits an edge of the screen.

### Exercise Solution
[Exercise 11 Solution](https://d3c33hcgiwev3.cloudfront.net/CDiwFSd8T2m4sBUnfL9p3Q_85ee95cf6f5749c9a321987a67311df1_4-2-Exercise-11-Solution.zip?Expires=1643068800&Signature=lIzMMnh2GTrzzfJr3flkf98e2j~KYkq~ap4REOo2F8ultIzPThVeCt1Kkbf7MVpFHX8pB1TiLmX6~fS43MjS3fdqBAcUdT4K5PtZqGvdQ2rBO~fgvW7ktePF4xStZIrpRtTJupMpsJJyJ34ZSFX8sb0zR9PCQAUNDpt73fXz-5g_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
