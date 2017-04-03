# Entry 3: Codecademy Tutorial on Components
### Breakdown of the Components
`var React = require('react');` will return a JavaScript object, which contains methods. This returned object is called the React *library*.

`var ReactDOM = require('react-dom');` is similar to the previous code but the difference is that it ***interacts*** with the DOM.

`var myComponentClass = React.createClass();` is the **component class**, which creates whatever component. It only takes on argument and this argument MUST be a JavaScript object.  
* Similar to Mr. Mueller's Object Orientation visual diagram, think of the component class as the factory and the components as the production (objects).
* 