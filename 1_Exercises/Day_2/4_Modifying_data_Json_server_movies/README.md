<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Modifying the data

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.


## Exercises to do on your own

# Exercise 1 (5min)

Install and run json-server.
In the catalog, you will find a ```movies.json``` file with a movie database that we will use.

Add jQuery to the file, and download all elements that you will work on in the script (form, inputs and list).


# Exercise 2 (~ 15min - 30min)

Create a ```loadMovies()``` function that will load the data from the server using Ajax.
After the data is loaded, display it in the console. Initiate a function named ```insertMovies(movies)``` that you will write in a moment. Pass the loaded data to this function.


# Exercise 3 (~ 15min - 30min)

* Create a ```insertMovies(movies)``` function that you will pass the data loaded in the previous exercise. This function will iterate through the data in a loop, create new li elements, and append them to the list on the page. See the example of a single li element:

```
<li class="movie">
    <div class="movie-content">
        <h3 class="movie-title">Movie title</h3>
        <p class="movie-description">Movie description</p>
    </div>
</li>
```

To create the code for a single li element you can use [template strings](https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/template_strings) or create appropriate elements individually and append them to the created li element.


# Exercise 4 (~ 15min - 20min)
Create ```addMovie(title, description)``` function that will add a new movie to the database using Ajax. Pass appropriate parameters to it, make a connection with an appropriate method in which you will send movie title and description. You do not have to sent the ID - it is generated automatically by the database.
After the data is sent to the server, you can launch the ```loadMovies()``` function to load the list with the newly added film.

In the next step, outside the addMovie function, modify the submit event of the form (to prevent its default action). In this event, download data from form fields, then run the ```addMovie (title, description)``` function passing the appropriate data to it.


# Exercise 5 (~ 15min - 20min)
The task is to remove a movie from the database. This will work analogically to the previous exercises:
* create a ```removeMovie(id)``` function that will create Ajax connection. When the connection is closed, you will call the ```loadMovies()``` function to refresh the movie list. Remember that if you want to remove a movie with **id=2**, you sent a request with the DELETE method to the address http://localhost:3000/movies/2.
* return to the function from exercise 3 (the one creating li) and modify it so that it adds a ```Delete``` button with ```.btn-delete``` class at the end when creating a new li element.
* Outside of this function (preferably under the submit event that was written above), add a new element for all Delete buttons. New li elements will be created dynamically so you can work on them directly here. Ude the knowledge obtained in the "Advanced events" section.
* After the button is clicked, you should call the ```removeMovie(id)``` function passing to it the **id** of deleted movie. Where should you get the id from? When creating new li elements, you can add a **data-id** attribute to each of them, and assign to it the values taken from the data returned when loading movies (just like you insert the title and description). When clicking on the button, you should download this li (it is the parent of the button) and retrieve its ```data-id``` attribute.


# Exercise 4 (~ 20min - 25min)
Modify the movie on the server. In order to do this:
1. Create a function named ```updateMovie(id, title, description)``` that will create Ajax connection and send data to the server using the PUT method. The data should be ssent to an appropriate address - just like when removing a movie.
2. Return to the function from exercise 3 and modify it so that it adds a ```Modify``` button with ```.btn-edit``` as well when creating a new li element.
3. Analogically to ```.btn-delete``` buttons, add a new click event to ```.btn-edit``` buttons.
4. When a single ```.btn-edit``` button is clicked, do the following:
  - save the nerest li (parent of the button) in a variable
  - save the ```id``` of a given movie in a variable
  - turn on or off the ```editable``` class for this li. Use the [toggleClass()](http://jqapi.com/#p=toggleClass) function.
  - in the next step, check whether the given li has the ```editable``` class or not. Depending on the result, you will turn the edit mode on or off.
  To do this, in an if statement, check if the given li has the ```editable``` class. Use the jQuery function [hasClass()](http://jqapi.com/#p=hasClass)
    - if li has the editable class:
      1. download the title and description of the movie and save in variables
      2. change the title to text input with ```.movie-title``` class and value that you have just downloaded. Use  [replaceWith()](http://jqapi.com/#p=replaceWith) function
      2. change the description to text input with ```.movie-description``` class and value that you have just downloaded.
      3. change the text on the button to ```Save```
    - if li does not have the editable class:
      1. download the title and description of the movie and save in variables (they are text fields this time!)
      2. change the title to h3 with ```.movie-title``` class and the text that you have just downloaded. (http://jqapi.com/#p=replaceWith)
      2. change the description to a div with ```.movie-description``` class and text that you have just downloaded.
      3. change the text on the button to ```Edit```
      4. run the ```updateMovie(id, title, description)``` function that you wrote, and pass the downloaded data to it.
