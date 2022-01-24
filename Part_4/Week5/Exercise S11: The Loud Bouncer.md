# Exercise S11: The Loud Bouncer

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

[Exercise S11 Solution](https://d3c33hcgiwev3.cloudfront.net/ialFQIuqSm-pRUCLqspvMA_ff5fddabf7d44b91b9626f10ebb89ef1_5-6-Exercise-S11-Solution.zip?Expires=1643155200&Signature=WJj8t0RfH~qJxBLZwVV2oPiDdNh6vKaEsoOsH~D4epK4wZRsCXm32hjfmEuRu6DVKu3h7a1A9Ct2Td96V530V1oMtsv2wyadGQR4y41VwQpUeo33c8g0RgXaM8Iz7GceH16eEFbHzuiZ6WAl84AwR4Aavh0QFuL4m22nAmVOCA0_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
