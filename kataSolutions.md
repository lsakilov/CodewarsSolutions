https://www.codewars.com/kata/remove-duplicates-from-list/train/javascript

Define a function that removes duplicates from an array of numbers and returns it as a result.

The order of the sequence has to stay the same.

function distinct(a) {
  const items = {};
  const res = [];
  
  for(let i =0; i < a.length; i++){
    if(!items[a[i]]){
      res.push(a[i]);
      items[a[i]] = true;
    }
  }
  return res;
}