
## Table of Contents

- [Basics](#Basics)
    -[JavaScript Basics](#javascript-basics)
- [Install](#install)
- [Usage](#usage)
	- [Generator](#generator)
- [Badge](#badge)
- [Example Readmes](#example-readmes)
- [Related Efforts](#related-efforts)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

# Basics
## JavaScript Basics
### Spread & Rest:
are the three ... function in front of object/const.
## Spread:
Spread: to merge the one array with other data or object properties.
### Ex:
```js
const numbers = [1, 2, 3, 4];
const newNumbers = [...numbers, 5, 6];
console.log(newNumbers);
```
O/P: [1, 2, 3, 4, 5, 6]

## Rest:
to convert the multiple args into an array.
### Ex:
```js
const filter = (...args)=>{
  return args.filter(arg=> arg===1);
}
console.log(filter(1, 2, 3, 4));
```
O/P= [1]

# Destructuring
to store array elements/objects properties into variables.
### Ex:
```js
const numbers = [1,2];
[num1, num2] = numbers;
console.log(num1, num2);

const person = {name:'suhail', age:32};
[name] = person;
console.log(name);
```
# Create a copy of array, rather then copying the reference.
### Ex:
If assigning one array to new one. it will copy the reference. so any modification in new array will change the orignal aray value.
```js
const arr = {name:'sam', age:32};
const newArr = arr;
newArr.name = 'newSam';
console.log(arr.name);
```
O/P: newSam

### Solution: 
use spread operator.
```js
const arr = {name:'sam', age:32};
const newArr = {...arr};
newArr.name = 'newSam';
console.log(arr.name);
```
O/P: sam

# Array function 
functions to processing each element of the array and return the new array.
### Ex:
```js
const numbers=[1, 2, 3];
const multipleArr = numbers.map((num)=>{
  return num*2;
});
console.log(numbers);
console.log(multipleArr);
```
O/P: [1, 2, 3]
[2, 4, 6]

# React Basics:
- npm:      Node Package MAnager, a js depenedency resolver.
- webpack:  js project packing
- babel:    ES6/ES5 to normal js transpiler.

<img src="react_build_workflow.png"/>

# Installation
- download node.js [click here, Ctrl+Click](https://nodejs.org/en/), and install.
- open command prompt and type below cmd to install global react package.
```npm
npm install -g create-react-app
```
- select the directorry using cd command and execcute the below command to create the react project.
```npm
npm create-react-app <project name>
```
- go to cd <project name> directory
```npm
npm start
 ```
