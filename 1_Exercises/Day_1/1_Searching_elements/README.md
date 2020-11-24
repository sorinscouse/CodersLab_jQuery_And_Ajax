<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Searching for elements

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.


## Exercises done with the lecturer

### 1  (~ 2min - 5min)
Add the jQuery library to your file. In **app.js**, place code that will check if DOM contents were loaded.
Ten, find all ```section``` elements and give them ```section``` **class**. Create a new function where you will perform these activities.

### 2 (~ 2min - 5min)
Find the ```body``` element and set its background color to ```#eee```.

-------------------------------------------------------------------------------

## Exercises to do on your own

### Exercise 1 (~ 5min - 10min)

Take a look at **index.html** and appropriate CSS files.
Find the **ul list** in the section with **.section-menu** class. Add the **.menu** class to this list, and add ```menu-element``` class to each li element of this list.

### Exercise 2 (~ 5min - 10min)

In the section with ```section-main``` class, give two additional **classes** to each **li** elements:
* ```main-element-bg```,
* ```main-element-color```.

### Exercise 3 (~ 5min - 10min)

In the section with  ```section-links``` class, find all links. Then:

1. Add ```links-element``` class to them
2. Give the first link in this section the ```links-element-first``` class
3. Give the last link in this section the ```links-element-last``` class
4. Give the fifth link the ```links-element-active``` class


### Exercise 4  (~ 2min - 3min)

Find the element with the ```shape``` id.
- Add it the ```shape-star``` class.
- Add ```shape``` and ```shape-circle``` classes to the previous element.
- Add ```shape``` and ```shape-square``` classes to the next element.


### Exercise 5  (~ 5min - 7min)

Find the element with the```counter``` class. Hide its second, third, and fourth child. Use one of the following functions:
[hide()](http://jqapi.com/#p=hide), [slideUp()](http://jqapi.com/#p=slideUp) lub [fadeOut()](http://jqapi.com/#p=fadeOut)


### Exercise 6  (~ 5min - 7min)

In ```index.html``` you will find a link with the ```codersLink``` id. Save its href attribute in a variable and write it in the console. Then, replace it with another value of your choice :)


### Exercise 7  (~ 5min - 7min)

Find the element with the ```form``` class.
There are two **input** fields in it.
Extract their values (individually) and display them in the console.
Now, try to extract these values with the [each()](http://jqapi.com/#p=each) loop.
