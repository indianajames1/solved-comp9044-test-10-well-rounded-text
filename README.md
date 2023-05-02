Download Link: https://assignmentchef.com/product/solved-comp9044-test-10-well-rounded-text
<br>
<h1></h1>

Write a program remove_repeats.pl which takes 0 or more arguments and prints some of those arguments.

The first occurrence and only the first occurrence of any argument should be printed.

The arguments should be printed on a single line. A single space should separate each argument.

Your program can NOT assume the arguments with be in any particular order.

Make your program behave exactly as indicated by the examples below.

It must produce exactly the same output as below, except you may print an extra space at the end of the line if you wish.

Your program must be Perl.

For example:

<table width="961">

 <tbody>

  <tr>

   <td width="961">$ <strong>remove_repeats.pl </strong>$ <strong>remove_repeats.pl bird</strong> bird$ <strong>remove_repeats.pl bird cow fish</strong> bird cow fish$ <strong>remove_repeats.pl echo echo echo</strong> echo$ <strong>remove_repeats.pl bird cow fish bird cow fish bird</strong> bird cow fish$ <strong>remove_repeats.pl how much wood would a woodchuck chuck</strong> how much wood would a woodchuck chuck $ <strong>remove_repeats.pl a a a a b a</strong> a b$ <strong>remove_repeats.pl a b c d c b a</strong> a b c d$ <strong>remove_repeats.pl d c b d c a a d</strong> d c b a</td>

  </tr>

 </tbody>

</table>

When you think your program is working you can autotest to run some simple automated tests:

$ <strong>2041 autotest remove_repeats</strong>

When you are finished working on this exercise you must submit your work by running give:

$ <strong>give cs2041 test10_remove_repeats remove_repeats.pl</strong>

Write a program text_round.plthat copies its standard input to standard output but maps all numbers to their nearest whole number equivalent. For example, 0.667 would be mapped to 1, 99.5 would be mapped to 100, 16.35 would be mapped to 16, and so on. All other text in the input should be transferred to the output unchanged.

A <em>number</em> is defined as a string containing some digit characters with an optional decimal point (‘.’) followed by zero or more additional digit characters.

For example 0, 100, 3.14159, 1000.0, 0.999 and 12345. are all valid numbers.

For example, given this input:

I spent $15.50 for 3.3kg of apples yesterday.

Pi is approximately 3.141592653589793 2000 is a leap year, 2001 is not.

your program should produce this output:

I spent $16 for 3kg of apples yesterday.

Pi is approximately 3

2000 is a leap year, 2001 is not.

For example:

<table width="961">

 <tbody>

  <tr>

   <td width="961">$ <strong>cat text_round_input.txt</strong>I spent $15.50 for 3.3kg of apples yesterday.Pi is approximately 3.141592653589793 2000 is a leap year, 2001 is not.$ <strong>text_round.pl &lt;text_round_input.txt</strong>I spent $16 for 3kg of apples yesterday.Pi is approximately 32000 is a leap year, 2001 is not.</td>

  </tr>

 </tbody>

</table>

When you think your program is working you can autotest to run some simple automated tests:

$ <strong>2041 autotest text_round</strong>

When you are finished working on this exercise you must submit your work by running give:

$ <strong>give cs2041 test10_text_round text_round.pl</strong>

Write a program reference.pl that reads lines of text from its standard input and prints them to its standard output. Except for lines which contain with a ‘#’ character followed by a positive integer.

Lines of the form #n (where n is an integer value), should be replaced this by the n’th line of input.

This transformation only applies to lines which start with a # character, followed by the digits of a positive integer and then the newline character. No other characters appear on such lines.

You may assume:

Lines are numbered starting from 1,

There are no more than 100 lines in the input,

No line is more than 80 characters long, All n values are valid input line numbers, No n values refer to other #n lines.

For example:

<table width="961">

 <tbody>

  <tr>

   <td width="961">$ <strong>cat reference_input.txt</strong> line A line B line C #7 line D #2 line E$ <strong>reference.pl &lt;reference_input.txt</strong> line A line B line C line E line D line B line E</td>

  </tr>

 </tbody>

</table>

When you think your program is working you can autotest to run some simple automated tests:

$ <strong>2041 autotest reference</strong>

When you are finished working on this exercise you must submit your work by running give:

$ <strong>give cs2041 test10_reference reference.pl</strong>