https://www.codewars.com/kata/if-you-cant-sleep-just-count-sheep/train/javascript
Given a non-negative integer, 3 for example, return a string with a murmur: 
"1 sheep...2 sheep...3 sheep...". Input will always be valid, i.e. no negative integers.

function countSheep(num){
  let arr = [];
  for(i = 1; i <= num; i++){
    arr.push(i + ' sheep...');
  }
  arr = arr.toString();
  arr = arr.replace(/,/g, '');
  return arr;
}
  const res = countSheep(5);