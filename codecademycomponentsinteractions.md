# Entry 4: Codecademy Tutorial on Component Interactions
### Understanding the Interactions
##### How a Component RENDERS Another Component 
* One important thing to take note of is that by default, every JavaScript file is invisible to any other JavaScript file. This means that if the application consists of multiple .js files, then it will need to include `var file_name = require('./{file_name}.js');` in order to allow the current file to navigate its path to the other file (this is called a *filepath*).
* By requiring that specific line of code, it importing the entire file. In order to redner a specific part, `module.exports` will be used.  
    * How does module.exports work? Well, when a module is created, just think of it as moving all related functions into one file. In other words, the functions that are referenced by `module.exports = ___;` will be made into the current values. 
    *   `module.exports` and `require` are often seen used together.
##### How a Component PASSES INFO to Another Component 
`this.props` has objects which holds information about the component.
In order to get the information, add a name and value to the first argument and then put `return <h1>Hi there, {this.props.firstName}!</h1>;` in the variable section. 
Example: 
```javascript
var Greeting = React.createClass({
  render: function () {
    return <h1>Hi there, {this.props.firstName}!</h1>;
  }
});

// ReactDOM.render goes here:
ReactDOM.render(
  <Greeting firstName='Sharon' />, 
  document.getElementById('app')
);
```
##### Event Handler
* Functions are usually passed as props. These functions are defined as instructions object properties. 

Example: (Top portion is the event handler)
```javascript
handleEvent: function () {
    alert('');
  },
render: function () {
    return (
      <h1 onClick={this.handleEvent}>
        Hello world
      </h1>
    );
  }
});
  ```
How to attach as an event handler? Attach any event handler to a JSX element by adding a special attribute (attributee names include -- onClick, onHover, and etc.)


```javascript
<List>  // opening tag
  <li></li> // child
</List> // closing tag
```

Using `{this.props.children}` will list. 

##### Dynamic Information 
The two ways to access dynamic info: `props` and `state`. 
```javascript
var Example = React.createClass({
  getInitialState: function () { #getInitialState returns an object
    return { mood: 'decent' }; #has a state of mood
  },
```
In order to read a component's state, use the expression `this.state.name-of-property`

In order to change state, use this function `this.setState`

-----
##### Vocabulary: 
To **inject** a variable name between tags, put curly brackets around it.

**props**: name of the object that stores the information being passed OR two pieces of information passed-in.

**this.props**: refers to that storage object.

**prop**: *each* piece of information passed.

Note: `<Button />` is a component instance.

### What I Learned + Takeaways
* Because this unit was very long but **extremely important**, it was a good idea to breakdown the lessons and spend a day or two working on 3-5 lessons instead of doing all the lessons in one topic and cramming all the information. 
* Use outside resources if the definition from codecademy is unclear. Do not be afraid to use outside sources!! 
* Understand the material, do not just memorize.
  * Honestly, there's no point in memorizing certain parts of code because there are so many resources to look up that specific part so the best advice is to understand it because it is more useful to know HOW to read the code. 