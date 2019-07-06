https://www.codewars.com/kata/find-the-missing-element-between-two-arrays/train/javascript
Given two integer arrays where the second array is a shuffled duplicate of the first array with one element missing, find the missing element.

Please note, there may be duplicates in the arrays, so checking if a numerical value exists in one and not the other is not a valid solution.

function findMissing(arr1, arr2) {
  let index;
  for(let i = 0; i < arr1.length; i++){
    index = arr2.indexOf(arr1[i])
    if(index > -1){
      arr2.splice(index, 1);
    } else {
      return arr1[i];
    }
  }
}