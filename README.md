# Flexbox in the Batcave


Flexbox must have a container and elements
```HTML
<nav class="container">
    <div>Home</div>
    <div>Search</div>
    <div>Logout</div>
</nav>
```

The container:
* Has a main axis (horizontal)
* Has a cross axis (vertical)
```CSS
.container{
    display:flex; 
    flex-direction: row; /* do you want the container to read vertically or horizontally? */
    justify-content:  flex-start;  /* justifies the elements */ /* flex-start, flex-end, center, space-around, space-between, space-evenly */
}
```
* Flex-start:
![flex-start](flex-start.png)
* Flex-end:
![flex-end](flex-end.png)
* Center:
![center](center.png)
* Space-around:
![Space-around](space-around.png)
* Space-between:
![Space-between](space-between.png)
* Space-evenly:
![Space-evenly](space-evenly.png)