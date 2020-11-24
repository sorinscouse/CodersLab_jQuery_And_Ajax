<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Modifying elements

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.

## Exercise done with the lecturer

### Adding (~ 5min - 7min)

Create a ```div``` element with the ```info``` **class** and insert it above the ```section-users``` element. Using jQuery, add any text you want to it - e.g. "Let's start the exercises!".

-----------------------------------------------------------------------------------------------------

## Exercises to do on your own

### Exercise 1 (~ 15min - 20min)

In **index.html**, find the element with ```section-users``` **class**. Extract all elements that you will work on:
- form
- inputs
- user list.

Add a ```submit``` event to the form. Do the following steps in the event:

1. Block the default action for the form.
2. Extract input values and assign them to variables.
4. Place a new element at the end of the list; set age as the ```data-age``` attribute.
5. Clear inputs by setting their values to empty strings.
6. Add a condition that will prevent adding new users if appropriate fields are not filled.

Write a function (NOT inside the submit event) that will extract li elements from the user list. Then, in an **each** loop, the function should give each li the ```color-white``` class and color all **li** as follows:
  * for people under 15 - **#75D701**,
  * for people aged 16 to 40 - **#f9c00c**,
  * for people aged 41 and above - **#c03546**.
Initiate the function after the new li is added to the list.

### Exercise 2 (~ 7min - 10min)

Take a look at **index.html**. Find elements with ```panel-left``` and ```panel-right``` classes in it. Within those elements, find li elements with ```list-element``` class.

Write a function that will move a clicked element with ```list-element``` **class** to the column with the ```panel-right``` **class**.
Try to add a feature that will move such element from the left column to the right and the other way round (a hint: - you can check the parent of the element at the time of clicking).
