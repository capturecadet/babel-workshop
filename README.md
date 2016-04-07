# babel-workshop
A short workshop on setting up babel and webpack to execute some simple ES6 code.

### Before attending the workshop

Please ensure you download the repo and run `npm install` on a LAN connection before the workshop. We’ve provided you with a sample `package.json` containing all the node_modules you’ll need for the workshop, but the booths don't have many LAN cables, so let's save some wifi related pain.

##### Useful links

* http://babeljs.io/
* http://webpack.github.io

### Step 1 - Make Webpack your friend (10 Minutes)

* Set up a simple html page that pulls in a javascript file called `bundle.js`.
* Use commandline webpack to bundle another file called `index.js` into `bundle.js` using webpack. Have a play around with serving and watching changes on the file.
* You can run commandline webpack by doing `node_modules/.bin/webpack`
* In `index.js` write some sample ES5 code that writes the sentence “Javascript Happy Funtimes!” to the document, and preview it in chrome. If you have time, you could also try creating another .js file to require into `index.js`, to see webpack in action!

### Step 2 - Require some css files! (10 Minutes)

* Set up webpack to use a config file and enable a style loader.
* Create a style.css file and stick some rules in it.
* With the style loader enabled, use webpack to require the css file and preview the styles in the browser.

### Step 3 - Transpile some ES6 bro (10 Minutes)

* Add this code to your index.js file:

```javascript
var myAwesomeFunction = require(“./myAwesomeFunction”);
myAwesomeFunction();
```

Create the `myAwesomeFunction.js` file, add a function that executes some ES6code and export it.
Use babel and webpack to bundle your ES6 code and check it works in the browser.
