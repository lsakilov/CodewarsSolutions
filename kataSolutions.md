https://www.codewars.com/kata/convert-a-string-to-a-number/train/javascript
We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.

var stringToNumber = function(str){
  return parseInt(str, 10);
}