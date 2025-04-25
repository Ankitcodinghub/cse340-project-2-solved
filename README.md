# cse340-project-2-solved



**<span style='color:red'>TO GET THIS SOLUTION VISIT:</span>** https://www.ankitcodinghub.com/product/cse340-project-2-solved-4/

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;102518&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE340  Project 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">
            
<div class="kksr-stars">
    
<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
    
<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">
            

<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>
                

<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<span style="font-size: 2.61792em; letter-spacing: -1px;">Overview</span>

In this project, you are asked to write a C++ program that reads a description of a context free grammar, then, depending on the command line argument passed to the program, performs one of the following tasks (see Section 6.3 for more details on how to run the program with command line arguments):

<ol>
<li>print the list of non-terminals followed by the list of terminals in the order in which they appear in the grammar rules,</li>
<li>find <em>useless </em>symbols in the grammar and remove rules with useless symbols,</li>
<li>calculate FIRST sets,</li>
<li>calculate FOLLOW sets , or</li>
<li>determine if the grammar has a predictive parser.</li>
</ol>
We provide you with code to read the command line argument into an integer variable. Depending on the value of the variable, your program will invoke the appropriate functionality. The rest of the document is organized as follows:

<ol>
<li>Section 3 describes the input format</li>
<li>Section 4 describes what the input represents</li>
<li>Section 5 describes what the output of your program should be for each task. This is the largest section of the document.</li>
<li>Section 6 discusses command line arguments and how you should run and test your program.</li>
<li>Section 7 describes the grading scheme.</li>
<li>Section 8 addresses some submission concerns.</li>
</ol>
<table width="763">
<tbody>
<tr>
<td width="763"><strong>Important Note</strong>. For this project, there is a timeout that we enforce when testing submissions.

•&nbsp;&nbsp;&nbsp;&nbsp; Programs that are functionally correct but that take an inordinate amount of time can be timed out before finishing execution.

•&nbsp;&nbsp;&nbsp;&nbsp; <strong>DO NOT IMPLEMENT YOUR CALCULATIONS RECURSIVELY: </strong>Write a recursive descent parser for the grammar, but do not do the calculations of the sets recursively. If you try to invent a new recursive algorithm for calculating FIRST and FOLLOW, for example, it risks being timed out, and you will not get credit for test cases for which the program is timed out.

•&nbsp;&nbsp;&nbsp;&nbsp; If you follow the algorithms I discussed in class, you should have no problem with timeout.
</td>
</tr>
</tbody>
</table>
<h1>3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Input Format</h1>
The following context-free grammar specifies the input format:

<table width="763">
<tbody>
<tr>
<td width="201">Grammar</td>
<td width="28"><em>→</em></td>
<td width="194">Rule-list HASH</td>
<td width="340"></td>
</tr>
<tr>
<td width="201">Rule-list</td>
<td width="28"><em>→</em></td>
<td width="194">Rule Rule-list&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; |&nbsp;&nbsp;&nbsp; Rule</td>
<td width="340"></td>
</tr>
<tr>
<td width="201">Id-list</td>
<td width="28"><em>→</em></td>
<td width="194">ID Id-list&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | ID</td>
<td width="340"></td>
</tr>
<tr>
<td width="201">Rule</td>
<td width="28"><em>→</em></td>
<td width="194">ID ARROW Right-hand-side</td>
<td width="340">STAR</td>
</tr>
<tr>
<td width="201">Right-hand-side</td>
<td width="28"><em>→</em></td>
<td width="194">Id-list&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; |</td>
<td width="340"></td>
</tr>
</tbody>
</table>
The input consists of a rule list. Each rule has a lefthand side which is an ID, which is followed by an arrow and is followed by a sequence of zero more IDs and terminated with a STAR. The meaning of the input is explained in the <em>Semantics </em>section below. The tokens used in the above grammar description are defined by the following regular expressions:

<table width="763">
<tbody>
<tr>
<td width="172">ID</td>
<td width="591">= letter (letter + digit)*</td>
</tr>
<tr>
<td width="172">STAR</td>
<td width="591">= ‘*’</td>
</tr>
<tr>
<td width="172">HASH</td>
<td width="591">= #</td>
</tr>
<tr>
<td width="172">ARROW</td>
<td width="591">= -&gt;</td>
</tr>
</tbody>
</table>
Where digit is the digits from 0 through 9 and letter is the upper and lower case letters a through z and A through Z.

Tokens are case-sensitive. Tokens are space separated and there is at least one whitespace character between any two successive tokens. We provide a lexer with a geToken() function to recognize these tokens. You should use the provided lexer in you solution.

<h1>4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Semantics</h1>
Each grammar Rule starts with a non-terminal symbol (the left-hand side of the rule) followed by ARROW, then followed by a sequence of zero or more terminals and non-terminals, which represent the right-hand side of the rule. If the sequence of terminals and non-terminals in the right-hand side is empty, then the right hand side represents .

The set of non-terminals for the grammar is the set of symbols that appear to the left of an arrow. Grammar symbols that do not appear to the left of an arrow are terminal symbols. The start symbol of the grammar is the left hand side of the first rule of the grammar.

