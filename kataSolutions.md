https://www.codewars.com/kata/reversed-strings/train/javascript
Complete the solution so that it reverses the string value passed into it.


function solution(str){
  let letter = '';
  for(let i = str.length-1; i >= 0; i--){
    letter += str[i];
  }
  return letter;
}