https://www.codewars.com/kata/reverse-a-number/train/javascript

Given a number, write a function to output its reverse digits. (e.g. given 123 the answer is 321)

Numbers should preserve their sign; i.e. a negative number should still be negative when reversed.

function reverseNumber(n) {
  if (n >= 0){
    let arr = n.toString().split('').reverse();
    return +(arr.join(''));
  } else {
    n = n * (-1);
    let arr = n.toString().split('').reverse();
    return (-1) * (+(arr.join('')));
  }
}