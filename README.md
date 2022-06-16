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
