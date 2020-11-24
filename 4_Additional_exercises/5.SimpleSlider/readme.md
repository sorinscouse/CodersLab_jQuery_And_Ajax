<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; exercise
# SimpleSlider

Write a simple slider. The task is divided into sections. Stick to the instructions and do them one by one.
Remember to make a commit when you have finished the exercise.


## 1
Study the HTML code for this exercise. To create a slider, we usually style a list that stores images.
Therefore, when you have added ```slider``` **class** to an appropriate element, do the following in the **style.css** file:

1. Place the list elements side by side. As you can see, not all pictures are next to each other. Therefore, it is necessary to set such width for the outer container (**ul**) that will make all images fit side by side. We will do it in jQuery later but for now, try to set container width in the **style.css** so that all the pictures fit. Do it only to test how the elements will align. After testing, you can remove this width from the css file.
2. Reset margin and padding of the **ul** element to zero (do you remember that the browser gives default styles to some elements?)
3. Set the width of the container above the **ul** element to the width of a single image and set the property ```overflow: hidden``` for it.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded (remember that the exercise should be done in jQuery). Check if it works properly (e.g. by displaying the message "It works" in the console).

Create a function responsible for the entire gallery animation. Remember about appropriate comments and an appropriate name for the function.

In the function that you have written, find the following elements and save them in variables:

1. `Next` button.
2. `Prev` button.
3. All list elements (save them in an array).
4. Add a numeric variable that will determine the index of the visible image (At first, it will be the first image &ndash; the variable will point to **0** index).
5. Add another variable that will store the width of a single image. You will need it in a moment to set the width of the **ul** container with all the images (using jQuery, not CSS).

Check if you have found the right elements and if their number is correct. Display the variables in the console to ensure that they contain correct data.

## 3
In the function, set the height of the **ul** container based on the data stored in your variables, so that all images fit side by side (remember to remove the container width from **style.css**).

## 4
Add a mouse click event to the `Next` button (do not use loops &ndash; you are working in jQuery).
For now, the event should display any text in the console.

## 5
Modify the event so that, after the button is clicked, it:

1. Increases the value of the variable that stores image index.
2. Makes sure that the variable does not exceed the number of images.
3. If everything is in order, animate movement of a slide (use the ```left``` property). Remember that the element that you move (**ul**) needs to have ```position: relative``` in CSS. Think about what direction you want to move in.

## 6
Add another event for the `Prev` button. Follow the same steps as for the `Next` event. Just remember about the condition that the variable with image index has to meet, and about the direction of movement. You should still use the ```left``` property.

## 7* (for volunteers)
Try to create one more function that will be responsible for moving the slide after clicking any button. Consider what parameters should be passed to the function. Set an appropriate name for it and a comment.

## 8
Check how your site works. Can you see any problems? If so, describe them in a comment.
