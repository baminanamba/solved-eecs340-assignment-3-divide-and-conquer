Download Link: https://assignmentchef.com/product/solved-eecs340-assignment-3-divide-and-conquer
<br>
Problem 1

Let 0 <em>&lt; λ &lt; </em>1 <em>&lt; a &lt; b </em>be constants. Solve the following recurrences using Master Method, noting the case that applies.

<ul>

 <li><em>T</em>(<em>n</em>) = <em>bT</em>(<em>n/a</em>) + Θ(<em>n</em>).</li>

 <li><em>T</em>(<em>n</em>) = <em>a</em><sup>2</sup><em>T</em>(<em>n/a</em>) + Θ(<em>n</em><sup>2</sup>).</li>

 <li><em>T</em>(<em>n</em>) = <em>T</em>(<em>λn</em>) + <em>n<sup>λ</sup></em>.</li>

 <li><em>T</em>(<em>n</em>) = <em>aT</em>(<em>n/a</em>) + Θ(<em>n<sup>λ</sup></em>(log<em>n</em>)<em><sup>b</sup></em>).</li>

</ul>

<h1>Problem 2</h1>

Prove the solutions to the following recurrences using Substitution Method:

<ul>

 <li>For any constant 0 <em>&lt; α &lt; </em>1, if <em>T</em>(<em>n</em>) = <em>T</em>(<em>αn</em>) + <em>T</em>((1 − <em>α</em>)<em>n</em>) + Θ(<em>n</em>), then <em>T</em>(<em>n</em>) = <em>O</em>(<em>n</em>log<em>n</em>).</li>

 <li>For any constant ), then <em>T</em>(<em>n</em>) = <em>O</em>(<em>n</em>).</li>

</ul>

<h1>Problem 3</h1>

Dr. Purplesheep discovered a new class of materials, which are useful in converting solar energy to electrical energy. She has designed 25 unique materials that belong to this class, and she would like to identify the top 3 out of these 25 materials in terms of their effectiveness. Unfortunately, however, she does not have an experimental method that can be used to quantify the effectiveness of a given material. Instead, she can run comparative experiments such that each experiment provides a ranking of 5 materials in terms of their effectiveness (from most effective to least effective). Running these experiments is rather expensive, so she would like to minimize the number of experiments she runs. Can you help her design a strategy that will identify the 3 most effective materials among 25 materials by performing the minimum number of experiments? What is the minimum number of experiments needed to conclusively determine the 3 most effective materials? You do not need to write pseudo-code; a verbal explanation, possibly supported by graphics, will suffice.

<strong>Example. </strong>Suppose Dr. Purplesheep performs an experiment on materials <em>M</em><sub>3</sub>, <em>M</em><sub>7</sub>, <em>M</em><sub>9</sub>, <em>M</em><sub>14</sub>, <em>M</em><sub>25</sub>. Then, the result of the experiment will be a ranking such as: <em>M</em><sub>14 </sub><em>&gt; M</em><sub>3 </sub><em>&gt; M</em><sub>25 </sub><em>&gt; M</em><sub>7 </sub><em>&gt; M</em><sub>9</sub>.

<h1>Problem 4</h1>

We are given a dictionary <em>D</em>, which is an array of <em>n </em>distinct strings, sorted in lexicographic order. We are also given a procedure Compare-Strings(<em>x</em>, <em>y</em>), which will compare two strings <em>x </em>and <em>y </em>in Θ(1) time, and return true if <em>x </em>comes before <em>y</em>, and false if <em>y </em>comes before <em>x </em>in lexicographic order. We are also given an array <em>C</em>, which contains <em>n</em>−1 of the <em>n </em>strings in <em>D</em>, but <em><u>C </u></em><u>is not sorted</u>. We would like to develop an algorithm that will find the string that is missing in <em>C</em>.

(a) Design a divide-and-conquer algorithm that will find the missing string in Θ(<em>n</em>) time. You can assume that we can utilize the Partition algorithm that is used by QuickSort, by modifying it to compare strings instead of comparing numbers (you do not need to show how to do the modification). Write the pseudo-code of your algorithm and explain how it works. (Hint: You can select the pivot used for Partition algorithm in an informed manner that guarantees the resultant subarrays to be of nearly equal size.) (b) Show that the runtime of your algorithm is Θ(<em>n</em>).

<strong>Example. </strong>Suppose <em>D </em>= {”<em>W</em>”<em>,</em>”<em>X</em>”<em>,</em>”<em>Y </em>”<em>,</em>”<em>Z</em>”} and <em>C </em>= {”<em>Y </em>”<em>,</em>”<em>Z</em>”<em>,</em>”<em>W</em>”}. <em>D </em>contains <em>n </em>= 4 strings and <em>C </em>contains all <em>n </em>− 1 = 3 strings in <em>D </em>except ”X”. Thus, missing string in <em>C </em>is: ”X”.