https://www.codewars.com/kata/sum-all-the-arrays/train/javascript
You are given an array of values.

Sum every number value in the array, and any nested arrays (to any depth).

Ignore all other types of values.

function arraySum(arr) {
  const b = arr.toString().split(',');
  let sum = 0;
  
  for(let i = 0; i < b.length; i++){
    sum += Number.isNaN(Number(b[i])) ? 0 : Number(b[i]);
  }
  return sum;
}