https://www.codewars.com/kata/bin-to-decimal/train/javascript
Complete the function which converts a binary number (given as a string) to a decimal number.

function binToDec(bin){
  let a = parseInt(bin, 2).toString(10);
  return parseInt(a, 10);
}
===========================
function binToDec(bin){
  return parseInt(bin, 2);
}