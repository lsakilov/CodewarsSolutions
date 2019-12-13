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
