# Exercise 7: Is There Anybody Out There?

Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.  

### Problem 1 – Add events

Create a new Unity project named Exercise7 and rename SampleScene as scene0.

Create a script named MessageEvent for an event that inherits from the \tt{UnityEvent}UnityEvent that doesn't have any arguments. The script will be printing messages to the Console window. Remember, \tt{UnityEvent}UnityEvent is in the \tt{UnityEngine.Events}UnityEngine.Events namespace.

### Problem 2 – Implement event handling

Create an Invoker script. Copy one of the Timer scripts we've been using into the project. Declare fields for a timer and a no argument event object. Add an \tt{Awake}Awake method that creates an instance of the event object in your new field. Add a public \tt{AddNoArgumentListener}AddNoArgumentListener method that adds a no argument UnityAction delegate as a listener; remember, \tt{UnityAction}UnityAction is in the \tt{UnityEngine.Events}UnityEngine.Events namespace. Add code to the \tt{Start}Start method to add a Timer component, set its duration to 1 second, and run the timer. Add code to the \tt{Update}Update method to invoke the event and run the timer again after it's finished. 

In the Unity editor, attach the Invoker script to the main camera.

Create a Listener script. Add a no argument method that prints a message of your choice. In the \tt{Start}Start method, add code to get access to the Invoker class (by getting the Invoker component from the main camera) and add your no argument method as a listener.

In the Unity editor, attach the Listener script to the main camera.

Run the game. The message should be printed in the Console window every second.

### Exercise Solution

[ Exercise 7 Solution](https://d3c33hcgiwev3.cloudfront.net/azaKQ2apQ0O2ikNmqUNDXA_cb4824d02dff45df888654886327b5cf_3-1-Exercise-7-Solution.zip?Expires=1643068800&Signature=QvZXrTeO7070eHCqlpcYur4iaeP1oIGWPwxTEIW9OsHmk2LP49lm6u6Hp8UMJ6VimQOqiSPPhZjnA-tljlNlY525-RD2mRg1dOuRRvYAEIiu~8l5~7EuFFycgc~XUx5BqbnQZ1KKLHvAzeDJbtG6sY4wNR76~xHYXbRM-F8xewM_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)
