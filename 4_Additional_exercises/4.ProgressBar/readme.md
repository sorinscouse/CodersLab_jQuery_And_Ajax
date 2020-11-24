<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; exercise
# Progress Bar

Animate the **span** element so that it simulates a progress bar when an appropriate button is clicked.
Remember to make a commit when you have finished the exercise.

## 1
Study the HTML and CSS code for this exercise. The first step is studying the **index.html** carefully and modifying it.
Each **div** with ```progress-bar``` class has three buttons assigned. The content of the element will suggest what attributes you should set for the **button** element. Use the data attribute with appropriate suffixes, e.g. note that the animation of the first bar should go as far as **50%** of its width so one of the data attributes will have the suffix ```-width```.

You need two more attributes:
* one that will store the number of progress bar,
* second one that will set the color.

You have a CSS file ready, take a close look at it as well.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded (remember that the exercise should be done in jQuery). Check if it works properly (e.g. by displaying the message "It works" in the console).

Create a function responsible for animating the progress bars. Remember about appropriate comments and an appropriate name for the function.

Find the following elements and save them in variables:

1. All buttons.
2. All **div** elements that simulate progress bars.

Check if you have found the right elements and if their number is correct.

Display the variables in the console to ensure that they contain correct data.

## 3
Add an event to all buttons reacting to a mouse click (do not use loops &ndash; you are working in jQuery).
For now, the event should display any text in the console.

## 4
Modify the event so that, after a button is clicked, it:

1. Saves all data attributes in variables,
2. determines which progress bar (**div**) is assigned to the clicked button,
3. You know what the user clicked and which progress bar you want to animate - now, assign ```span``` element (within the **div**) to a variable.
4. Give an appropriate class with color to the chosen progress bar. Also, animate the change of its width based on the values extracted from data attributes.

## 5
Check how your site works. Can you see any problems? If so, describe them in a comment.
