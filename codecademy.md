# Entry 2: Codecademy Tutorial 

### Breakdown of REACT JSX
Example of a JavaScript file:
```var h1 = <h1>Hello world</h1>;```

```<h1>Hello world</h1>``` 
(This portion is actually not HTML, it is JSX.)
* JSX is **not** valid JavaScript.
* When a JavasScript file includes JSX, the JSX will be translated into regular JavaScript.
* JSX elements (JavaScript expressions) can be set to a variable, used in a function, stored in an object or array, and etc. 

JSX Attribute is written like this (similar to HTML): ```attribute-name="attribute-value"```

```ReactDOM.render``` is used to render the JSX, which is done by taking a JSX expression, creating a tree of the DOM nodes, and adding that tree to the DOM.
```
var myDiv = <div className="big">I AM A BIG DIV</div>
ReactDOM.render(
  myDiv, 
  document.getElementById('app')
  );
```
**Once again, manipulating the DOM is slow whereas manipulating the virtual DOM is faster since nothing is changed onscreen.**

* JSX requires slashes!! (e.g. Instead of ```<br>,``` use ```<br/>```)
* Use { } to run JavaScript 
  * 2 + 3 → 2 + 3 (read as a JSX element, not JavaScript)
  * {2 + 3} → 5 (treated as JavaScript)

[List of Event Listeners](https://facebook.github.io/react/docs/events.html#supported-events) - a process/function when a computer program waits for something to occur
  * The value of an event listener should be a function.
  ```
function myFunc () {
  alert('Make myFunc the pFunc... omg that was horrible i am so sorry');
}

<img onClick={myFunc} />
```

#### Conditional Statement
When the ```if``` statement is on the outside → no need for curly brackets or "JavaScript Injection"

* Ternary Operator: x ? y : z 

![Visual Diagram](http://unitedwebsoft.in/blog/wp-content/uploads/2015/10/php_ternary_operator.png)

```.map``` is used in JSX and is often used on an array of strings → returns a new array of lists```<li>```

#### Key?
```key``` is a JSX attribute (keys don't do anything, but are used to keep track of lists).
``` <li key="li-01">Example1</li>```


JSX: 
```var h1 = <h1>Hello world</h1>;
can be rewritten without JSX, like this:
```
WITHOUT JSX:
```
var h1 = React.createElement(
  "h1",
  null,
  "Hello, world"
);
```

### What I Learned + Takeaways
* Practice typing out the code. It is **extremely** helpful in getting you into the habit of typing the same code over and over again.
  * Especially ```ReactDOM.render();```
* Because this is Codecademy, make sure you read carefully and try out the code. Make more and more observations. 
* Also, because Codecademy offers quizzes after each unit, it is a good idea to test yourself to make sure you understand. Take advantage of your resources!! 