Note that the convention of using upper-case letters for non-terminals and lower-case letters for terminals that I typically followed in class does not apply in this project.

<h2>4.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Example</h2>
Here is an example input:

decl -&gt; idList colon ID * idList -&gt; ID idList1 *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * #

The list of non-terminal symbols in the order in which they appear in the grammar is:

Non-Terminals = <em>{ </em>decl<em>, </em>idList<em>, </em>idList1 <em>}</em>

The list of terminal symbols in the order in which they appear in the grammar is:

Terminals = <em>{ </em>colon<em>, </em>ID<em>, </em>COMMA <em>}</em>

The grammar that this input represents is the following:

<table width="763">
<tbody>
<tr>
<td width="763">decl <em>→ </em>idList colon ID

idList <em>→ </em>ID idList1

idList1 <em>→ </em>

idList1 <em>→ </em>COMMA ID idList1
</td>
</tr>
</tbody>
</table>
Note that even though the example shows that each rule is on a line by itself, a rule can be split into multiple lines, or even multiple rules can be on the same line. The following input describes the same grammar as the above example:

decl -&gt; idList colon ID * idList -&gt; ID idList1 * idList1 -&gt; * idList1

-&gt; COMMA ID idList1 *&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; #

<h1>5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Output Specifications: Tasks 1 – 5</h1>
<strong>Parsing: </strong>There is no serapate tsak for prasing the ipnut. Your praesr sohuld porerply prase the ipnut and should ouptut SYNTAX ERROR !!! if the input has a snyatx error and it should not ouptut SYNTAX ERROR !!! if the input does not have a syntax error. There will be a deduction of 15% if your praser does not corecrctly parse the input.

Your program should read the input grammar from standard input, and read the requested task number from the first command line argument (as stated earlier, we provide code to read the task number). Then, your program should calculate the requested output based on the task number and print the results in the specified format for each task to standard output (stdout). The following specifies the exact requirements for each task number.

<h2>5.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Task 1: Printing Terminals and Non-terminals</h2>
Task one simply outputs the list of terminals <em>in the order in which they appear in the grammar rules </em>followed by the list of non-terminals <em>in the order in which they appear in the grammar rules</em>.

<strong>Example:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>For the input grammar

decl -&gt; idList colon ID * idList -&gt; ID idList1 *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * #

the expected output for task 1 is:

colon ID COMMA decl idList idList1

<strong>Example:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>Given the input grammar:

decl -&gt; idList colon ID *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * idList -&gt; ID idList1 * #

the expected output for task 1 is:

colon ID COMMA decl idList idList1

Note that in this example, even though the rule for idList1 is before the rule for idList, idList appears before idList1 in the grammar rules. To be clear, here is the grammar again with the order of each symbol added between parentheses after the first appearance of the symbol.

decl (1)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -&gt; idList (2) colon (3) ID (4) * idList1 (5) -&gt; *

idList1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -&gt; COMMA (6) ID idList1 * idList&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; -&gt; ID idList1 *

#

<h2>5.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Task 2: Eliminating Useless Symbols</h2>
<h3>5.2.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Useless Symbols: Definition</h3>
The following is the definition for useless and useful symbols.

<strong>Definition: </strong>Symbol <em>A </em>is <em>useful </em>if there is a derivation starting from <em>S </em>of a string of terminals, possibly empty, in which <em>A </em>appears:

<em>∗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ∗&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <sup>∗</sup></em>

<em>S ⇒ … ⇒ xAy ⇒ … ⇒ w ∈ T</em>

A symbol is <em>useless </em>if it is not useful.

The algorithm for determining useless symbols is given in a separate presentation provided with the project documents.

<h3>5.2.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Task Requirements</h3>
Determine <em>useless </em>symbols in the grammar and remove rules that contain useless symbols. Then output each of the remaining rules on a single line in the following format:

&lt;LHS&gt; -&gt; &lt;RHS&gt; Where &lt;LHS&gt; should be replaced by the left-hand side of the grammar rule and &lt;RHS&gt; should be replaced by the right-hand side of the grammar rule. If the grammar rule is of the form <em>A → </em>, use # to represent the epsilon. Note that this is different from the input format.

The grammar rules should be printed in the same relative order that they were originally in. So, if Rule1 and Rule2 are not removed after the elimination of useless symbols, and Rule1 appears before Rule2 in the original grammar, then Rule1 should be printed before Rule2 in the output.

<strong>Example 1:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>Given the following input grammar :

decl -&gt; idList colon ID * idList -&gt; ID idList1 *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * #

the expected output for task 2 is:

decl -&gt; idList colon ID idList -&gt; ID idList1 idList1 -&gt; # idList1 -&gt; COMMA ID idList1

Note that none of the symbols of this grammar are useless.

<strong>Example 2:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>Given the following input grammar:

S -&gt; A B * S -&gt; C * C -&gt; c * S -&gt; a *

<ul>
<li>-&gt; a A *</li>
<li>-&gt; b *</li>
</ul>
#

