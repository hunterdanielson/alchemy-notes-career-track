# Alchemy Reading Notes
1. Why run JavaScript outside a browser?
    - Typically JavaScript is run inside a browser with some HTML/CSS code mixed in as well. Backends however can also use JavaScript code for the database and can be used to create RESTful APIs.
    [Quora source](https://www.quora.com/What-exactly-does-running-JavaScript-inside-a-browser-and-outside-of-a-browser-mean)
1. Difference between module and package
    - A module is a library, can be a single file. A package is a group of modules (libraries) grouped together, has a package.json file. 
    [Stackoverflow source](https://stackoverflow.com/questions/20008442/difference-between-a-module-and-a-package-in-node-js)
1. What does Node package manager do?
    - [This website](https://www.tutorialsteacher.com/nodejs/what-is-node-package-manager) sums it up nicely, "Node Package Manager (NPM) is a command line tool that installs, updates or uninstalls Node.js packages in your application. It is also an online repository for open-source Node.js packages."
1. 3 Ways to export a function from a node module
    - Export function
    ```javascript
        module.exports = function(msg) {
            console.log(msg);
        };
      ```
    - Export function as class
    ```javascript
       module.exports = function (firstName, lastName) {
            this.firstName = firstName;
            this.lastName = lastName;
            this.fullName = function () { 
                return this.firstName + ' ' + this.lastName;
            }
        }
    ```
    - Creating and exporting a module
    ```javascript
        const getName = () => {
            return 'Jim';
        };
        exports.getName = getName;
    ```
    - Sources: [Export functions](https://www.tutorialsteacher.com/nodejs/nodejs-module-exports), [Creating and exporting](https://www.sitepoint.com/understanding-module-exports-exports-node-js/)