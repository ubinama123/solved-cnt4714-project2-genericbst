Download Link: https://assignmentchef.com/product/solved-cnt4714-project2-genericbst
<br>
In this assignment, you will gain experience working with generics in Java. In particular, you will extend my binary search tree (BST) code from a data structure that just holds integers to a powerful container that can hold any kind of Comparable object under the sun.

A tangential benefit of this program is that you get to spend some time looking through some fairly straight-forward and well-structured BST code. It is always good to revisit how common data structures can be implemented as you ramp up your skills in different programming languages. You will also gain experience modifying someone else’s code (something you will be doing a lot if you become a software developer) and adding comments to code.

<h1>Deliverables</h1>

GenericBST.java

<strong><em>Note!</em></strong> The capitalization and spelling of your filename matter!

<strong><em>Note!</em></strong> Code must be tested on Eustis, but submitted via Webcourses.

<h1>1.        Problem Statement</h1>

Included with this assignment is a source file named <em>BST.java</em>. You must modify that file as follows:

<ol>

 <li>Change the class name to <em>GenericBST</em> and the file name to <em>java</em>.</li>

 <li>Modify the source code so that the class is generic (i.e., so that the binary search trees will be able to hold any type of data) with the restriction that only classes that implement <em>Comparable</em> may be stored in the BSTs. As with <em>java</em> (<a href="https://webcourses.ucf.edu/courses/1330842/pages/generics-and-interfaces-in-java">posted in Webcourses</a><a href="https://webcourses.ucf.edu/courses/1330842/pages/generics-and-interfaces-in-java">)</a>, you do <em>not</em> need to write a <em>compareTo()</em> method.</li>

 <li>The comments in <em>java</em> are practically non-existent. After you have read and absorbed the program’s structure and functionality, add comments for the entire program. (See the commenting guidelines below.)</li>

 <li>Write a <em>public static double difficultyRating()</em> method that returns a double on the range of 1.0 (ridiculously easy) through 5.0 (insanely difficult) indicating how difficult you found this assignment.</li>

 <li>Write a <em>public static double hoursSpent()</em> method that returns a realistic and reasonable estimate (greater than zero) of the number of hours you spent working on this assignment.</li>

</ol>

To make this class generic, you will have to change the return types of some of the methods I have implemented. However, please do not change static methods to non-static methods, or private methods to public methods, and vice-versa.

<h1>2.        Special Requirement: No Compile-Time Warnings (<em>Super Important!</em>)</h1>

Here are some special restrictions regarding compile-time warnings:

 Your code must not produce any warnings when compiled on Eustis. For this particular assignment, it’s especially important not to have any <em>-Xlint:unchecked</em> warnings. Please note that some systems don’t produce <em>-Xlint:unchecked</em> warnings! The safest way to check whether your code is producing such warnings is to compile and run your program on Eustis with the <em>test-all.sh</em> script.

 You cannot use the <em>@SuppressWarnings</em> annotation (or any similar annotations) to suppress warnings in this assignment.

Please do not give your code to classmates and ask them to check whether their compilers generate compile-time warnings for your code. Remember, sharing code in this course is out of bounds for assignments.

<h1>3.        General Commenting Guidelines</h1>

Here are some guidelines to follow when adding comments to <em>GenericBST.java</em> or when commenting your own code this semester:  Keep comments brief. In general, try to avoid comments that exceed two or three lines. Note that the comments in my code in Webcourses are designed for educational reading. They’re far more lengthy and verbose than anything you should be including in your own code.

 In general, above each method signature, give a high-level overview of what that method does. Say something about its input parameters, expected output, and return value (if applicable).

 Within your methods, give high-level comments that tell what different chunks of code do (rather than commenting every single line of code). However:

 Avoid simply repeating things that are “obvious” in your code, thereby making someone read your code twice (once in English and once in Java). That is, avoid <a href="http://ninjawords.com/transliterate">transliterating</a> your code from Java to English.

 Prefer comments that tell <em>how</em> or <em>why </em>something works, rather than simply saying <em>what</em> something does, unless you’re explaining the behavior of a chunk of code in a way that makes your code easier for a reader to digest.

 When writing comments, a good rule of thumb is this: Suppose you load up your code for an assignment five years from now, and you’ve lost the PDF for that assignment. What comments would help you quickly understand what you were doing and how each of the methods plays into your program’s overall functionality?  Try to use method names that are verb phrases, which therefore act as documentation of what your code is doing. (Avoid obscure method and variable names that would require us to add clarifying comments everywhere they appear.)

 Don’t copy and paste method descriptions from the assignment PDFs, as they sometimes contain nonstandard characters that will prevent your code from compiling. (Also, the method descriptions in the PDFs are often way too verbose. You should write shorter overviews for each of your methods.)

