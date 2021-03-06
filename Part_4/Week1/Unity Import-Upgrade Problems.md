# Unity Import/Upgrade Problems

### Asset Load Failure

When you try to open a project you created or that I provided, you may open scripts in Visual Studio and discover that Visual Studio doesn't seem to recognize any of the classes provided by Unity. If that happens, do the following:

 - In the Unity Editor, right click the Assets folder in the Project window

 - Select Reimport All

 - Click the Reimport button

This seems to resolve this problem for most people.

### Deterministic Compilation Problem

When you upgrade a Unity project from the version I've provided to the version you have installed, you may get an error message saying you should start in Safe Mode because deterministic compilation failed. If that happens, do the following:

 - Start Unity in Safe Mode

 - Select Edit > Project Settings

 - Select Player on the left

 - Scroll down in the pane on the right until you find the Enable Deterministic Compilation checkbox

 - Uncheck the checkbox

Unity will then continue loading the project and everything should work fine.

### Failed to Load Windows Layout Error

In some versions of Unity, when you try to load a project that you created previously or that I created for you, you get a "Failed to load window layout error." It's unclear where this Unity bug came from but here's a workaround that works in later than 2020.2 versions:

1. Press [Load Default Layout]

2. Unity copies the correct default layout to CurrentLayout-default.dwlt

3. Unity complains that it still cannot load the layout

4. Copy the now correct CurrentLayout-default.dwlt somewhere

5. Press Quit

6. Unity corrupts the file during quitting

7. Copy back the correct CurrentLayout-default.dwlt (into Library folder in project)

8. Start Unity again

      
