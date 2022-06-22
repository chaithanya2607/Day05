# day05
1.1] Print odd numbers in an array.
---
# Normal function method
const readline = require("readline");
const inp = readline.createInterface({
  input: process.stdin
});
const userInput = [];
inp.on("line", (data) => {
  userInput.push(data);
});
inp.on("close", () => {
var oddnum=function(arr) {
    let temp= [];
    for (let ele of arr) {
        if (ele % 2 !== 0) {
            temp.push(ele)
        }
    }
    return temp;
}
console.log(oddnum([3,90,56,78,99,33,11,67,43]));
});
# Anonymous function method
# Arrow function method

1.2] Convert all strings to upper case.
----
# Normal function method
# Anonymous function method
# Arrow function method
const readline = require("readline");
const inp = readline.createInterface({
  input: process.stdin
});
const userInput = [];
inp.on("line", (data) => {
  userInput.push(data);
});
inp.on("close", () => {
   const arr=['Hello','World','Guvigeeks','Chaithanya'];
   const uppercased=arr.map(name=> name.toUpperCase());
   console.log(uppercased);
});


1.3] Sum of all numbers in an array.
----
# Normal function method
# Anonymous function method
# Arrow function method
const readline = require("readline");
const inp = readline.createInterface({
  input: process.stdin
});
const userInput = [];
inp.on("line", (data) => {
  userInput.push(data);
});
inp.on("close", () => {
    var arr = [4, 8, 7, 13, 12]
    var sumofarr = 0;
    for (let i = 0; i < arr.length; i++) {
        sumofarr += arr[i];
    }
    console.log(sumofarr);
});


1.4] Return all the prime numbers in an array.
----
# Normal function method
# Anonymous function methodconst readline = require("readline");
const inp = readline.createInterface({
  input: process.stdin
});
const userInput = [];
inp.on("line", (data) => {
  userInput.push(data);
});
inp.on("close", () => {
let arr = [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,17,33,99,77,73,61,93];
let result = [];
function Primenums(arr) {
  if(arr < 2) return false;
  for (var i = 2; i< arr; i++){
    if(arr % i == 0){
      return false;
    }
  }
  return true;
}
arr.forEach(function (element) {
  const elemnum = Primenums(element);
  if (elemnum) {
    result.push(element);
  }
});
console.log(result);
});
# Arrow function method

1.5] Return all plindromes in an array.
---
# Normal function method
# Anonymous function method
# Arrow function method
1.6] Return median of 2 sorted arrays of some size.
---
# Normal function method
# Anonymous function method
# Arrow function method
1.7] Remove duplicates from an array.
---
1.8] Rotate an array by k times.
---

