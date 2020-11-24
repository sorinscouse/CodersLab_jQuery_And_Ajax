<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; exercise
# Tabs

Write a simple tab scheme.
The important thing is that the number of tabs and of messages assigned to them must be equal.
Remember to make a commit when you have finished the exercise.

## 1
Take a look at the HTML and CSS code for this exercise. All tab headers are stores in a list. Matching texts are in **div** elements.
Check the **style.css** file and set an appropriate **class** for the parent: **ul**.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded. Test your code (e.g. by displaying the message "It works" in the console).

## 3
Find the following elements and save them in variables:
1. All list elements corresponding to tabs.
2. All **divs** corresponding to texts.

Check if you have found the right elements and if their number is correct.

List the variables in the console to ensure that they contain correct data.

## 4
Add an event to all tabs that will react to a mouse click (do not use a loop - remember that you are working in jQuery).
Przetestuj (np. poprzez wyświetlenie w konsoli napisu "Działa").

## 5
Modify the event so that when a **li** is clicked, the **div** text assigned to it showed on the page (for a nice effect, you can use an animation).
Use the variable pointing to the clicked tab to find the **div** with text that was assigned to it. Remember that those tabs that were not clicked, should not be displayed.

## 6
Check how your site works. Can you see any problems? If so, describe them in a comment.
