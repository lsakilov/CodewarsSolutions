https://www.codewars.com/kata/string-average/train/javascript
You are given a string of numbers between 0-9. Find the average of these numbers and return it as a floored whole number (ie: no decimal places) written out as a string. Eg:

"zero nine five two" -> "four"

If the string is empty or includes a number greater than 9, return "n/a"

function averageString(str) {
  let arr = ['zero', 'one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine'];
  let arrStr = str.split(' ');
  let sum = 0;
    for(let i = 0; i < arrStr.length; i++){
      sum += arr.indexOf(arrStr[i]);
      if(arrStr[i] === '' || arr.includes(arrStr[i]) === false) return 'n/a'
    }
    let avg = Math.floor(sum/arrStr.length);
    return arr[avg];
}