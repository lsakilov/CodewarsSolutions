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

```javascript
for (let i = 1; i <= 10; i++) {     
  for (let j = 1; j <= 10; j++) {
    console.log(`${i} * ${j} = ${i * j}`);
  }

  console.log('--------------');  // строка, разделяющая столбцы таблицы умножения
}
```


[Power](https://www.codewars.com/kata/562926c855ca9fdc4800005b)
```javascript
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
```


[Draw stairs](https://www.codewars.com/kata/5b4e779c578c6a898e0005c5)
```javascript
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
```


[Sum of Multiples](https://www.codewars.com/kata/57241e0f440cd279b5000829)
```javascript
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
```


[Beginner Series #3 Sum of Numbers](https://www.codewars.com/kata/55f2b110f61eb01779000053)
```javascript
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
```


[Sum of the first nth term of Series](https://www.codewars.com/kata/555eded1ad94b00403000071)
```javascript
function SeriesSum(n)
{
  for(var x = 0, i = 0; i < n; i++){
    x += 1 / (1 + i * 3);
  }
  return x.toFixed(2);
}
```


[The wheat/rice and chessboard problem](https://www.codewars.com/kata/5b0d67c1cb35dfa10b0022c7)
```javascript
function squaresNeeded(grains){
  let count = 0;
  let i = 1;
  while(i <= grains){
    i = i * 2;
    count++;
  }
  return count;
}
```


[Powers of 3](https://www.codewars.com/kata/57be674b93687de78c0001d9)
```javascript
function largestPower(n){
  let k = 0;
  while(3**k<n){
    k++;
  }
  return k-1;
}
```


[Factorial](https://www.codewars.com/kata/57a049e253ba33ac5e000212)
```javascript
function factorial(n){
  let res = 1;
  let i = 1;
  while (i<=n){
    res = res * i;
    i++;
  }
  return res;
}
```


[No zeros for heros](https://www.codewars.com/kata/570a6a46455d08ff8d001002)
```javascript
function noBoringZeros(n) {
  while(n%10==0 && n!=0){
    n/=10;
  }
  return n;
}
```

 
[Power of two](https://www.codewars.com/kata/534d0a229345375d520006a0)
```javascript
function isPowerOfTwo(n){
   while(n>=2){
     n = n/2;
   }
   return n === 1 ? true : false;
}
```


[Difference Of Squares](https://www.codewars.com/kata/558f9f51e85b46e9fa000025)
```javascript
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
```


[simple calculator](https://www.codewars.com/kata/5810085c533d69f4980001cf)
```javascript
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
```


[Basic Mathematical Operations](https://www.codewars.com/kata/57356c55867b9b7a60000bd7)
```javascript
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
```


[Training JS #7: if..else and ternary operator](https://www.codewars.com/kata/57202aefe8d6c514300001fd)
```javascript
function saleHotdogs(n){
  return n<5 ? n*100 : n>=5 && n<10 ? n*95 : n>10 ? n*90 : n*90;
}
```


[101 Dalmatians - squash the bugs, not the dogs!](https://www.codewars.com/kata/56f6919a6b88de18ff000b36)
```javascript
function howManyDalmatians(number){
  var dogs = ["Hardly any", "More than a handful!", "101 DALMATIANS!!!", "Woah that\'s a lot of dogs!"];
  return res = number <= 10 ? dogs[0] : number <= 50 ? dogs[1] : number === 101 ? dogs[2] : dogs[3];
}
```


[Can we divide it?](https://www.codewars.com/kata/5a2b703dc5e2845c0900005a)
```javascript
function isDivideBy(number, a, b) {
  return (number/a)%1===0 && (number/b)%1===0 ? true : false;
}
```


[Rock Paper Scissors!](https://www.codewars.com/kata/5672a98bdbdd995fad00000f)
```javascript
const rps = (p1, p2) => {
  return p1 === 'scissors' && p2 === 'paper' || p1 === 'rock' && p2 === 'scissors' || p1 === 'paper' && p2 === 'rock' 
  ? 'Player 1 won!' 
  : p1 === 'scissors' && p2 === 'rock' || p1 === 'paper' && p2 === 'scissors' || p1 === 'rock' && p2 === 'paper' 
  ? 'Player 2 won!' 
  : p1 === p2 ? 'Draw!' 
  : false;
};
```


[Is this a triangle?](https://www.codewars.com/kata/56606694ec01347ce800001b)
```javascript
function isTriangle(a,b,c)
{
   return a + b > c && b + c > a && a + c > b ? true : false;
}
```


[Is n divisible by x and y?](https://www.codewars.com/kata/5545f109004975ea66000086)
```javascript
function isDivisible(n, x, y) {
  return (n / x)%1 === 0 && (n / y)%1 === 0 ? true : false;
}
```


[Calculate Two People's Individual Ages](https://www.codewars.com/kata/58e0bd6a79716b7fcf0013b1)
```javascript
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
```


[Alan Partridge II - Apple Turnover](https://www.codewars.com/kata/580a094553bd9ec5d800007d)
```javascript
function apple(x){
  return res = +(x ** 2 > 1000) ? "It\'s hotter than the sun!!" : "Help yourself to a honeycomb Yorkie for the glovebox.";
}
```


[Calculate BMI](https://www.codewars.com/kata/57a429e253ba3381850000fb)
```javascript
function bmi(weight, height) {
  return res = (weight / height ** 2) <= 18.5 ? "Underweight" : (weight / height ** 2) <= 25.0 ? "Normal" : (weight / height ** 2) <= 30.0 ? "Overweight" : "Obese";
}
```


[What's the real floor?](https://www.codewars.com/kata/574b3b1599d8f897470018f6)
```javascript
function getRealFloor(n) {
  return real = n <= 0 ? n : n > 12 ? n - 2 : n - 1;
}
```


[Even or Odd](https://www.codewars.com/kata/53da3dbb4a5168369a0000fe)
```javascript
even_or_odd = number => return msg = number % 2 === 0 ? msg = 'Even' : msg = 'Odd';

function even_or_odd(number) {
  return msg = number % 2 === 0 ? msg = 'Even' : msg = 'Odd';
}
```

```javascript
function even_or_odd(number) {
  let msg;
   if(number % 2 === 0){
     msg = 'Even';
   } else {
     msg = 'Odd';
    }
   return msg;
}
```


[Is he gonna survive?](https://www.codewars.com/kata/59ca8246d751df55cc00014c)
```javascript
function hero(bullets, dragons){
  return (bullets / 2) >= dragons ? true : false;
}
```


[Simple Comparison?](https://www.codewars.com/kata/57f6ecdfcca6e045d2001207)
```javascript
function add(a, b){
	return a == b ? true : false;
}
```


[Chuck Norris VII - True or False? (Beginner)](https://www.codewars.com/kata/570669d8cb7293a2d1001473)
```javascript
function ifChuckSaysSo(){
  return 10 > 12;
}
```


[Keep up the hoop](https://www.codewars.com/kata/55cb632c1a5d7b3ad0000145)
```javascript
function hoopCount (n) {
   return msg = n >= 10 ? "Great, now move on to tricks" : "Keep at it until you get it";
}
```


[Be Concise I - The Ternary Operator](https://www.codewars.com/kata/56f3f6a82010832b02000f38)
```javascript
let describeAge = age => "You're a(n) " + (age <13? "kid" : age < 18? "teenager" : age < 65?
    "adult" : "elderly");
```


[Century From Year](https://www.codewars.com/kata/5a3fe3dde1ce0e8ed6000097)
```javascript
function century(year) {
  return Math.ceil(year/100);
}
```


[Count Odd Numbers below n](https://www.codewars.com/kata/59342039eb450e39970000a6)
```javascript
function oddCount(n){
  return Math.floor(n / 2);
}
```

```javascript
const closestMultiple10 = num => {
  return (Math.round(num*0.1))*10;
};
```


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


[Is integer safe to use?](https://www.codewars.com/kata/55a4f9afeffe4231090000d6/javascript)
```javascript
function SafeInteger(n) {
  return Number.isSafeInteger(n);
}
```


[Return Negative](https://www.codewars.com/kata/55685cd7ad70877c23000102/javascript)
```javascript
function makeNegative(num) {
  return -(Math.abs(num));
}
```


[Invert values](https://www.codewars.com/kata/5899dc03bc95b1bf1b0000ad/javascript)
```javascript
function invert(array) {
   newArray = [];
     for(let i = 0; i < array.length; i++){
       newArray.push(array[i] * -1);
     };
   return newArray;
}
```


[BASIC: Making Six Toast.](https://www.codewars.com/kata/5834fec22fb0ba7d080000e8/javascript)
```javascript
function sixToast(num) {
  return num == 6 ? 0 : num < 6 ? 6 - num : num - 6;
}
```

[Closest elevator](https://www.codewars.com/kata/5c374b346a5d0f77af500a5a/javascript)
```javascript
function elevator(left, right, call){
  return Math.abs(right - call) <= Math.abs(left - call)  ? 'right' : 'left';
}
```

[Square Every Digit](https://www.codewars.com/kata/546e2562b03326a88e000020/javascript)
```javascript
function squareDigits(num){
  let numString = num.toString()
  let arr = []
  
  for(var i = 0; i < numString.length; i++) {
    arr[i] = numString[i] * numString[i]
  }
  return Number(arr.join('')) 
}
```

[Squares sequence](https://www.codewars.com/kata/5546180ca783b6d2d5000062/javascript)
```javascript
function squares(x, n) {
  if(n<=0){
    return [];
  } else {
      const arr = [x];
      let y = x;
      for(let i = 1; i < n; i++){
        y = Math.pow(y, 2);
      arr.push(y);
    }
    return arr;
  }
}
```


[To square(root) or not to square(root)](https://www.codewars.com/kata/57f6ad55cca6e045d2000627/javascript)
```javascript
function squareOrSquareRoot(array) {
  let arr = [];
  for(let i = 0; i <array.length; i++){
    if(Math.sqrt(array[i])%1==0){
      arr.push(Math.sqrt(array[i]));
    } else {
      arr.push(Math.pow(array[i], 2));
    }
  }
  return arr; 
}
```


[You're a square!](https://www.codewars.com/kata/54c27a33fb7da0db0100040e/javascript)
```javascript
function isSquare(n){
  return Math.sqrt(n)%1 === 0;
}
```

[Find the next perfect square!](https://www.codewars.com/kata/56269eb78ad2e4ced1000013/javascript)
```javascript
function findNextSquare(sq) {
  var sqRt = Math.sqrt( sq );
  if ( NaN === sqRt || sqRt !== parseInt( sqRt, 10 ) ) {
    return -1;
  }
  return Math.pow( sqRt + 1, 2 );
}
```
[Beginner Series #4 Cockroach](https://www.codewars.com/kata/55fab1ffda3e2e44f00000c6/javascript)
```javascript
function cockroachSpeed(s) {
  return Math.floor(s*100000/3600);
}
```

[Price of Mangoes](https://www.codewars.com/kata/57a77726bb9944d000000b06/javascript)
```javascript
function mango(quantity, price){
  return (quantity-Math.floor(quantity/3))*price;
}
```

[Holiday VIII - Duty Free](https://www.codewars.com/kata/57e92e91b63b6cbac20001e5/javascript)
```javascript
function dutyFree(normPrice, discount, hol){
  let discountNum = (normPrice/100)*discount;
  return Math.floor(hol/discountNum);
}
```

[All Star Code Challenge #22](https://www.codewars.com/kata/5865cff66b5699883f0001aa/javascript)
```javascript
function toTime(seconds) {
  let convertToHoures = Math.floor(seconds/3600);
  let convertToMinutes = Math.floor((seconds/60)%60);
  return (convertToHoures + ' hour(s) and ' + convertToMinutes + ' minute(s)');
}
```

[How many times should I go?](https://www.codewars.com/kata/57efcb78e77282f4790003d8/javascript)
```javascript
function howManyTimes(annualPrice, individualPrice) {
  return Math.ceil(annualPrice/individualPrice);
}
```

[Hello, Name or World!](https://www.codewars.com/kata/57e3f79c9cb119374600046b/train/javascript)
```javascript
function hello(name) {
  if(name === '' || name === undefined){
    return 'Hello, World!';
  } else {
    let nameAdjusted = name.toLowerCase();
      return 'Hello, ' + nameAdjusted[0].toUpperCase() + nameAdjusted.slice(1) + '!';
    }
}
```

[Grasshopper - Function syntax debugging](https://www.codewars.com/kata/56dae9dc54c0acd29d00109a/train/javascript)
```javascript
function main (verb, noun){
  return verb + noun;
}
```

[Grasshopper - Debug sayHello](https://www.codewars.com/kata/5625618b1fe21ab49f00001f/train/javascript)
```javascript
function sayHello(name) {
  return 'Hello, ' + name;
}
```

[Evens and Odds](https://www.codewars.com/kata/583ade15666df5a64e000058/train/javascript)t
```javascript
function evensAndOdds(num){
    return num % 2 === 0 ? (num).toString(2) : (num).toString(16);
}
```

[Evens and Odds](https://www.codewars.com/kata/583ade15666df5a64e000058/train/javascript)t
```javascript


```
