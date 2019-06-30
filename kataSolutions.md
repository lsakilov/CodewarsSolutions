https://www.codewars.com/kata/get-list-sum-recursively/train/javascript

Write function sumR which returns the sum of values in a given list.
Try no to cheat and provide recursive solution.

function sumR(x) {
  if(x.length === 0){
    return 0;
  } else {
      return x.shift() + sumR(x);
    }
}