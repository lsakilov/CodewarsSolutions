https://www.codewars.com/kata/fake-binary/train/javascript
Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the resulting string.

function fakeBin(x){
  let newStr = '';
  for(let i = 0; i < x.length; i++){
    if(x[i] < 5){
      newStr += '0';
    } else {
      newStr += '1';
    }
  }
  return newStr;
}