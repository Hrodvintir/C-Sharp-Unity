# Exercise S7: The Bouncer

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

### Exercise Solution

[Exercise S7 Solution](https://d3c33hcgiwev3.cloudfront.net/xwbaJyAyTiiG2icgMr4o7A_414a1bdcd25548248a9d18a7344488f1_5-4-Exercise-S7-Solution.zip?Expires=1643155200&Signature=cCB6D6pMqcRnISredE53K824ZoXMueYx-y0be2EU-nyQG4zBF0cIqx8fLOsHS-bo3PliYBg152Li70fOkONQCHPNfkzgR3lvfT-pw4LSgJns~k8VCof7tXz0LCqyfdZI4~7bRjiPo94oSTyPqZpCTM7eEVrHTNkBL6HPbV422jg_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
