<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; exercise
# Parallax

The task is to create a parallax effect.

## 1
Study carefully the HTML and CSS code for this exercise. Note that there are three elements that will be moved at the same time. All of them are in the ```scene``` **div**.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded (remember that the exercise should be done in jQuery). Check if it works properly (e.g. by displaying the message "It works" in the console).

Create a function responsible for handling the parallax effect. Remember about appropriate comments and an appropriate name for the function.

Next, find the following elements and save them in variables:

1. ```scene``` container.
2. all elements with ```elements``` **class**.

Check if you have found the right elements and if their number is correct.

Display the variables in the console to ensure that they contain correct data.

## 3
Every element has three dataset attributes ```data```. In a loop (each), extract these elements and give them appropriate CSS values in the following way:

* value of the ```data-z``` field - set ```z-index```,
* value of the ```data-x``` field - set```left```,
* value of the ```data-y``` field - set ```top```.

## 4
Set ```mouseenter``` and ```mousemove``` events on the ```scene``` element. Check if they are called depending on their purpose.
At the beginning of the function you defined variables storing the scene and elements. Add two more variables in the same place that will store the mouse cursor position when entering the scene. You can call these variables ```oldMousePositionX``` and  ```oldMousePositionY```. Set the value of both to **0**.
In the place where you expect the mouse to enter (```mouseenter``` event) assign new mouse position values (```event.offsetX``` and ```event.offsetY```) to ```oldMousePositionX``` and  ```oldMousePositionY```.

## 5
The next step is to launch elements depending on the mouse movements (code inside the function for the ```mousemove``` event). Set two variables that will store the X and Y position of the mouse: ```currentMousePositionX``` and ```currentMousePositionX```.

## 6
Now we have to set the position of the mouse. First, make sure you did not accidentally move the mouse cursor over the element. Use  ```event.target``` and jQuery method: ```is```. If we move the mouse over the square, increase the current mouse position by the value taken from the CSS (for the ```left``` and ```top``` values &ndash; just extract them from the current ```event.target``` element). This way you will avoid "squares flickering".

## 7
Create two variables that determine the movement, e.g. ```mouseMoveX``` and ```mouseMoveY```. Save the difference between the current mouse position and mouse position when it entered the scene in those variables.

## 8
Within the function for the ```mousemove``` event, in a loop, set the ```left``` and ```top``` position of each square in relation to the value of ```speed```. Extract this value from the data attribute set in the HTML for each element. Calculate the said position in the following way:
* e.g. for the left position it will be: ```current left position + mouseMoveX * speed```,
* calculate the ```top``` position analogically.

## 9
Check how your site works. Can you see any problems? If so, describe them in a comment.
