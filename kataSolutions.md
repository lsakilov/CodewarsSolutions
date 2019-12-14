
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
