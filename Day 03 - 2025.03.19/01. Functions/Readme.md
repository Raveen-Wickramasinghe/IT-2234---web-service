# 🧠 JavaScript Function Examples

This project demonstrates different types of functions in JavaScript, using Node.js to execute them in a backend runtime environment. It serves as a reference for various function types, including void functions, return-type functions, arrow functions, and more.

## 📂 File Included

- `Functions.js` – JavaScript file containing all the function examples

## 🚀 How to Run

1. **Install Node.js**  
   Download from: https://nodejs.org/  
   Check if installed:  
   ```bash
   node -v
cd "F:\2.2\2.2\IT2234- web service &server technology"
node Functions.js
1. Void Function


function printMsg() {
    console.log("Hello Raveen...!");
}

2. Return Type Function
function sum() {
    return 5 + 6;
}
3. Function with Parameters
function sub(a, b) {
    return a - b;
}
4. Arrow Function

const msg = () => {
    console.log("Hello Raveen...!");
};

5. Default Parameter
const multiply = (num1, num2 = 2) => {
    return num1 * num2;
};
6. Rest Parameters

const mySum1 = (...n) => {
    let sum = 0;
    for (let a of n) {
        sum += a;
    }
    return sum;
};
const mySum2 = (...n) => {
    let sum = 0;
    n.forEach((a) => sum += a);
    return sum;
};
const mySum3 = (...n) => {
    return n.reduce((sum, a) => sum + a, 0);
};

7. Callback Function
const greet = (msg, fun) => {
    console.log("Hi...." + msg);
    fun();
};

greet("Good Morning..!", () => {
    console.log("My name is Raveen");
});

8. Callback with Rest Parameters
const multwo = (n) => n * 3;

const myArr = (mul, ...n) => {
    n.forEach((a) => console.log(mul(a)));
};

myArr(multwo, 2, 4, 6);

