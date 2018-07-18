# CSS VARIABLES IN THE BATCAVE

Here's why you should be using CSS variables:
1. No transpiling
2. Has access to the DOM
3. Perfect for themes

### Declare a CSS variable
```CSS
/* This is a global variable */
:root{
    --red: #ff6f69;
}
```
### Use a CSS variable
```CSS
#title{
    color:var(--red);
    }
```
### Overwrite a CSS value
```CSS
/* The red variable is overwridden with a new value*/
/* You can also create entirely new variables this way*/
#title{
    --red: #ff0000;
    --green: #00ff00;
}
```
### CSS variables with Javascript
```Javascript
// generally get the root HTML
var root = document.querySelector(":root");

// fetch the variable
var rootStyles = getComputedStyle(root);
var red = rootStyles.getPropertyValue("--red");
console.log("red: ",red);

// update the variable
root.style.setProperty("--red","#ff0000");
```

### CSS variables with Media queries
```CSS
.grid{
    --columns: 200px 200px;
}

@media all and (max-width: 450px){
    .grid{
        --columns: 200px;
    }
}
```