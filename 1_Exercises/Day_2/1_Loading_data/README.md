<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Loading data

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.

## Exercise **discussed** with the lecturer (~ 15min - 20min)

Take a look at HTML and JavaScript files. The task is to load data from the following address: https://swapi.co/api/films/
Go through this task using the **debugger**. Note when is the data loaded?

Useful information:
* use an appropriate HTTP method if necessary,
* use appropriate functions that inform the user about the status of his request (```done()```, ```fail()``` methods),
* check in the console what the loaded data looks like. Is it an array, a string, or JSON?
* if the data are correctly loaded, call an appropriate function, e.g. ```insertContent()```, and pass it the loaded data as a parameter,
* within the ```insertContent()``` function, iterate through the array with results using a loop,
* inside the loop, create **li** elements where you will insert movie titles, and append them to the **ul** list.
