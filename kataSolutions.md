++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Count Odd Numbers below n

function oddCount(n){
  return Math.floor(n / 2);
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

const closestMultiple10 = num => {
  return (Math.round(num*0.1))*10;
};

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Area of a Square

function squareArea(A){
  return Math.round((((A*4)/(2*Math.PI))**2)*100)/100;
}

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Formatting decimal places #0

function twoDecimalPlaces(n) {
  return (Math.round(n * 100) / 100);
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Discover The Original Price

function discoverOriginalPrice(discountedPrice, salePercentage){
  return Math.floor((discountedPrice /(100 - salePercentage)* 100)*100)/100;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Sum The Strings

function sumStr(a,b) {
  return (Number(a)+Number(b))+ '';
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Number toString

public class Kata
{
  public static string A = 123.ToString();
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
The Wide-Mouthed frog!

function mouthSize(animal) {
  if(animal == 'alligator'){
    return 'small';
  } if(animal == 'ALLIGATOR') {
    return 'small';
  } else {
    return 'wide';
  }
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Super Duper Easy

function problem(x){
  if(typeof x === 'string'){
    return 'Error';
  } else {
    return x * 50 + 6;
  }
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Convert boolean values to strings 'Yes' or 'No'.

function boolToWord( bool ){
  if(bool === true){
    return 'Yes';
  } else {
    return 'No';
  }
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Sum of angles

function angle(n) {
  return 180*(Math.round(n-2));
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
For Twins: 2. Math operations

function iceBrickVolume(radius, bottleLength, rimLength) {
  let brickSide = (radius*2)/(2**0.5);
  let brickHeight = Math.round(bottleLength - rimLength);
  return Math.round(brickHeight*brickSide*brickSide);
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Breaking chocolate problem

function breakChocolate(n,m) {
  let cut = 0;
  if(n === 0 || m === 0){
    return 0;
  } else {
    return n*m-1;
  }
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++


Training JS #1: create your first JS function and print "Helloworld!"

function helloWorld(){
var str = "Hello World!";
console.log(str);
return str;
}
console.log(helloWorld());

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

package com.company;

public class Main {

    public static void main(String[] args) {
	    int[][] array = {{1, 2, 3, 4, 5}, {6, 7, 8, 9}, {-1, -2, -3, -4}, {-5, 6}};
	    int count = 0;
	    for (int i = 0; i < array.length; i++) {
	        count += array[i].length;
        }
	    System.out.println(count);
    }
}
