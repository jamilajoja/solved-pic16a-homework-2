Download Link: https://assignmentchef.com/product/solved-pic16a-homework-2
<br>
<strong>Instructions: </strong>Name your file hw2.py and submit on CCLE. Add comments to each function.

<ul>

 <li><strong>Problem 1</strong>:</li>

</ul>

Write a function longestpath(d) that finds the length of the longest path, (<em>a </em>: <em>b</em>) → (<em>b </em>: <em>c</em>) → ···, in a dictionary d. It counts each pointer from a key to a value as one step. For example, the path (<em>a </em>: <em>b</em>) → (<em>b </em>: <em>c</em>) has length 2. To avoid cycles, we do not allow any key to appear more than once in a path (as a key).

<u>Test cases</u>:

d1 = {“a”:”b”,”b”:”c”} d2 = {“a”:”b”,”b”:”c”,”c”:”d”,”e”:”a”,”f”:”a”,”d”:”b”} longestpath(d1) should return 2. longestpath(d2) should return 5.

<ul>

 <li><strong>Problem 2</strong>:</li>

</ul>

Implement Newton’s method (also known as the Newton-Raphson method) to find a root (zero) of a function. No prior knowledge of this algorithm is needed. Just follow the steps.

Given a function <em>f</em>(<em>x</em>) , the function’s derivative <em>f</em><sup>0</sup>(<em>x</em>), and a desired tolerance <em> </em>(usually a very small positive number), your goal is to find a desired value <em>x</em><sup>∗ </sup>which is close enough to a root of <em>f</em>(<em>x</em>) such that . The algorithm is as follows:

<strong>Algorithm:</strong>

<ol>

 <li>Starting from an initial guess <em>x</em><sub>0</sub>, calculate the error of your guess <em>f</em>(<em>x</em><sub>0</sub>).</li>

</ol>

, then you are done because <em>x</em><sub>0 </sub>is close enough to the root. Otherwise, a better approximation than <em>x</em><sub>0 </sub>is given by<em>.</em>

<ol start="3">

 <li>Keep updating your guess <em>x<sub>n </sub></em>using the formula until you have</li>

</ol>

<strong>Instructions:</strong>

<ul>

 <li>Write your algorithm in a solve function that takes as input a function <em>f</em>(<em>x</em>), its derivative <em>f</em><sup>0</sup>(<em>x</em>), an initial guess <em>x</em><sub>0 </sub>and the tolerance . This function can be called like this:</li>

</ul>

solve(lambda x: [x**2-1, 2*x], 3, 0.0001)

<ul>

 <li>Test your solve function using the following functions <em>f</em>(<em>x</em>), their derivatives <em>f</em><sup>0</sup>(<em>x</em>), and initial guesses <em>x</em><sub>0</sub>:</li>

</ul>

<em>f</em>(<em>x</em>) = <em>x</em><sup>2 </sup>− 1, <em>f</em><sup>0</sup>(<em>x</em>) = 2<em>x</em>, <em>x</em><sub>0 </sub>= 3 <em>f</em>(<em>x</em>) = <em>x</em><sup>2 </sup>− 1, <em>f</em><sup>0</sup>(<em>x</em>) = 2<em>x</em>, <em>x</em><sub>0 </sub>= −1 <em>f</em>(<em>x</em>) = exp(<em>x</em>) − 1, <em>f</em><sup>0</sup>(<em>x</em>) = exp(<em>x</em>), <em>x</em><sub>0 </sub>= 1 <em>f</em>(<em>x</em>) = sin(<em>x</em>), <em>f</em><sup>0</sup>(<em>x</em>) = cos(<em>x</em>), <em>x</em><sub>0 </sub>= 0<em>.</em>5.

Use a calculator to test if the solutions provided by your code are correct, and put results in comment in your script.

Due 5 PM, Wednesday, Jan. 20               <strong>Homework 2                                                    </strong>PIC 16A

<strong>Suggestions:</strong>

<ul>

 <li>You can start by hard-coding the function, its derivative, the initial guess, and the tolerance in your script without getting user input. This will help you better understand the algorithm.</li>

</ul>

If you are still confused, watch this video for an example of Newton’s method with two iterations: <a href="https://www.youtube.com/watch?v=xdLgTDlFwrc">https://www.youtube.com/watch?v=xdLgTDlFwrc</a>