# node-express

# Instructions

## Part 1
[Instructions](https://romebell.gitbook.io/sei-1019/node-express/00readme/01intro-to-node)
1. create a new repo
2. `clone` repo in local server
3. type `npm init` in terminal and complete prompts or `npm init -y`
4. create a js file called `index.js`
5. write some code in file
6. type `node index.js` in terminal to run in node

## Part 2
[Instructions](https://romebell.gitbook.io/sei-1019/node-express/00readme/02modules)
1. create a js file called `myModule.js`
2. create and define functions add, subtract, addAgain in `myModule.js`
```javascript
function add(num1, num2) {
    return num1 + num2
}

function subtract(num1, num2) {
    return num2 - num1
}

function addAgain(num1, num2) {
    return num1 + num2
}
```
3. add functions to module.exports
```javascript
module.exports = {
    add,
    subtract,
    addAgain
}
```
4. import the module in `index.js`
```js
const {add, subtract, addAgain} = require('./myModule.js')
```
5. call the functions in `index.js`
```js
console.log(add(10, 1))
console.log(subtract(5, 21))
console.log(addAgain(19, 13))
```
6. type `node index.js` in terminal to run in node

# Creating and Importing Node Modules
1. find a [node module](https://www.npmjs.com/browse/depended)
2. type `npm install <module>` in terminal
3. Refer to the documentation for proper usage
4. Create a `.gitignore` file so the `node_modules` folder doesn't upload to Github
5. Add `node_modules` to `.gitignore` file
