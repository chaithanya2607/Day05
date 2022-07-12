# Day05
# 1] Do the below programs in anonymous function & IIFE
# 1.1] Print odd numbers in an array

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

        (function(arr) {
    let temp= [];
    for (let ele of arr) {
      if (ele % 2 !== 0) {
        temp.push(ele)
      }
      }
      console.log(temp);
      })([3,90,56,78,99,33,11,67,43]);
 
# 1.2]Convert all the strings to title caps in a string array

# anonymous function---

     var string = function toTitleCase(str) {
     return str.toLowerCase().split(' ').map(function (string) {
        return (string.charAt(0).toUpperCase() + string.slice(1));
    }).join(' ');
        }
       console.log(string("guvi geeks full stack development"));
  
# IIFE---

    (function(str) {
    var a= str.toLowerCase().split(' ').map(function (string) {
    var b= (string.charAt(0).toUpperCase() + string.slice(1));
    console.log(b);
    })
    })("guvi geeks full stack development");


# 1.3] Sum of all numbers in an array

# anonymous function---

    var sumofarr=function(arr){
    var sumofarr = 0;
      for (let i = 0; i < arr.length; i++) {
           sumofarr += arr[i];
            }
        }
    console.log(sumofarr([4, 8, 7, 13, 12]));

# IIFE---

      (function(arr){
      var sumofarr = 0;
      for (let i = 0; i < arr.length; i++) {
        sumofarr += arr[i];
       }
        console.log(sumofarr);
       })([4, 8, 7, 13, 12]);


# 1.4] Return all the prime numbers in an array
-----
      let arr= [-1,-2,-3,1,2,3,4,5,6,7,8,9,10];
       let result = [];
       function isPrime(arr) {
       if(arr< 2) return false;

       for (let k = 2; k < arr; k++){
         if(arr % k == 0){
           return false;
         }
            }
         return true;
        }
          arr.forEach(function (element) {
          const item = isPrime(element);
         if (item) {
         result.push(element);
           }
         });
         console.log(result);

# 1.5] Return all the palindromes in an array

# anonymous function---

        function isPalindrome(str) {
      str = str.replace(/\W/g, '').toLowerCase();
       return (str == str.split('').reverse().join(''));
          }
          console.log(isPalindrome("level"));               
          console.log(isPalindrome("levels"));
          console.log(isPalindrome("A car, a man, a maraca"));


# 1.6] Return median of two sorted arrays of the same size
# anonymous function---function getMedian(ar1, ar2, n)
    {
    let j = 0;
    let i = n - 1;
    while (ar1[i] > ar2[j] && j < n && i > -1)
    {
        let temp = ar1[i];
        ar1[i] = ar2[j];
        ar2[j] = temp;
        i--; j++;
    }
    ar1.sort(function(a, b){return a - b});
    ar2.sort(function(a, b){return a - b});
    return parseInt((ar1[n - 1] + ar2[0]) / 2, 10);
    }
     
    let ar1 = [ 1, 12, 15, 26, 38 ];
    let ar2 = [ 2, 13, 17, 30, 45 ];
 
    let n1 = 5;
    let n2 = 5;
     if (n1 == n2){
      console.log(getMedian(ar1, ar2, n1));}
       else{
       console.log("Doesn't work for arrays of unequal size");
       }

# 1.7] Remove duplicates from an array
# anonymous function---

          let arr=['guvi','geek','fullstack','vacation','geek','fullstack','sriptinglanguage','guvi'];
          let dups=[...new Set(arr)];
          console.log(dups);

# IIFE---

      (function (a){
       var arr = [];
       for (var i = 0; i < a.length; i++) {
       if (arr.indexOf(a[i]) === -1) {
            arr.push(a[i]);
             }
           }
          console.log(arr);
       })(["guvi","geeks","geeks","guvi","guvi"]);


# 1.8] Rotate an array by k times
----    
      function arrayRotate(arr, k) {
          k -= arr.length * Math.floor(k / arr.length);
          arr.push.apply(arr, arr.splice(0, k));
          return arr;
       }
      for(let i =0 ; i <= 3 ; i++) {
      console.log(arrayRotate(["Guvian","a","am","I"], i), i);
      }

# 3] Do the below programs in arrow functions
# 3.1] Print odd numbers in an array. (arrow function)
---
       var numbers = [11,12,33,45,56,67,78,79,90,93,99,98];
       var oddnum = numbers.filter(number => number%2 != 0);
       console.log(oddnum);

# 3.2] Convert all the strings to title caps in a string array (arrow function)
---
       var arr=['Hello','World','Guvigeeks','Chaithanya'];
       var uppercased=arr.map(name=> name.toUpperCase());
       console.log(uppercased);

# 3.3] Sum of all numbers in an array (arrow function)
---
      var nums = [26,23,17,8,12,14];
      var sum = nums.reduce((acc, ele) => acc+ele);
      console.log(sum);


# 3.4] Return all the prime numbers in an array (arrow function)
---
       var arr=[26,2,3,5,77,88,93,71,31];
       var primenum=num=>{
          for (var i=2;i<num;i++){
             if(num%i===0)  return false;
          }
         return num !== 1;
         };
       var prime=arr.filter((ele)=>primenum(ele));
        console.log(prime);
 

# 3.5] Return all the palindromes in an array (arrow function)
---    
         const getAllPalindromes = (words) => words.filter((word) => word.split("").reverse().join("") === word);
         console.log(getAllPalindromes(["damage", "rotator"]));


