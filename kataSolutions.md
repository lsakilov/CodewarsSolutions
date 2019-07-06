https://www.codewars.com/kata/remove-string-spaces/train/javascript

Simple, remove the spaces from the string, then return the resultant string.

function noSpace(x){
  let str = x.replace(/ /g, '');
  return str
}