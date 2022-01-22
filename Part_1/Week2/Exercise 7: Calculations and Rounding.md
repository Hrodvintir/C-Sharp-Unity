# Exercise 7: Calculations and Rounding
Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Temperature Conversions

In this exercise, you'll be converting temperatures from Fahrenheit to Celsius and back again.

To convert from Fahrenheit to Celsius:

 - Begin by subtracting 32 from the Fahrenheit temperature.

 - Divide the answer by 9.

 - Finally, multiply by 5 to get the Celsius temperature.

To go convert Celsius to Fahrenheit:

 - Begin by multiplying the Celsius temperature by 9.

 - Divide the answer by 5.

 - Finally, add 32 to get the Fahrenheit temperature.

### Problem 1 – Temperature Calculations with Int

Create a new 2D Unity project named Exercise7. Rename SampleScene to Scene0. Add a Scripts folder and add a new C# script named ConvertTemperatures. 

Open the script, fill in the comment near the top of the script, and delete the Update method. Add the following code to the Start method:

 - Declare three int variables to store an original temperature in Fahrenheit, a calculated temperature in Celsius, and a calculated temperature in Fahrenheit (when you convert from Celsius back to Fahrenheit).

 - Assign 0 as your original temperature in Fahrenheit and print that Fahrenheit value, convert to Celsius and print the Celsius value, then convert the Celsius value back to Fahrenheit and print the Fahrenheit value. Be sure to label each of your outputs rather than just printing out the numbers.

 - Assign 32 as your original temperature in Fahrenheit and print that Fahrenheit value, convert to Celsius and print the Celsius value, then convert the Celsius value back to Fahrenheit and print the Fahrenheit value. Be sure to label each of your outputs rather than just printing out the numbers.

 - Assign 212 as your original temperature in Fahrenheit and print that Fahrenheit value, convert to Celsius and print the Celsius value, then convert the Celsius value back to Fahrenheit and print the Fahrenheit value. Be sure to label each of your outputs rather than just printing out the numbers.

Attach the script to the Main Camera in the scene and run the game to see the output in the Console window.

You'll discover that the conversion from 0 to Celsius and back to Fahrenheit yields 5, not 0, for the final Fahrenheit temperature. That's one of the points of this exercise! Think about the data type you used and why you might get this result given that data type.

### Problem 2 – Temperature Calculations with Float

Add the following code to the Start method after the code you already added:

 - Declare three float variables to store an original temperature in Fahrenheit, a calculated temperature in Celsius, and a calculated temperature in Fahrenheit (when you convert from Celsius back to Fahrenheit).

 - Assign 0 as your original temperature in Fahrenheit and print that Fahrenheit value, convert to Celsius and print the Celsius value, then convert the Celsius value back to Fahrenheit and print the Fahrenheit value. Be sure to label each of your outputs rather than just printing out the numbers.

Now the conversion from 0 to Celsius and back to Fahrenheit is closer to 0, but it’s still not exactly 0. Remember, even though floating point numbers are approximations of the real numbers in the continuous domain, they give us more precision than whole numbers do. That's why we got a closer final Fahrenheit temperature when we used float variables instead of int variables.

### Problem 3 – Temperature Calculations with Double

Add the following code to the Start method after the code you already added:

 - Declare three double variables to store an original temperature in Fahrenheit, a calculated temperature in Celsius, and a calculated temperature in Fahrenheit (when you convert from Celsius back to Fahrenheit).

 - Assign 0 as your original temperature in Fahrenheit and print that Fahrenheit value, convert to Celsius and print the Celsius value, then convert the Celsius value back to Fahrenheit and print the Fahrenheit value. Be sure to label each of your outputs rather than just printing out the numbers.

Finally, the conversion from 0 to Celsius and back to Fahrenheit yields a 0 as you probably originally expected. Because the double data type uses more bytes than the float data type, we don’t get the rounding error we got when we used floats.  

This exercise shows how data type really matters, especially when we do multiple calculations.

### Exercise Solution - iCloud
