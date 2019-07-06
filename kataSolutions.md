https://www.codewars.com/kata/valid-parentheses/train/javascript
Write a function called that takes a string of parentheses, and determines if the order of the parentheses is valid. The function should return true if the string is valid, and false if it's invalid.

function validParentheses(str){
  const arr = str.split('');
  let a = 0;
  for(let i  = 0; i < arr.length; i++){
    if(arr[i] === '(') a += 1;
    else if (arr[i] === ')') a -= 1;
    if(a < 0 ) return false;
  }
  if(a === 0) return true;
  else return false;
}