# Entry 3: Codecademy Tutorial on Components
### Breakdown of the Components
`var React = require('react');` will return a JavaScript object, which contains methods. This returned object is called the React *library*.

`var ReactDOM = require('react-dom');` is similar to the previous code but the difference is that it ***interacts*** with the DOM.

`var myComponentClass = React.createClass();` is the **component class**, which creates whatever component. It only takes on argument and this argument MUST be a JavaScript object (component class names must start with capital letters).
* Similar to Mr. Mueller's Object Orientation visual diagram, think of the component class as the factory and the components as what is produced (objects) - in this case, the duct tape.

![analogy](/pictures/analogy.JPG)
* A render function has to be included in an object and the render function must include a *return statement*. 
```javascript
var instructions = {
  render: function () { //"instructions object" 
    return <h1>Hello world</h1>;
  }
};
```
`render` is a function that every component instance *inherits* (There can be many different instances: `<MyComponentClass />`)
* A render function **must** have a return statement.

### How does JSX and React work together?
First of all, a multi-line JSX expression needs to be wrapped in parentheses. 

The term `this` is used very often. Similar to Ruby, it refers back to a specific object being passed by React.createClass. 

```javascript
var MyName = React.createClass({
	// name property goes here:
name: 'Sharon',

  render: function () {
    return <h1>My name is {this.name}.</h1>;
  }
});

ReactDOM.render(<MyName />, document.getElementById('app'));
```

### What I Learned + Takeaways
* Double check that curly brackets, semi-colons, and parentheses are in the right place.
* Draw out or refer to a visual diagram that can help you understand the process. For me, I related back to Mr. Mueller's object orientation diagram.



