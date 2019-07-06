https://www.codewars.com/kata/spongebob-meme/train/javascript
Remember the spongebob meme that is meant to make fun of people by repeating what they say in a mocking way?


You need to create a function that converts the input into this format, with the output being the same string expect there is a pattern of uppercase and lowercase letters.

function spongeMeme(s) {
  let str = '';
  for(let i = 0; i < s.length; i++){
    if(i % 2 == 0){
      str += s[i].toUpperCase();
    } else {
      str += s[i].toLowerCase();
    }
  }
  return str;
}