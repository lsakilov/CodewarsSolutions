
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Alan Partridge II - Apple Turnover

function apple(x){
  return res = +(x ** 2 > 1000) ? "It\'s hotter than the sun!!" : "Help yourself to a honeycomb Yorkie for the glovebox.";
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Calculate BMI

function bmi(weight, height) {
  return res = (weight / height ** 2) <= 18.5 ? "Underweight" : (weight / height ** 2) <= 25.0 ? "Normal" : (weight / height ** 2) <= 30.0 ? "Overweight" : "Obese";
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
What's the real floor?

function getRealFloor(n) {
  return real = n <= 0 ? n : n > 12 ? n - 2 : n - 1;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Even or Odd

even_or_odd = number => return msg = number % 2 === 0 ? msg = 'Even' : msg = 'Odd';

function even_or_odd(number) {
  return msg = number % 2 === 0 ? msg = 'Even' : msg = 'Odd';
}

OR

function even_or_odd(number) {
  let msg;
   if(number % 2 === 0){
     msg = 'Even';
   } else {
     msg = 'Odd';
    }
   return msg;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Is he gonna survive?

function hero(bullets, dragons){
  return (bullets / 2) >= dragons ? true : false;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Simple Comparison?

function add(a, b){
	return a == b ? true : false;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Chuck Norris VII - True or False? (Beginner)

function ifChuckSaysSo(){
  return 10 > 12;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Keep up the hoop

function hoopCount (n) {
   return msg = n >= 10 ? "Great, now move on to tricks" : "Keep at it until you get it";
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Be Concise I - The Ternary Operator

let describeAge = age => "You're a(n) " + (age <13? "kid" : age < 18? "teenager" : age < 65?
    "adult" : "elderly");
    
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Century From Year

function century(year) {
  return Math.ceil(year/100);
}
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
