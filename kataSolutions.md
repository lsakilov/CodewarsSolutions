https://www.codewars.com/kata/reverse-list-order/train/javascript

In this kata you will create a function that takes in a list and returns a list with the reverse order.

function reverseList(list) {
    let arr = [];
    for(let i = list.length - 1; i >= 0; i--){
        arr.push(list[i]);
    }
    return arr;
}