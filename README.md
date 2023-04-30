Download Link: https://assignmentchef.com/product/solved-foundations-of-algorithms-programming-assignment-3
<br>
The following is a problem to be completed by the individual (i.e., it is not collaborative) and then implemented. You may use any programming language you wish. Please follow the requirements provided under Syllabus &amp; Course Information under the link Programming Assignment Requirements.

<ol>

 <li>Programming (non-collaborative)—Due at the end of Module 13. You are consulting for a group of people (who would prefer not to be mentioned here by name) whose job consists of monitoring and analyzing electronic signals coming from ships in the Atlantic ocean. They want a fast algorithm for a basic primitive that arises frequently: “untangling” a superposition of two known signals. Specifically, they are picturing a situation in which each of two ships is emitting a short sequence of 0s and 1s over and over, and they want to make sure that the signal they are hearing is simply an interleaving of these two emissions, with nothing extra added in.</li>

</ol>

This describes the whole problem; we can make it a little more explicit as follows. Given a string <em>x </em>consisting of 0s and 1s, we write <em>x<sup>k </sup></em>to denote <em>k </em>copies of <em>x </em>concatenated together. We say that string <em>x</em><sup>′ </sup>is a repetition of <em>x </em>if it is a prefix of <em>x<sup>k </sup></em>for some number <em>k</em>. So <em>x</em><sup>′ </sup>=10110110110 is a repetition of <em>x</em>=101.

We say that a string <em>s </em>is an interleaving of <em>x </em>and <em>y </em>if its symbols can be partitioned into two (not necessarily contiguous) subsequence <em>s</em><sup>′ </sup>and <em>s</em><sup>′′ </sup>so that <em>s</em><sup>′ </sup>is a repetition of <em>x </em>and <em>s</em><sup>′′ </sup>is a repetition of <em>y</em>. (So each symbol in <em>s </em>must belong to exactly one of <em>s</em><sup>′ </sup>and <em>s</em><sup>′′</sup>.) For example, if <em>x</em>=101 and <em>y</em>=00, then <em>s</em>=100010101 is an interleaving of <em>x </em>and <em>y </em>since characters 1, 2, 5, 7, 8, and 9 form 101101—a repetition of <em>x</em>—and the remaining characters 3, 4, 6 form 000—a repetition of <em>y</em>. In terms of our application, <em>x </em>and <em>y </em>are the repeating sequences from the two ships, and <em>s </em>is the signal we are listening to. We want to make sure <em>s </em>“unravels” into simple repetitions of <em>x </em>and <em>y</em>.

<ul>

 <li>[50 points] Give an efficient algorithm that takes strings <em>s</em>, <em>x</em>, and <em>y </em>and decides if <em>s </em>is an interleaving of <em>x </em>and <em>y</em>. Derive the computational complexity of your algorithm.</li>

 <li>[50 points] Implement your algorithm above and test its run time to verify your analysis. Remember that CPU time is not a valid measure for testing run time. You must use something such as the number of comparisons.</li>

</ul>