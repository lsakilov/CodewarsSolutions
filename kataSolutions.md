https://www.codewars.com/kata/valid-parentheses/train/javascript
Write a function called that takes a string of parentheses, and determines if the order of the parentheses is valid. The function should return true if the string is valid, and false if it's invalid.

function validParentheses(str){
  const stack = [], open = ['(', '{', '['], close = [')', '}', ']'];
  
  for(let i = 0; i < str.length; i++){
    if(open.includes(str[i])){
      stack.push(str[i]);
    } else {
      if(close.indexOf(str[i]) === open.indexOf(stack[stack.length - 1])){
        stack.pop(); 
      } else {
        return false;
      }
    }
  }
  return stack.length === 0;
  console.log(stack);
}