the expected output for task 2 is:

S -&gt; C C -&gt; c S -&gt; a

Note that A and B are useless symbols and the modified grammar has only three rules. Also note that the relative order of the rules is preserved.

<h2>5.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Task 3: Calculate FIRST Sets</h2>
Compute the FIRST sets for all the non-terminal symbols. Then, for each of the non-terminals of the input grammar, in the order in which it appears in the grammar, output one line in the following format: FIRST(&lt;symbol&gt;) = { &lt;set_items&gt; }

where &lt;symbol&gt; should be replaced by the non-terminal name and &lt;set_items&gt; should be replaced by a comma-separated list of elements of the set ordered in the following manner.

<ul>
<li>If belongs to the set, represent it as #.</li>
<li>If belongs to the set, it should be listed before any other element of the set.</li>
<li>All other elements of the set should be sorted in the order in which they appear in the grammar.</li>
</ul>
<strong>Example:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>Given the input grammar:

decl -&gt; idList colon ID * idList -&gt; ID idList1 *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * #

the expected output for task 3 is:

FIRST(decl) = { ID }

FIRST(idList) = { ID }

FIRST(idList1) = { #, COMMA }

<h2>5.4&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Task 4: Calculate FOLLOW Sets</h2>
Compute the FOLLOW sets for all the non-terminal symbols. Then, for each of the non-terminals of the input grammar, in the order in which it appears in the grammar, output one line in the following format: FOLLOW(&lt;symbol&gt;) = { &lt;set_items&gt; }

where &lt;symbol&gt; should be replaced by the non-terminal and &lt;set_items&gt; should be replaced by the comma-separated list of elements of the set ordered in the following manner.

<ul>
<li>If EOF belongs to the set, represent it as $.</li>
<li>If EOF belongs to the set, it should be listed before any other element of the set.</li>
<li>All other elements of the set should be sorted in the order in which they appear in the grammar.</li>
</ul>
<strong>Example:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>Given the input grammar:

decl -&gt; idList colon ID * idList -&gt; ID idList1 *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * #

the expected output for task 4 is:

FOLLOW(decl) = { $ }

FOLLOW(idList) = { colon }

FOLLOW(idList1) = { colon }

<h2>5.5&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Task 5: Determine if the grammar has a predictive parser</h2>
If the grammar has useless symbols, your program should output NO. Otherwise, determine if the grammar has a predictive parser and output either YES or NO accordingly.

<strong>Example:&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>Given the grammar:

decl -&gt; idList colon ID * idList -&gt; ID idList1 *

idList1 -&gt; *

idList1 -&gt; COMMA ID idList1 * #

the expected output of Task 5 is:

YES

<strong>Note </strong>You will not get credit for this task if you output NO for all input or YES for all input. You should get at least 70% of the test cases correct to get credit on this task.

<h1>6&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Implementation</h1>
<h2>6.1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Lexer</h2>
A lexer that can recognize ID, ARROW, STAR and HASH tokens is provided for this project. You are required to use it and you should not modify it.

<h2>6.2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Reading command-line argument</h2>
As mentioned in the introduction, your program must read the grammar from stdin and the task number from command line arguments. The following piece of code shows how to read the first command line argument and perform a task based on the value of that argument. Use this code as a starting point for your main function.

/* NOTE: You should get the full version of this code as part of the project material, do not copy/paste from this document. */

#include &lt;stdio.h&gt; #include &lt;stdlib.h&gt;

int main (int argc, char* argv[])

{ int task;

if (argc &lt; 2) {

printf(“Error: missing argument\n”); return 1;

} task = atoi(argv[1]);

switch (task) { case 1:

// TODO: perform task 1. break;

// …

default: printf(“Error: unrecognized task number %d\n”, task); break;

} return 0;

}

<h2>6.3&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Testing</h2>
You are provided with a script to run your program on all tasks for each of the test cases. The test cases that we provided for this project are not extensive. <strong>They are meant to serve as example cases and are not meant to test all functionality</strong>. The test cases on the submission site will be extensive. <strong>You are expected to develop your own additional test cases based on the project specification</strong>.

To run your program for this project, you need to specify the task number through command line arguments. For example, to run task 3:

$ ./a.out 3

Your program should read the input grammar from standard input. To read the input grammar from a text file, you can redirect standard input:

$ ./a.out 3 &lt; test.txt

For this project we use 5 expected files per each test case input. For an input file named test.txt , the expected files are test.txt.expected1, test.txt.expected2, test.txt.expected3, test.txt.expected4 and test.txt.expected5 corresponding to tasks 1 through 5. The test script test_p2.sh , provided with the project material, takes one command line argument indicating the task number to use. So for example to test your program against all test cases for task 2, use the following command:

$ ./test_p2.sh 2

To test your program against all test cases for all tasks, you need to run the test script 5 times:

$ ./test_p2.sh 1 $ ./test_p2.sh 2 $ ./test_p2.sh 3 $ ./test_p2.sh 4

$ ./test_p2.sh 5

&nbsp;
