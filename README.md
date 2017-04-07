# Javascript Problems

1 - Zero to Twenty
Write a function called **generateZeroToTwenty** that returns an array of integers from 0 to 20, inclusive.

~~~javascript
function generateZeroToTwenty() {
	var display = [];
	for(var i = 0; i < 21; i++) {
		display.push(i);
	}
		return display;
}
generateZeroToTwenty();
~~~
2 - Twenty to Zero
Write a function called **generateTwentyToZero** that returns an array of integers from 20 to 0 in descending order.

~~~javascript
function generateTwentyToZero() {
	var display = [];
	for(var i = 20; i > 0; i--) {
		display.push(i);
	}
		return display;
}
generateTwentyToZero();
~~~
3 - Even Numbers
Write a function called **generateEvenNumbers** that will return an array of even numbers between 0 and 20, inclusive.

~~~javascript
function generateEvenNumbers() {
	var display = [];
	for(var i = 0; i < 21; i++) {
		if(i % 2 === 0) {
			display.push(i);
		}
	}
			return display;	
}
generateEvenNumbers();
~~~
4 - Multiply By Nine
Write a function called **multiplyByNine** that accepts an array of integers. It returns an array-of-arrays containing the original integers and each integer multiplied by 9.

For example, given the input array [1,2,3], 
it should return [[1,9],[2,18],[3,27]].

~~~javascript
var inputArray = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
function multiplyByNine(inputArray) {
    var display = [];
    for(var i = 1; i < inputArray.length + 1; i++) {
        display.push([i, i * 9]);
    }
    return display;
}
multiplyByNine(inputArray);
~~~
5 - Add Arrays
Write a function that adds 2 given arrays of numbers, of the same length.

Example: sumArrays([1,2,3], [4,5,6]) ⇒ [5,7,9]

~~~javascript
var twoArray = [6, 7, 8, 9, 10];
function sumArrays(oneArray, twoArray) {
	var bothArrays = [];
    for(var i = 0; i < oneArray.length; i++) {
        bothArrays.push(oneArray[i] + twoArray[i]);
        }
    return bothArrays;
}
sumArrays(oneArray, twoArray);
~~~
6 - Max Value in Array
Write a function that finds the maximum value in a given array. Do not use Math.max

~~~javascript
var oneArray = [9, 1, 10, 2, 8, 3, 7, 4, 6, 5,];
function Max(oneArray) {
	result = oneArray[0];
    for(var i = 0; i < oneArray.length; i++) {
    	if(oneArray[i] > result) {
    		result = oneArray[i];
        }
    	return result;
	}
}
Max(oneArray);
~~~
7 - Average Values
Write a function that averages a given array of numbers.

~~~javascript
var oneArray = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
function avgArray(oneArray) {
    var sum = 0;
    for(var i = 0; i < oneArray.length; i++) {
        sum += oneArray[i];
    }
    return sum / oneArray.length;
}
avgArray(oneArray);
~~~
8 - Alternate operators
Write a function that adds and subtracts a given array of numbers in alternation and returns the result. For example, given [1,2,3,4,5], it should return -1, because 1+2-3+4-5=-1

~~~javascript
var oneArray = [1, 2, 3, 4, 5];
var addArray = function (oneArray) {
    var display = oneArray[0];
    for(var i = 1; i < oneArray.length; i++) {
        if(i % 2 === 0) {
        	display -= oneArray[i];
    }	else	{
    		display += oneArray[i];
    }
    }
    	return display;
};
addArray(oneArray);
~~~
9 - Line o' Asterisks
Write a function that returns a horizontal line of asterisks of a specified length.

Don't just write this out to the log -- actually return the string.

~~~javascript
function lineOfAsteriks(Number) {
	var display = [];
    for(var i = 0; i < Number; i++) {
    display += "*";
    }
    return display;
}
lineOfAsteriks(60);
~~~
10 - Draw a Right Triangle
Write a function called drawTriangle that returns the following string. Feel free to debug-print using console.log, but make sure that the function actually returns a string. 

Note that in a string, the character for a carriage return (the equivalent of hitting the “Enter” or “Return” key) is “\n”.

~~~javascript
function drawTriangle() {
    	return "#\n" + "##\n" + "###\n" + "####\n" + "#####\n" 
    	+ "######\n" + "#######\n" + "########\n" + "#########\n" 
    	+ "##########";
}
drawTriangle();
~~~
