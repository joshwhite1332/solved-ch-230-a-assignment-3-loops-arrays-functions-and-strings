Download Link: https://assignmentchef.com/product/solved-ch-230-a-assignment-3-loops-arrays-functions-and-strings
<br>
<h1>Problem 3.1 <em>Writing numbers                                                                                      </em></h1>

Write a program where you first enter a float x and then an integer n from the keyboard. Print the float xn times to the screen. Make sure that n will have a valid integer value. In the invalid case repeat entering n until a valid value will be entered.

<em>Your solution has to satisfy the requirements from the problem description and has to pass the following testcase and potentially other testcases which are uploaded. All characters are relevant for passing testcases including newlines and spaces.</em>

<table width="564">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 3.1: input</strong>1.25-804</td>

   <td width="274"><strong>Testcase 3.1: output</strong>Input is invalid, reenter valueInput is invalid, reenter value1.2500001.2500001.2500001.250000</td>

  </tr>

  <tr>

   <td width="290"><strong>Problem 3.2 </strong><em>Writing characters</em></td>

   <td width="274"> </td>

  </tr>

 </tbody>

</table>

<h2><strong>Language: C</strong></h2>

Write a program where you first enter a lowercase character ch and then an integer n from the keyboard. Print the characters ch, ch−1, …, ch−n on the screen.

You can safely assume that the input is valid and you do not have to do any checks.

<h1>Problem 3.3 <em>Centimeters to kilometers                                                                       </em></h1>

Write a program that converts an integer length that is entered from the keyboard in cm to km.

Write and use a function float convert(int cm) that does the actual conversion.

<em>You can safely assume that the input will be valid.</em>

<em>Your solution has to satisfy the requirements from the problem description and has to pass the following testcase and potentially other testcases which are uploaded. All characters are relevant for passing testcases including newlines and spaces.</em>

<h1>Testcase 3.3: inputTestcase 3.3: output</h1>

12Result of conversion: 0.000120

<h2><strong>Problem 3.4 </strong>Wrong position</h2>

The program below should print the position of the first occurrence of the character ’g’ within a

string. You can safely assume that ’g’ will be contained in the string. Why does it always print the position 0? Fix the program such that it prints the correct position.

#include &lt;stdio.h&gt;

int position(char str[], char c)

{ int idx;

/* Loop until end of string */ for (idx = 0; str[idx] != c &amp;&amp; str[idx] != ’ ’; ++idx)

/* do nothing */ return idx;

}

int main() { char line[80]; while (1) { printf(“Enter string:
”); fgets(line, sizeof(line), stdin); printf(“The first occurrence of ’g’ is: %d
”, position(line, ’g’));

}

}

<h2><strong>Problem 3.5 </strong>Computing the average of temperature values</h2>

Write a program where you first enter a character c followed by an integer n and n double values representing temperatures in Celsius. Use an array for storing the temperatures. You can assume that not more than 100 temperature values would be entered. Your program should compute and/or print the following: if c is ’s’ the sum of the temperatures, if c is ’p’ the list of all temperatures, if c it ’t’ the list of all temperatures in Fahrenheit and if another character was entered then the arithmetic mean (or average) of all temperatures. The formula for converting Celsius to Fahrenheit is the following:

<em>.</em>

<em>Use a switch instruction in your solution.</em>

<em>You can safely assume that the input will be valid.</em>

<h2><strong>Problem 3.6 </strong>Kilograms and grams to pounds</h2>

Write a program that converts the units of mass kg and g to pounds. First read the weight of an object expressed by values for kilograms and grams from the keyboard and convert the units of mass using the function (written by you as well)

float to_pounds(int kg, int g); that does the actual conversion. Note that: 1 kilogram =2<em>.</em>2 pounds

<em>You can safely assume that the input will be valid.</em>

<em>Your solution has to satisfy the requirements from the problem description and has to pass the following testcase and potentially other testcases which are uploaded. All characters are relevant for passing testcases including newlines and spaces.</em>

<h1>Testcase 3.6: inputTestcase 3.6: output</h1>

5Result of conversion: 11.220000

100

<h2><strong>Problem 3.7 </strong>Printing a form</h2>

