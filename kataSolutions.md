https://www.codewars.com/kata/numerical-palindrome-number-5-1/train/javascript
A palindrome is a word, phrase, number, or other sequence of characters which reads the same backward as forward. Examples of numerical palindromes are:

2332 
110011 
54322345

For a given number num, write a function to test if the number can be rearranged to form a numerical palindrome or not and return a boolean (true if it can and false if it cannot). For this kata, single digit numbers will NOT be considered numerical palindromes.

Return "Not valid" if the input is not an integer or is less than 0.

function palindrome(num) { 
  if(typeof num !== 'number' || num < 0) return "Not valid";
  if(num < 10) return false;
  num = num.toString().split('').sort();
  console.log(num)
  let count = 0;
  for(let i = 0; i < num.length - 1; i){
    if(num[i] === num[i+1]){
      count = count + 2;
      i = i + 2;
    } else i++;
  }
    if(num.length === count || num.length === count +1){
      return true;
    } else return false;
}