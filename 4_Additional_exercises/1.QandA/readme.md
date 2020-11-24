<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery &ndash; exercise
# Questions and Answers

Write a simple question and answer scheme. Ultimately, the answers should be invisible. They should appear only after the question was clicked. Remember to make a commit when you have completed the exercise.

## 1
Take a look at the HTML and CSS code added to the exercise. All questions and answers are in a **div** which you should give the right class.

## 2
Prepare the JavaScript file so that you can work in it. Add an event that will check if DOM elements are loaded. Test it (e.g. by displaying the message "It works" in the console).

## 3
Find the following elements and save them in variables:

1. All questions (**h1** elements).
2. All answers (**p** elements).

Write these variables in the console to make sure that they contain appropriate data.

## 4
Add an event to all **h1** elements that will react to a mouse click (do not use a loop &ndash; remember that you are working in jQuery). Test your code (e.g. by displaying the message "**h1** was clicked" in the console).

## 5
Modify the event so that when **h1** is clicked, a neighboring **p** element showed on the page (use an animation of your choice). If an element is already visible, hide it.

## 6
Write code that will make only one answer visible on the screen &ndash; the clicked one.
To get such effect, in the event, write code that will cause all paragraphs to disappear (all besides the one assigned to the clicked question). Behavior of the paragraph assigned to the question does not change.

## 7
Check how your site works. Can you see any problems? If so, what problems? Write in a comment.
