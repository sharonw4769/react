# Entry 4: Codecademy Tutorial on Component Interactions
### Understanding the Interactions
##### How a Component RENDERS Another Component 
* One important thing to take note of is that by default, every JavaScript file is invisible to any other JavaScript file. This means that if the application consists of multiple .js files, then it will need to include `var file_name = require('./{file_name}.js');` in order to allow the current file to navigate its path to the other file (this is called a *filepath*).
* By requiring that specific line of code, it importing the entire file. In order to redner a specific part, `module.exports` will be used.  
    * How does module.exports work? Well, when a module is created, just think of it as moving all related functions into one file. In other words, the functions that are referenced by `module.exports = ___;` will be made into the current values. 
    *   `module.exports` and `require` are often seen used together.
##### How a Component PASSES INFO to Another Component 
### What I Learned + Takeaways
*