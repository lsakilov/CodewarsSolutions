[Filter the number](https://www.codewars.com/kata/55b051fac50a3292a9000025/javascript)
```javascript
var FilterString = function(value) {
return parseInt(value.replace(/[a-z]/gi,''))
}
```
[isReallyNaN](https://www.codewars.com/kata/56c24c58e0c0f741d4001aef/javascript)
```javascript
const isReallyNaN = (val) => {
  return Number.isNaN(val) ? true : false;
};
```
for (let i = 1; i <= 10; i++) {     
  for (let j = 1; j <= 10; j++) {
    console.log(`${i} * ${j} = ${i * j}`);
  }

  console.log('--------------');  // строка, разделяющая столбцы таблицы умножения
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Power
function numberToPower(number, power){
  var res = 1;
  var count = 0;
  if(power > 0){
    do{
      res = res * number;
      count++;
      console.log(res);
    } while (count < power)
  } else {
    return 1;
  }
  return res;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Draw stairs

function drawStairs(n){
  let a = 'I';
  let b = '\n';
  let c = ' ';
  let str = a;
  for(let i = 1; i < n; i++){
    str = str + b + c.repeat(i) + a;
  }
  return str;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Sum of Multiples

function sumMul(n,m){
  let sum = 0;
  if(n===m || m <= 0 || n <= 0){
    return "INVALID";
  }
  
  if( n > 0 ){
    for(let i = n; i <= m; i+=n){
      sum = sum + i;
    }
    return sum;
  }
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Beginner Series #3 Sum of Numbers

function getSum( a,b )
{
   var sum = 0;
   if(a === b){
     return a;
   }
   
   if(a > b){
     for(let i = b; i <= a; i++){
       sum+=i;
     }
   return sum;
   }
   
   if(a < b){
     for(let i = a; i <= b; i++){
       sum+=i;
     }
     return sum;
   }
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Sum of the first nth term of Series

function SeriesSum(n)
{
  for(var x = 0, i = 0; i < n; i++){
    x += 1 / (1 + i * 3);
  }
  return x.toFixed(2);
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
The wheat/rice and chessboard problem

function squaresNeeded(grains){
  let count = 0;
  let i = 1;
  while(i <= grains){
    i = i * 2;
    count++;
  }
  return count;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Powers of 3

function largestPower(n){
  let k = 0;
  while(3**k<n){
    k++;
  }
  return k-1;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Factorial

function factorial(n){
  let res = 1;
  let i = 1;
  while (i<=n){
    res = res * i;
    i++;
  }
  return res;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
No zeros for heros

function noBoringZeros(n) {
  while(n%10==0 && n!=0){
    n/=10;
  }
  return n;
}
 
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Power of two

function isPowerOfTwo(n){
   while(n>=2){
     n = n/2;
   }
   return n === 1 ? true : false;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Difference Of Squares

function differenceOfSquares(n){
  let x = 1;
  let sumSqr = 0;
  while(x <= n){
    sumSqr = sumSqr + (x ** 2);
    x++;
  }
  let y = 1;
  let sum = 0;
  for(let y = 1; y <= n; y++){
    sum = sum + y;
  }
  
  return (sum ** 2) - sumSqr;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
simple calculator

function calculator(a, b, sign){
  var res;
  if(typeof(a)==='number' && typeof(b)==='number') {
  switch(sign){
    case '+':
      res = a + b;
      break;
    case '-':
      res = a - b;
      break;
    case '*':
      res = a * b;
      break;
    case '/':
      res = a / b;
      break;
    default:
      res = 'unknown value';
      break;
  }
    } else {
    res = 'unknown value';
    }
  return res; 
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Basic Mathematical Operations

function basicOp(operation, value1, value2)
{
  let res;
  switch(operation){
    case '+':
      res = value1 + value2;
      break;
    case '-':
      res = value1 - value2;
      break;
    case '*':
      res = value1 * value2;
      break;
    case '/':
      res = value1 / value2;
      break;
  }
  return res;
}

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Training JS #7: if..else and ternary operator

function saleHotdogs(n){
  return n<5 ? n*100 : n>=5 && n<10 ? n*95 : n>10 ? n*90 : n*90;
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
101 Dalmatians - squash the bugs, not the dogs!

function howManyDalmatians(number){
  var dogs = ["Hardly any", "More than a handful!", "101 DALMATIANS!!!", "Woah that\'s a lot of dogs!"];
  return res = number <= 10 ? dogs[0] : number <= 50 ? dogs[1] : number === 101 ? dogs[2] : dogs[3];
}
++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Can we divide it?

function isDivideBy(number, a, b) {
  return (number/a)%1===0 && (number/b)%1===0 ? true : false;
}

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Rock Paper Scissors!

const rps = (p1, p2) => {
  return p1 === 'scissors' && p2 === 'paper' || p1 === 'rock' && p2 === 'scissors' || p1 === 'paper' && p2 === 'rock' 
  ? 'Player 1 won!' 
  : p1 === 'scissors' && p2 === 'rock' || p1 === 'paper' && p2 === 'scissors' || p1 === 'rock' && p2 === 'paper' 
  ? 'Player 2 won!' 
  : p1 === p2 ? 'Draw!' 
  : false;
};

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Is this a triangle?

function isTriangle(a,b,c)
{
   return a + b > c && b + c > a && a + c > b ? true : false;
}

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Is n divisible by x and y?

function isDivisible(n, x, y) {
  return (n / x)%1 === 0 && (n / y)%1 === 0 ? true : false;
}

++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

Calculate Two People's Individual Ages

function getAges(sum,difference){
  const arr = [];
  if(sum < 0 || difference < 0){
    return null;
    } else {
        arr.push((sum/2) + (difference/2));
        arr.push((sum/2) - (difference/2));
    }
  if(arr[0]<0 || arr[1]<0){
    return null;
  } else {
  return arr;
  }
};
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



[Area of a Square](https://www.codewars.com/kata/5748838ce2fab90b86001b1a)
```javascript
function squareArea(A){
  return Math.round((((A*4)/(2*Math.PI))**2)*100)/100;
}
```


[Formatting decimal places #0](https://www.codewars.com/kata/5641a03210e973055a00000d)
```javascript
function twoDecimalPlaces(n) {
  return (Math.round(n * 100) / 100);
}
```


[Discover The Original Price](https://www.codewars.com/kata/552564a82142d701f5001228)
```javascript
function discoverOriginalPrice(discountedPrice, salePercentage){
  return Math.floor((discountedPrice /(100 - salePercentage)* 100)*100)/100;
}
```


[Sum The Strings](https://www.codewars.com/kata/5966e33c4e686b508700002d)
```javascript
function sumStr(a,b) {
  return (Number(a)+Number(b))+ '';
}
```


[Number toString](https://www.codewars.com/kata/53934feec44762736c00044b)
```javascript
public class Kata
{
  public static string A = 123.ToString();
}
```


[The Wide-Mouthed frog!](https://www.codewars.com/kata/57ec8bd8f670e9a47a000f89)
```javascript
function mouthSize(animal) {
  if(animal == 'alligator'){
    return 'small';
  } if(animal == 'ALLIGATOR') {
    return 'small';
  } else {
    return 'wide';
  }
}
```


[Super Duper Easy](https://www.codewars.com/kata/55a5bfaa756cfede78000026)
```javascript
function problem(x){
  if(typeof x === 'string'){
    return 'Error';
  } else {
    return x * 50 + 6;
  }
}
```


[Convert boolean values to strings 'Yes' or 'No'](https://www.codewars.com/kata/53369039d7ab3ac506000467)
```javascript
function boolToWord( bool ){
  if(bool === true){
    return 'Yes';
  } else {
    return 'No';
  }
}
```


[Sum of angles](https://www.codewars.com/kata/5a03b3f6a1c9040084001765)
```javascript
function angle(n) {
  return 180*(Math.round(n-2));
}
```


[For Twins: 2. Math operations](https://www.codewars.com/kata/59c287b16bddd291c700009a)
```javascript
function iceBrickVolume(radius, bottleLength, rimLength) {
  let brickSide = (radius*2)/(2**0.5);
  let brickHeight = Math.round(bottleLength - rimLength);
  return Math.round(brickHeight*brickSide*brickSide);
}
```


[Breaking chocolate problem](https://www.codewars.com/kata/534ea96ebb17181947000ada)
```javascript
function breakChocolate(n,m) {
  let cut = 0;
  if(n === 0 || m === 0){
    return 0;
  } else {
    return n*m-1;
  }
}
```


[Training JS #1: create your first JS function and print "Helloworld!"](https://www.codewars.com/kata/training-js-number-1-create-your-first-js-function-and-print-helloworld/javascript)
```javascript
function helloWorld(){
var str = "Hello World!";
console.log(str);
return str;
}
console.log(helloWorld());
```
