# day05
2] Convert all strings to upper case
----
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

3] Sum of all numbers in an array
----
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
4] Return all the prime numbers in an array
----
const readline = require("readline");
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

