# Exercise 7: The Bouncer

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 - Getting started

Create a new Unity project and save the current scene. Add Edge Collider 2D components to the camera on all 4 sides of the screen. Turn off gravity (in the game). Add a bouncy, no friction Physics Material 2D to all the edge colliders and the Bouncer's collider.

### Problem 2 - Bouncing is deadly

Implement a Unity class (script) called Bouncer that keeps track of its health and destroys the game object it's attached to when its health reaches 0 (or below 0). Reduce the health by 10 whenever the object collides with something. You'll also need to get your object moving by adding a force in the Start method.

Add a sprite for your Bouncer game object to your project, add the Bouncer game object to the game, and attach a Rigidbody2D, some collider 2D, and your Bouncer script as components to the game object.

When you run your game, your Bouncer should be destroyed when it hits an edge of the screen for the tenth time.

### Problem 2 - Fading away

Let's add some visual interest, where the game object fades a little on each bounce until its destroyed.

When you reduce the health, reduce the alpha value of the color for the SpriteRenderer by 0.1f also. You'll need to explore the SpriteRenderer and Color documentation to figure this out. The alpha component of a color is how opaque it is, with 1 meaning fully opaque and 0 meaning fully transparent.

Exercise Solution

[Exercise 7 Solution](https://d3c33hcgiwev3.cloudfront.net/Dv6O2mkVSdS-jtppFUnUJw_82978eccc90d400b9bfa4ebb153f1bf1_3-1-Exercise-7-Solution.zip?Expires=1643068800&Signature=jZQM8IehUqZ3a9qG9nBMkPy3isCz1gh7mAQGsB5qZTDM98Vio5OFHPZBFSCYxU7UvP8ReO-hj~qWuoJuLnAyNyz2GlCm1wemqOR-GWc5ibRo59UWtj6rzpVs~ks7L1ccn9~qIsUqAvVPJUhfH6~lRQTri3Od28Ukr4REM8HS4ns_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
