<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; exercise
# Forms

Create a script validating form fields and sending data to the following address: [http://api.coderslab.pl/showpost.php](http://api.coderslab.pl/showpost.php)

## 1
Study the HTML code for this exercise.
In an appropriate attribute of the ```form``` element, add an addresswhere you want to send the form.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded (remember that the exercise should be done in jQuery). Check if it works properly (e.g. by displaying the message "It works" in the console).

Create a function responsible for handling the form. Remember about appropriate comments and an appropriate name for the function.

Next, find the following elements and save them in variables:

1. The form.
2. Each form field (in separate variables).
3. The **div** element that will display errors if the user writes something incorrectly.

Check if you have found the right elements and if their number is correct.

Display the variables in the console to ensure that they contain correct data.

## 3
Add a ```submit``` event to the form that will react to a mouse click. Pass the caught event to the callback function. Block the default action of the submit event (do you remember the ```event.preventDefault()``` function?)

## 4
When the ```submit``` button is clicked, the following should happen:

1. Save values entered by the user into the form fields in variables (Do you remember how to extract data from the input field?)
2. Check every value entered by the user in the following way:
  * name must be longer than five characters,
  * email must contain ```@``` sign and a dot ```.```,
  * message must be longer than 10 characters.

If any of these values is incorrect, display an appropriate message in the **div** with ```error``` **class**.

## 5
Check how your site works. Can you see any problems? If so, describe them in a comment.