<strong>Due by Monday, September 27<sup>th</sup>, 23:00</strong>

<h3>Language: C</h3>

Write a program which reads two integers n, m and a character c from the keyboard. This program should define and call a function with the prototype:

void printform(int n, int m, char c);

which prints a trapezoid of height n, bases m and m+n-1 consisting of the character c as in the following testcase.

<table width="431">

 <tbody>

  <tr>

   <td width="274"><strong>Testcase 3.7: input</strong>43$</td>

   <td width="157"><strong>Testcase 3.7: output</strong>$$$$$$$$$$$$</td>

  </tr>

 </tbody>

</table>

$$$$$$

<em>You can safely assume that the input will be valid.</em>

<h2><strong>Problem 3.8 </strong>Computing sum and average</h2>

<h3>Language: C</h3>

Write a program where you can enter from the keyboard up to 10 floats. If the number entered is equal to −99<em>.</em>0, stop reading numbers from the keyboard and compute the sum and average of all values (excluding −99<em>.</em>0) using two functions (one for the sum and one for the average). Print your results on the screen.

<em>You can safely assume that the input will be valid.</em>

<em>Make sure you consider all the cases: less than </em>10 <em>numbers might be entered. After all the numbers have been entered you need to make sure that the sum and average are computed.</em>

<h2><strong>Problem 3.9 </strong>Determine sum of two values in array</h2>

<h3>Language: C</h3>

Write a program which reads from the keyboard an integer value n followed by n double values as elements of an array with not more than 20 elements. Write also a function with the prototype:

double sum25(double v[], int n);

which computes and returns the sum of the elements in v at position 2 and position 5. Check that positions 2 and 5 are valid within v, if not then print a corresponding message on the screen. In this case the function should return the value −111. Print the sum on the screen.

<em>Your solution has to satisfy the requirements from the problem description and has to pass the following testcase and potentially other testcases which are uploaded. All characters are relevant for passing testcases including newlines and spaces.</em>

<table width="431">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 3.9: input</strong>6</td>

   <td width="141"><strong>Testcase 3.9: output</strong>sum=0.000000</td>

  </tr>

 </tbody>

</table>

1.5

1.5

1.5

1.5

1.5

-1.5

<h2><strong>Problem 3.10 </strong>Return changes by reference</h2>

Write a program which reads two float values from the keyboard. Then write three functions. The first function should return the product of the two float values and should have the prototype:

float product(float a, float b);

The second function should return the product of the two float values by reference and should have the prototype:

void productbyref(float a, float b, float *p);

The third function should add 3 to the first float and 11 to the second float and return the change by reference. It should have the prototype:

void modifybyref(float *a, float *b);

Show that the calls of the first two functions have the same effect. Also show what is the effect of calling modifybyref.

<em>You can safely assume that the input will be valid.</em>

<h2><strong>Problem 3.11 </strong>Working with strings</h2>

Write a program where you can enter two strings called one and two from the keyboard. The string should be able to contain spaces. The program should do the following:

<ol>

 <li>Print on the screen the lengths of both strings,</li>

 <li>Print on the screen the concatenation of one with two,</li>

 <li>Declare a third string, copy correctly two into it and print the third string to the screen,</li>

 <li>Compare the two strings two and one and print a corresponding message to the screen,</li>

 <li>Read a character c from the keyboard and search for c in two. The position of the first occurrence of c within two should be printed to the screen. If the character is not contained in the string then print a corresponding message on the screen.</li>

</ol>

For solving this problem use the string functions from string.h.

<em>Learn how to use them with the help of the man pages.</em>

<em>Your solution has to satisfy the requirements from the problem description and has to pass the following testcase and potentially other testcases which are uploaded. All characters are relevant for passing testcases including newlines and spaces.</em>

<table width="585">

 <tbody>

  <tr>

   <td width="290"><strong>Testcase 3.11: input</strong>first string hello world l</td>

   <td width="295"><strong>Testcase 3.11: output</strong>length1=12 length2=11 concatenation=first stringhello world</td>

  </tr>

 </tbody>

</table>

copy=hello world one is smaller than two position=2