<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Events

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.


## Exercises done with the lecturer

### Moving the mouse cursor over and out of an element  (~ 7min - 12min)
Place an event on the **dt** element that displays in the console information about the element that we moved the mouse over to.

### Extracting data values  (~ 10min - 15min)
In **index.html**, find three **buttons** in the element with the ```hero-buttons``` **class**. Do the following:
* set a ```click``` event for each element that will extract value from the data-feature attribute after clicking the element, and will display this value in the console.

-------------------------------------------------------------------------------

## Exercises to do on your own

### Exercise 1 (~ 10min - 15min)

In **index.html**, find a **section** with ```superhero-description``` **class** and write a function that will:
1. hide all **dd** elements by default.
2. When **dt** is clicked, make **dd** elements:
* appear if they were hidden,
* disappear if they were visible.
* to find the nearest siblings of a given element, use the .next() function.

### Exercise 2  (~ 10min - 12min)

In **index.html** find the element with ```shopping-list``` **class** and buttons within it. When a button is clicked, do the following:
* Give the button's parent the ```added``` **class**,
* Set the following properties in the clicked button:
  - background: #0080ff;
  - color: #fff;
* Replace the text on the button with ```Added```.
* When the button is clicked again, reset the settings of the ```shopping-list-item``` element.
