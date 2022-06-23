# day05
1] Do the below programs in anonymous function & IIFE
1.1] Print odd numbers in an array
# anonymous function---
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

# IIFE---



1.2]Convert all the strings to title caps in a string array
# anonymous function---
  



# IIFE---


1.3] Sum of all numbers in an array
# anonymous function---
    var sumofarr=function(arr){
    var sumofarr = 0;
      for (let i = 0; i < arr.length; i++) {
           sumofarr += arr[i];
            }
}
    console.log(sumofarr([4, 8, 7, 13, 12]));


# IIFE---


1.4] Return all the prime numbers in an array
# anonymous function---
 

# IIFE---


1.5] Return all the palindromes in an array
# anonymous function---


# IIFE---


1.6] Return median of two sorted arrays of the same size
# anonymous function---


# IIFE---


1.7] Remove duplicates from an array
# anonymous function---

let arr=['guvi','geek','fullstack','vacation','geek','fullstack','sriptinglanguage','guvi'];
let dups=[...new Set(arr)];
console.log(dups);

# IIFE---


1.8] Rotate an array by k times
# anonymous function---


# IIFE---

3] Do the below programs in arrow functions
3.1] Print odd numbers in an array. (arrow function)
---
  var numbers = [11,12,33,45,56,67,78,79,90,93,99,98];
  var oddnum = numbers.filter(number => number%2 != 0);
       console.log(oddnum);

3.2] Convert all the strings to title caps in a string array (arrow function)
---
   var arr=['Hello','World','Guvigeeks','Chaithanya'];
   var uppercased=arr.map(name=> name.toUpperCase());
       console.log(uppercased);

3.3] Sum of all numbers in an array (arrow function)
---
   var nums = [26,23,17,8,12,14];
   var sum = nums.reduce((acc, ele) => acc+ele);
       console.log(sum);


3.4] Return all the prime numbers in an array (arrow function)
---
 

3.5] Return all the palindromes in an array (arrow function)
---


