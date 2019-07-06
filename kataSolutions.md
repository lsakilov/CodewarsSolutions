https://www.codewars.com/kata/print-a-rectangle-using-asterisks/train/javascript
Write a method that, given two arguments, width and height, returns a string representing a rectangle with those dimensions.

The rectangle should be filled with spaces, and its borders should be composed of asterisks (*).

For example, the following call:

getRectangleString(3, 3);
Should return the following string:

***
* *
***
End each line of the string (including the last one) with a carriage return-line feed combination.

Note: You may assume that width and height will always be greater than zero.

function getRectangleString(w, h) {
  const rn = '\r\n';
  const tb = '*'.repeat(w) + rn;
  const center = (w > 1) ? ('*' + ' '.repeat(w - 2) + '*' + rn).repeat(h - 2) : ''; 
  return h > 1 ? (tb + center + tb) : tb.repeat(h);
}