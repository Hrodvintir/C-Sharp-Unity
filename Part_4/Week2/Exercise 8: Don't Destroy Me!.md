# Exercise 8: Don't Destroy Me!

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Problem 1 – Create project and add event manager

Create a new Unity project named Exercise8 and save the default scene into a new scenes folder.

Add a DestroyButton script (you'll use this in Problem 3, but you need the class now to use in the event manager). Add a stub for an \tt{AddDestroyEventListener}AddDestroyEventListener method to the script; your stub should be the entire method without any code in the method body.

Add a static \tt{EventManager}EventManager class that has static fields for an invoker and a listener for a no argument event. Add public static methods to add an invoker and to add a listener for that event. Remember, you don’t know in what order those methods will be called, so when you add the invoker you should also add the listener to the invoker (if the listener isn’t null). You should also do this when you add a listener (if the invoker isn’t null);

### Problem 2 – Add a game object that listens for the event

Add a game object to the scene. Have the game object’s script add itself as a listener for theDestroyEvent to the event manager in the script’s \tt{Start}Start method. Have the script destroy the game object it’s attached to when the event is invoked.

### Problem 3 – Add a menu button that invokes the event

Add a DestroyEvent class for a no argument UnityEvent.

Add a menu button that invokes the event to the scene when it’s clicked. Have the DestroyButton script add itself as an invoker of the DestroyEvent to the event manager in the script’s \tt{Start}Start method. Have the script invoke the event when the menu button is clicked.

### Exercise Solution

[Exercise 8 Solution](https://d3c33hcgiwev3.cloudfront.net/o9qMcGz6RQ6ajHBs-vUORw_f28aff218f034ac6a67ce4e53af8f213_3-2-Exercise-8-Solution.zip?Expires=1643068800&Signature=RwxwMF1s68wFAiORPJ--tte6gZLvxcDHjcpTj93X1qjEoeoRCj5ZW1Z-K-oXItMT5H70vgFojz3QZmXCoiLm1ZEFPkZY4P1vpz-BgdNJjrEoE4BAAppyqh0GW4Chaqt8B0O2uGbUuD4ccCdTEotI6fmanWr6quqj3YVQCjmfkWs_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
