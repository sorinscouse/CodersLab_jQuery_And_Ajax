<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# Gallery

> Write your answers in appropriate files, unless the instructions tell you otherwise.
Remember to separate exercises with comments, and write legible, well-formatted code.
If the instruction says "Create a new function", this means that you should
create the function. Even if the task seems really simple,
learn to use functions.


## Exercises to do on your own

Your task will be to create a dynamic image search engine.

Under the link https://pixabay.com you will find a website that shares free graphics. At the bottom, there is a link to a free [API](https://pixabay.com/pl/service/about/api/) .
To use this API you need to register. You can do this on [this page](https://pixabay.com/pl/accounts/register/) or clicking the **Register** link at the top of the page.
After registering, return to the [API page](https://pixabay.com/pl/service/about/api/) above and click the green button labeled **Get Started**.
On [the page that will load](https://pixabay.com/api/docs/#api_search_images) you will see all parameters that will be sent, and a required key that was created for you.


### Loading data  (~ 15min - 30min)
Create variables:
- **apiUrl** - a link to the abovementioned API
- Assign elements that you will work on to variables: a form with `.form` class, input with ```.form-search``` class, and an element with ```.gallery``` class.

Add a **submit** event to the form that will:
- prevent the default form action,
- extract field values.

The next step will be loading the data.
At the end of the event above, initiate a ```loadImages(searchQuery)``` function that you will write in a moment. searchQuery parameter will be the value of a form field extracted above.

Write the ```loadImages(searchQuery)``` function and call it at the end of the submit event.
This function will make an Ajax connection in which you must sent the right data. [Two of the parameters](https://pixabay.com/api/docs/#api_search_images) are required - **key** and **q** that represents the searched phrase. Other parameters are optional.

Connection made in this function can take the form of:
```
...
$.ajax({
    url : apiUrl,
    data : {
        q : searchTerm,
        key : "...."
    }
}).done(function(result) {
    ...
})
...
```

After closing the connection, write the result in the console and check what it looks like. You can also use the Network tab.

Then, iterate through received data with a loop, generate gallery elements and insert them into the gallery. You can find an example of an element that you can generate in the **index.html** file. To create more complex html pieces (as in this case) you can use [template string](https://developer.mozilla.org/pl/docs/Web/JavaScript/Referencje/template_strings).
Before inserting new elements, clear the gallery contents using an appropriate jQuery method.

### Counteracting redundancy (~ 10min)
At this point, the search engine should already work. The problem will appear when the user starts quickly clicking on the search button. The previous connections will not end, and more will be created. You must prevent this.

At the beginning of the form submission - just after blocking the default action, find the submit button in the form and assign it to a variable.
Add the ```disabled``` attribute to this button and set it to true. Add the ```.loading``` class to it as well.
After you finish adding the loaded items to the gallery, delete the ```disabled``` attribute and the ```.loading``` class in the submit.
If you want, you can also add the ```.loading``` class to the gallery element for the time of loading.

Now, test what you have written.
Go to the Network tab in the debugger and switch the option of simulating the connection speed (to the right on the top bar of this tab - next to the Offline option) to slow connection. After testing, return to the normal setting.

### Lightbox (~ 10min - 15min)
One of the biggest advantages of jQuery was and still is a huge collection of ready-made plugins. In this case, we want to add lightbox to our search engine - a photo viewer with a darkened background. If you search the Internet for "jquery lightbox", one of the first results will be the fancybox.

Go to the following page: http://fancyapps.com/fancybox/3/

At the top of the page, there is a "Quick  Start" section. You need to add 2 files to your page - a stylesheet and a script with the library.

```
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/fancybox/3.4.1/jquery.fancybox.min.css" />
<script src="https://cdnjs.cloudflare.com/ajax/libs/fancybox/3.4.1/jquery.fancybox.min.js"></script>
```

Remember to place the script with the library **below** the jQuery script.

Add ```data-fancybox="gallery"``` attribute to the links that were made earlier (in the ```loadImages``` function).
Now, after clicking on a miniature, the lightbox will launch with an enlarged graphic.
