1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
// Anonymous function
let percentage = function(marks,total){
  return (marks * 100) / total;
}
// function expression 
let percentage = function percentage(marks,total){
  return (marks * 100) / total;
}
// arrow function
let percentage = (marks,total) => {
  return (marks * 100) / total;
}
//  Arrow function with return statement
let percentage = (marks,total) => (marks * 100) / total;




```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer - function defination



```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};


// Your answer - function expression 



```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};

// Your answer - anonymous function


```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// Your ansswer - function expression

```

```js
let percentage = (marks, total) => (marks * 100) / total;
// Your Answer - function expresssion

```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

   Function is a object and object is a value, we have to put on the right hand side of equal to, i.e why function expression exist in javascript.
   ex- let percentage = (marks, total) => (marks * 100) / total;


4. Why is a function call an expression in JavaScript?
   - A function call always return a value whether it is undefined or a particular value.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Answer - VALID  - function excution/call while storing the value.

five = add; // Answer VALID - this is function reference.

five = five(10, 11); // Answer - VALID - 21 

five = function () {
  return 'Hello';
}; // Answer -  VALID  
```

6. What is the difference between function definition and function call? Explain with an example.

- function defination means when function starting the keyword that is known as function defination. 

  function add(a,b){
    return a + b;
  }

  function call means to excute the function by calling it with exact name.

  add(23,4);

7. What is the similarities between function definition and function call?

  - function defination is an expression  i.e function is an object
    function call is a expression i.e function call always return a value ewheteher it is a value or undefined.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid - Valid because function is behaving like an object. Function is a special type object that can be excuted.
```

9. What is higher order function explain with an example.
  - A function that accepts a function defination as an arguments  or return the function defination from the function is known as higher order function.

  let isodd = function (num) {
    return num % 2 !== 0;
  }

  function filterOdd(arr, fn){
    console.log((fn(23), "Inside filteredOdd");
    return arr;
  }

  filterOdd([1,2,3,4], isodd);

10. Explain what is callback function. Why you can pass a function inside a function?

    - A function that is passed as a function defination is known as a call function.
       We are passing function inside another as a parameter because function is an expression i.e called higher order function.

      
