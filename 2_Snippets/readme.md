<img alt="Logo" src="http://coderslab.pl/svg/logo-coderslab.svg" width="400">

# jQuery - Snippets
> Short pieces of code that solve various problems, illustrate dependencies, or show how to use some more complicated functions.

#### 1. Ajax

Connecting to the server, downloading data and writing them in the console:

```
$.ajax({
  url: "...",
  type: "GET",
  dataType: "json"
})
.done(function(response) {
  console.log(response);
});
```
XXXX is server address.