<h1>4.        Style Restrictions (Same as in Program #1) (<em>Super Important!</em>)</h1>

Please conform as closely as possible to the style I use while coding in class. To encourage everyone to develop a commitment to writing consistent and readable code, the following restrictions will be strictly enforced:

 Capitalize the first letter of all class names. Use lowercase for the first letter of all method names.

 Any time you open a curly brace, that curly brace should start on a new line.

 Any time you open a new code block, indent all the code within that code block one level deeper than you were already indenting.

 Be consistent with the amount of indentation you’re using, and be consistent in using either spaces or tabs for indentation throughout your source file. If you’re using spaces for indentation, please use at least two spaces for each new level of indentation, because trying to read code that uses just a single space for each level of indentation is downright painful.

 Please avoid block-style comments: /*<em> comment </em>*/

 Instead, please use inline-style comments: //<em> comment</em>

 Always include a space after the “//” in your comments: “// <em>comment</em>” instead of “//<em>comment</em>”

 The header comments introducing your source file (including the comment(s) with your name, course number, semester, NID, and so on), should always be placed <em><u>above</u></em> your import statements.

 Use end-of-line comments sparingly. Comments longer than three words should always be placed <em><u>above</u></em> the lines of code to which they refer. Furthermore, such comments should be indented to properly align with the code to which they refer. For example, if line 16 of your code is indented with two tabs, and line 15 contains a comment referring to line 16, then line 15 should also be intended with two tabs.

 Please do not write excessively long lines of code. Lines must be no longer than 100 characters wide.  Avoid excessive consecutive blank lines. In general, you should never have more than one or two consecutive blank lines.

 Please leave a space on both sides of any binary operators you use in your code (i.e., operators that take two operands). For example, use <em>(a + b) – c</em> instead of <em>(a+b)-c</em>. (The only place you do <em><u>not</u></em> have to follow this restriction is within the square brackets used to access an array index, as in: <em>array[i+j]</em>.)  When defining or calling a method, do not leave a space before its opening parenthesis. For example:

use <em>System.out.println(“Hi!”)</em> instead of <em>System.out.println (“Hi!”)</em>.

 Do leave a space before the opening parenthesis in an <em>if</em> statement or a loop. For example, use use <em>for (i = 0; i &lt; n; i++)</em> instead of <em>for(i = 0; i &lt; n; i++)</em>, and use <em>if (condition)</em> instead of <em>if(condition)</em> or <em>if( condition )</em>.

 Use meaningful variable names that convey the purpose of your variables. (The exceptions here are when using variables like <em>i</em>, <em>j</em>, and <em>k</em> for looping variables or <em>m</em> and <em>n</em> for the sizes of some inputs.)  Do not use <em>var</em> to declare variables.

<h1>5.        Compiling and Testing GenericBST on Eustis (and the <em>test-all.sh</em> Script!)</h1>

Recall that your code must compile, run, and produce precisely the correct output on Eustis in order to receive full credit. Here’s how to make that happen:

<ol>

 <li>To compile your program with one of my test cases:</li>

</ol>

javac GenericBST.java TestCase01.java

<ol start="2">

 <li>To run this test case and redirect your output to a text file:</li>

</ol>

java TestCase01 &gt; myoutput01.txt

<ol start="3">

 <li>To compare your program’s output against the sample output file I’ve provided for this test case:</li>

</ol>

diff myoutput01.txt sample_output/TestCase01-output.txt

If the contents of <em>myoutput01.txt</em> and <em>TestCase01-output.txt</em> are exactly the same, <em>diff</em> won’t print anything to the screen. It will just look like this:

<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="314254505f424b71544442455842">[email protected]</a>:~$ diff myoutput01.txt sample_output/TestCase01-output.txt <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="7704121619040d37120204031e04">[email protected]</a>:~$ _

Otherwise, if the files differ, <em>diff</em> will spit out some information about the lines that aren’t the same.

<ol start="4">

 <li>I’ve also included a script, <em>test-all.sh</em>, that will compile and run all test cases for you. You can run it on Eustis by placing it in a directory with <em>java</em> and all the test case files and typing:</li>

</ol>

bash test-all.sh

<strong>Super Important:</strong> Using the <em>test-all.sh</em> script to test your code on Eustis is the safest, most sure-fire way to make sure your code is working properly before submitting.