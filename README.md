Download Link: https://assignmentchef.com/product/solved-ads-assignment-1-stable-marriage
<br>



”Life’s a game made for everyone. And love is the prize.” (Wake me up – Avicii)

Everywhere we look, love is featured. In movies, series, commercials, when you go for a walk and some couple are kissing (annoyingly) passionatly on your favourite park bench. Furthermore various articles and books are written on the subject, suggesting that it is of great interest to many people.

Finding love is a tough challenge for everyone. Sometimes you like someone who does not love you. Sometimes someone likes you who you don’t like. Sometimes you like each other, but then a third person appears and causes a love triangle.

<h1>Aims</h1>

The goal of the lab is:

<ul>

 <li>Implementing an algorithm.</li>

 <li>Debugging your code.</li>

 <li>Structuring your code in a logical fashion.</li>

 <li>Parsing messy input.</li>

 <li>Reason about correctness of your algorithm.</li>

 <li>Reason about upper bounds for time complexity.</li>

</ul>

<h1>Problem formulation</h1>

Please note that the algorithm was invented (by David Gale and Lloyd Shapley) and the problem was formulated in 1962<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> with binary, heterosexual, monogamous relationships. To ease the understanding of the problem we keep the formulation, but the student is encuraged to change ”men” and ”women” to some binary classes of e.g. hospitals and medical students or servers and clients.

You are given each man’s and woman’s preference lists. Given these lists find a stable matching, meaning that there do not exist two man-woman-pairs (<em>m</em><sub>1</sub><em>,w</em><sub>1</sub>)<em>,</em>(<em>m</em><sub>2</sub><em>,w</em><sub>2</sub>) such that <em>w</em><sub>2 </sub>is higher ranked on <em>m</em><sub>1</sub>’s preference list than <em>w</em><sub>1 </sub>and simultaneously <em>m</em><sub>1 </sub>is higher ranked on <em>w</em><sub>2</sub>’s preference list than <em>m</em><sub>2 </sub>(thus that both <em>m</em><sub>1 </sub>and <em>w</em><sub>2 </sub>would prefer to change partner).

<h1>Input</h1>

Input is given through standard in (not from a file). To run the program write for instance

<ul>

 <li>java solution_file &lt; input_file</li>

 <li>python3 solution_file &lt; input_file</li>

 <li>./a.out &lt; input_file</li>

</ul>

The first line of the input contains a single integer <em>N </em>(1 ≤ <em>N </em>≤ 3000), the number of men and women.

Then follows the preference lists. In total (<em>N </em>+1) · 2<em>N </em>integers are given on one or more lines. These numbers are structured in 2<em>N </em>chunks of <em>N </em>+1 integers each. Each chunk contain the description of one persons preference list – first an integer 1 ≤ <em>i </em>≤ <em>N</em>, the index of the person, then <em>N </em>distict integers, the preference list of person <em>i</em>. These <em>N </em>integers are all different and between 1 and <em>N</em>, inclusive.

Note that each person index <em>i </em>∈ {1<em>,</em>2<em>,…,N</em>} appears twice – the first appearence is for woman <em>i</em>, the second for man <em>i</em>.

<h1>Output</h1>

The output should be printed to standard out (not to a file). To do this use for instance

<ul>

 <li>out.println() in Java</li>

 <li>print() in Python</li>

 <li>cout in C++.</li>

</ul>

The output should consist of exactly <em>N </em>rows. Row <em>i </em>should contain exactly one integer, the index of the man paired with woman <em>i</em>.

<h1>Examination and Points of Discussion</h1>

To pass the lab make sure you:

<ul>

 <li>Have successfully implemented the algorithm with time complexity O(<em>n</em><sup>2</sup>).</li>

 <li>Have neat and understandable code.</li>

 <li>Have descriptive variable names.</li>

 <li>Have filled in the blanks in the report.</li>

 <li>Have run the check_solution script, to validate your solution.</li>

</ul>

During the oral presentation you will discuss the following questions with the lab assistant: • Why does your algorithm obtain a stable solution?

<ul>

 <li>Could there be other stable solutions? Do you have an example/proof of uniqueness?</li>

 <li>What is the time complexity and why?</li>

 <li>Is this (the algorithm) how matching is performed in real life? If not, what flaws does it have?</li>

 <li>Are there any applications of the algorithm (as it is or in a slightly shifted version)?</li>

</ul>

<strong>Sample Input 1                                                                                 Sample Output 1</strong>

<table width="622">

 <tbody>

  <tr>

   <td width="311">21     1 22     2 11     1 22     2 1</td>

   <td width="311">12</td>

  </tr>

 </tbody>

</table>

<strong>Sample Input 2                                                                                 Sample Output 2</strong>

<table width="622">

 <tbody>

  <tr>

   <td width="311">21 1 21     2 12     2 12 1 2</td>

   <td width="311">21</td>

  </tr>

 </tbody>

</table>




<a href="#_ftnref1" name="_ftn1">[1]</a> https://en.wikipedia.org/wiki/Stable_marriage_problem#Algorithm