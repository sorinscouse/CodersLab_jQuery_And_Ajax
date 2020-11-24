<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Advanced events

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.

## Exercise done with the lecturer

### Hiding  (~ 5min)

Extract from **index.html** all elements that you will work on:
- form
- inputs
- list.

Add ```submit``` event to the ```form``` element. The event will:
- prevent the default action of the form,
- collect data from the form,
- create a new li element and add it at the end of the list with ```user-list``` class.

Below the submit event (not within it), add an event to **Delete** buttons that will delete a given li element. You can use the code below:

```
$(".btn-delete").on("click", function() {
    $(this).parent("li").slideUp(function() { //hiding li element
        $(this).remove(); //removing li element
    });
});
```

As you can see, the above code does not work properly. The initial li elements are removed, but those added by the form - era not.
Try to correct the code so that the removal works equally for all elements.

-----------------------------------------------------------------------------------------------------

## Exercises to do on your own

### Exercise 1 (~ 20min - 25min)

* Add an ```Edit``` button to each li with ```btn-edit``` class (preferably before the ```btn-delete``` button),
* write a function that will enable element editing when the ```Edit``` button is clicked.
During editing, change the name of the button from ```Edit``` to ```Confirm```. End editing when ```Confirm``` is clicked.

A challenge for volunteers: during editing, you can try to change **span** to **input:text** that will have an appropriate value, and after editing the input, change it back to span.
Use knowledge obtained in previous exercises (2_Events->Exercise 2) and the jQuery method [replaceWith](http://jqapi.com/#p=replaceWith)

Sample code that you can use here:
```
//if the field is a text field
$(this).prev().replaceWith(`<input type="text" value="${$(this).prev().text()}" />`)

//if the field is an input
$(this).prev().replaceWith(`<span class="user-name">${$(this).prev().val()}</span>`)
```
