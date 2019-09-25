**Functions set as attributes** 

```html
<button onclick="saySomething('You said something!')">Click</button>
```
- easy to read and follow
- easy to write 
- no seperation of concerns
- only one function per argument

=====================================

**Functions set as properties**

```html
<button id="myButton">Click</button>
```

```js
document.getElementById('myButton').onclick = function (event) {
    alert('You have been alerted again!');
```

- easy to write
- does provide seperation of concerns
- less obvious event
- only one function per event

=====================================

**Functions as eventListeners**

- easy to write
- provides seperation of concerns
- events are less obvious
- allows for multiple functions attached to a single event

```js
function listenerAlert() {
    alert("you were clicked with the addEventListener method")
};

document.getElementById('myButton').addEventListener('click', listenerAlert);
```

```html
    <div></div>
    <div class="element"></div>
    <div id="element"></div>
```

```js
document.getElementsByTagName("div");
document.getElementsByClassName("element");
document.getElementById("element");
```

<!-- Introduce jQuery -->

```js
$("div");
$(".element");
$("#element");
```

<!-- 2013 Browsers Catch Up -->

```js
document.querySelector("div");
document.querySelector(".element");
document.querySelector("#element");
```