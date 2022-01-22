# Exercise 9: Look at the Cards
Although this exercise isn't worth any points, it gives you valuable programming experience. You're almost definitely going to have to complete the exercises to succeed in the course.

### Getting Started

Download one the zip file below and extract the file somewhere on your computer. 

*Exercise 9 Materials - iCloud*

Double-click the index file in the Help folder and click the Exercise9 link in the pane on the left; this is the documentation for the classes I provided to you in the Exercise9 solution. Note: You can't open the index file from within the zip file, you need to open it in the extracted (unzipped) location.

Open the Exercise9 solution in Visual Studio.

### Problem 1 - Create a deck and tell it to print itself

Declare a deck variable and use the Deck constructor to put a new Deck object into the deck variable.

Tell the deck to print itself. Use the help documentation I provided to figure out which method to use.

### Problem 2 - Tell the deck to shuffle and print itself

Tell the deck to shuffle itself and print itself. Use the help documentation I provided to figure out which methods to use.

### Problem 3 - Take two cards from the deck and print their ranks and suits

Take a card from the top of the deck and print its rank and suit. Use the help documentation I provided to figure out which Deck method to use to get the top card and which Card properties to use to print the rank and suit.

Take another card from the top of the deck and print its rank and suit.

Hint 1: The Card class doesn't expose a Print method, so you have to access a card's properties to print the required information. 

Hint 2: You haven't called a method that returns a value yet. Here's a good way to do that for this exercise:

Card card0 = deck.TakeTopCard();

The Deck TakeTopCard method returns a Card object. You need to save that object in a variable so you can access its properties.

Exercise Solution - iCloud
