<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; Exercise
# Sticky menu

Write a **sticky menu** - a menu that sticks to the top edge of the screen while scrolling.
Remember to make a commit when you have finished the exercise.

## 1
Study the HTML and CSS code for this exercise. The menu is placed in a list.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded and check if it works properly (e.g. by displaying the message "It works" in the console).

## 3
Find the following elements and save them in variables:

1. **nav** that you will need to prevent unwanted upward movement of the content when the menu drops down. The height of the element is already set in **style.css**.
2. **ul** with ```menu``` **class**.
3. Variable that will store the position (top) of the element with the ```menu``` **class**.

Check if you have found the right elements and if their number is correct.

Display the variables in the console to ensure that they contain correct data.

## 4
Set an event on the **window** element that reacts to scrolling. Check if it works.

## 5
When scrolling, check when the menu should stick to the top bar. Extract the the number of pixels by which the entire ```document``` item has been scrolled (```scrollTop```) and save it in a variable.
Then, compare this value to th eposition of the menu. If the document distance is greater than the menu distance, add ```sticky``` **class** to the menu. Otherwise, remove this class.

## 6
On ```window```, set another event reacting to the change of window width. Check if it works.

## 7
When changing the window width, the distance of the menu from the top bar will change. To take care of this, we created the ```resize``` event.
You need to check the distance for the menu again. Create a condition that will check this distance (if the menu item has ```sticky``` **class**) and assign it to the same variable as before. Otherwise, get the distance from the top bar for the **nav** element.

## 8
Check how your site works. Can you see any problems? If so, describe them in a comment.
