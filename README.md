Download Link: https://assignmentchef.com/product/solved-cs213-assignment3-polynomial-addition
<br>
P1 : Polynomial Addition

Build a class to represent “sparse” polynomials (think about it!) and use it to add two polynomials. You are expected to build the necessary member functions too.

<u>Input :</u>

No. of terms in polynomial 1 having non-zero coefficients : n​1

Space separated coefficients of polynomial 1

Space separated powers having the corresponding coefficients of polynomial 1

No. of terms in polynomial 2 : n​2

Space separated coefficients of polynomial 2

Space separated powers having the corresponding coefficients of polynomial 2




<u>Output:</u>

Space separated coefficients of the multiplied polynomial

Space separated powers having the corresponding coefficients of the multiplied polynomial




<u>Constraints:</u>

nnIntegral Coefficients &lt; 10​1​2 &lt; 10​ &lt;10​                    3​ 3​            6​




<u>Examples:</u>

Worked out example :

Input:

A[] = {5, 0, 10, 6}         B[] = {1, 0, 0, 0,  4}  Output:

add[] = {6,0,10,6,4}




The first input array represents =&gt; 5 + 10x<sup>4</sup>  <sup>2</sup>​ ​ + 6x<sup>3</sup>​

The second array represents  =&gt; 1 + 4x​

And Output is  =&gt; 6 + 10×2​ <sub>​</sub><sub> + 6x</sub>3​ <sub>​</sub><sub> + 4x</sub>4​<sub>  </sub>




<table width="624">

 <tbody>

  <tr>

   <td width="312">Input</td>

   <td width="312">Output</td>

  </tr>

  <tr>

   <td width="312">35 10 60  2 321  40 4</td>

   <td width="312">6 10 6 40 2 3 4</td>

  </tr>

 </tbody>

</table>

<em><u>File to be submitted : p1.cpp</u> </em>

<h1>P2: Merge Sort and Quick sort</h1>

Having learned the problem of sorting in the context of the divide and conquer paradigm, you have to implement the Merge Sort and Quick sort algorithm to sort arrays in files p2-ms.cpp and p2-qs.cpp respectively.




<u>Input Format:</u>

The first line contains a single integer ​<strong>n</strong>, the length of the array.​          The next line contains ​<strong>n </strong>​integers.




<u>Output:</u>

Sorted array space separated




<u>Examples:</u>

<table width="624">

 <tbody>

  <tr>

   <td width="312"><strong>Input </strong></td>

   <td width="312"><strong>Output </strong></td>

  </tr>

  <tr>

   <td width="312">63 4 2 1 5 6</td>

   <td width="312">1 2 3 4 5 6</td>

  </tr>

  <tr>

   <td width="312">63 3 4 1 5 7</td>

   <td width="312">1 3 3 4 5 7</td>

  </tr>

 </tbody>

</table>

<em>File to be submitted : p2-ms.cpp and p2-qs.cpp </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<em> </em>

<h1>P3: Longest Prefix Common in a list of strings</h1>

<strong> </strong>

Given a list/array of strings, find the longest common prefix among the list of strings. You need to assume case sensitivity, i.e. ‘L’ != ‘l’.




<u>Expected complexity:</u>​ O( n*log(n) ), where n is the size of the list/array.




<u>Input:</u>

The first line contains a single integer ​<strong>n</strong>, the length of the list.​

Next <strong>n</strong>​ lines : ‘​ <strong>s</strong>​ ’, s.t. |​ <strong>s</strong>​ ​| &lt; 100




<u>Output </u>​:

Longest common prefix, or ​<strong>-1</strong>​ in case there are no common prefixes




<u>Constraints</u>​ : n &lt; 10​<sup>5 </sup>|s| &lt; 100

<u>Examples</u>​ :




<table width="624">

 <tbody>

  <tr>

   <td width="312"><strong>Input  </strong></td>

   <td width="312"><strong>Output </strong></td>

  </tr>

  <tr>

   <td width="312">3 hello hell  holy</td>

   <td width="312">h</td>

  </tr>

  <tr>

   <td width="312">2  great  big</td>

   <td width="312">-1</td>

  </tr>

  <tr>

   <td width="312">4ManMangoMankindMandatory</td>

   <td width="312">Man</td>

  </tr>

  <tr>

   <td width="312">2 Bat bat</td>

   <td width="312">-1</td>

  </tr>

 </tbody>

</table>

<em> </em>

<em>File to be submitted : p3.cpp</em>

<h1>P4: Playing with array search</h1>

Consider that you are communicating with a backend server using an http connection. The backend server has an array of Strings, <strong>‘arr’</strong>​   ​ of length N. Each element of the array is a lowercase string ​<strong>s</strong>​ such that |​<strong>s</strong>​| &lt;= 20, i.e. length of the string is &lt;= 20. This array is sorted according to the lexicographical order i.e. dictionary order. <em>(</em>​ <em>Read about it if you are not aware: </em><a href="https://en.wikipedia.org/wiki/Lexicographical_order"><em>Lexicographical Order Wiki</em></a><a href="https://en.wikipedia.org/wiki/Lexicographical_order">​</a><em>)</em>​. You are allowed to communicate with the backend in a very simple way : You send an index i s.t. (i &lt; N), and the backend returns the string at index i, i.e. arr[i]. This communication or ‘access’ takes a certain time due to the network delays.




You have to search a given string in the array, i.e. output the index of the string in the array else <strong>-1</strong>​ if it is not present. Assume 0-based indexing.




There are two types of accesses —

<ol>

 <li><strong>Good Access</strong>​ : An access of index i, i.e. arr[i] is a good access if arr[i] &lt; given string.</li>

 <li><strong>Bad Access</strong> : An access of index i, i.e. arr[i] is a bad access if arr[i] &gt;= given string.​ Here s​1 &lt; s​                        ​2 if s​           ​1 occurs lexicographically before s​          ​2 (If s​        ​1 is a prefix of s​                        ​2 , then s​                     ​1 &lt; s​          ​2)​</li>

</ol>




It turns out that the backend code written has some bugs in it due to which it can handle only at most ​<strong>k</strong>​ bad accesses. At the ​<strong>(k+1)</strong>​<strong><sup>th</sup></strong>​ bad access the backend code will crash and you should have known your answer by then. i.e.  at max you can do ​<strong>(k+1)</strong>​ bad accesses. You are to minimize the number of good accesses (thereby time) done by your search algorithm while keeping the bad accesses at max ​<strong>k+1</strong>​. Keep in mind that this minimization is to take into account the different possibilities of the given strings positions in the array. i.e. it should not be the case that your algorithm works for certain cases really well and for certain cases it performs very poorly.




<ul>

 <li>For k = 0 : the answer is a simple linear search starting from the start of the array. If you encounter the given string ​<strong>a</strong>​, output the index else keep on moving till you encounter the first element ​<strong>s</strong>​t. ​<strong>s</strong> &gt; ​ ​<strong>a</strong>​, in which case it is a bad query and hence the backend will crash. At this point you know the answer that the given string is not present in the array. And hence you can output ​<strong>-1</strong>​. This is the best guarantee we can give, hence the number of accesses would be O(n).</li>

</ul>




<ul>

 <li>For k &gt;= log(​<strong>N</strong>​) + 1 : The answer is a O( log(​<strong>N</strong>​) ). This can be done using a binary search algorithm.</li>

</ul>




<strong>The task of this assignment is to do the search for k = 1, i.e. only one bad access allowed by the backend server.  </strong>




<u>Coding it up :</u>

For the purpose of the assignment you have to model the backend server as an array and maintain a counter of the number of accesses that you are doing of an array. Thus, counter * Delay would model the actual delay of your algorithm. Essentially every single time you access an element, i.e. write arr[i] in your code you need to increment the counter by 1. Also you need to ensure that the number of bad queries in your algorithm is &lt;= ​<strong>k + 1</strong>​.




<u>Input Format:</u>

N : number of elements in the array

Next N lines : elements of the array, strings of size &lt;= 20. Last line : given string to search, str




<u>Output Format</u>​:

1st line contains the answer : index i of given search string, -1 is not present.        Next line contains the number of good accesses made by your algorithm.




(Extra : It would be a good idea to test your code by running it on different instances searching for different strings for a given array and also for strings that are not present. You can even see the algorithm complexity by plotting the accesses made against the inputs of different sizes. ​<strong>Do not submit these graphs</strong>​)




<u>Grading :</u>

You will be given 3 marks for writing a code with correct implementation, i.e. the first line of output matching the correct solution. Also your number of accesses would be compared with the best solution and based on how close your solution is you will be given partial marks for the remaining 7 marks. So it is highly recommended to explore and try out different solutions.




<u>Examples</u>:​

For a naive linear Search implementation :

<table width="624">

 <tbody>

  <tr>

   <td width="312">Input</td>

   <td width="312">Output</td>

  </tr>

  <tr>

   <td width="312">5 apple banana grapes mango orange guava</td>

   <td width="312">-15</td>

  </tr>

  <tr>

   <td width="312">5 apple banana grapes mango orange</td>

   <td width="312">34</td>

  </tr>

  <tr>

   <td width="312">mango</td>

   <td width="312"> </td>

  </tr>

 </tbody>

</table>

<em>Files to be submitted : p4.cpp </em>




<u>Bonus Question </u>​: Do the same for k = 2. Submit another file p4-bonus.cpp. (Hint O(n<sup>1</sup>​ <sup>/3</sup>​) solution can be achieved) (5 marks)

<strong>P5: (Bonus Question) Electric Force Calculation :  </strong>

Consider ​<strong>n</strong>​ point charges located at points on the x axis (1D) at coordinates 0, 1, 2, … , n – 1. The charge at point ​<strong>i</strong>​ has value ​<em>q</em>​<em>i</em><sub>​</sub> , which may be positive or negative. The net force on charge <sub>​     </sub>​<strong>i</strong> due to all other charges is defined as :

∑<sub> <em>i</em> &lt; <em>j</em> </sub> (<em>q<sub>i </sub></em>* <em>q<sub>j</sub></em>) / [(<em>i </em>− <em>j</em>)<sup>2</sup>]<strong> –</strong>∑<sub> <em>j</em> &lt; <em>i</em></sub> (<em>q<sub>i </sub></em>* <em>q<sub>j</sub></em>) / [(<em>j </em>− <em>i</em>)<sup>2</sup>] <strong> </strong>

<strong> </strong>

Write an O(n*log(n)) algorithm to calculate the force on each charged particle calculated using the above formula.




<u>Input :</u>

<strong>n </strong>:​ number of particles <strong><em>q</em></strong>​<strong><em>i</em></strong><sub>​</sub> where 0 &lt;= <em>i </em>&lt; <em>n</em>  <u>Output :</u> <strong>n</strong>​ space separated integers, i.e. force on particle at position ​<strong>i</strong>​ rounded to the nearest

integer




<u>Constraints </u>0 &lt; ​:<em>n</em>  &lt; 10<sub>5</sub>

|<em>q<sub>i</sub></em>| &lt; 10<sup>6</sup>




<u>Hint:</u>​ Is the problem a bit ​<strong><em>convoluted </em></strong>​? Maybe that’s why it is a bonus




<u>Examples :</u>




<table width="624">

 <tbody>

  <tr>

   <td width="312">Input</td>

   <td width="312">Output</td>

  </tr>

  <tr>

   <td width="312">21 -1</td>

   <td width="312">1 -1</td>

  </tr>

  <tr>

   <td width="312">1 100</td>

   <td width="312">0 </td>

  </tr>

 </tbody>

</table>

<em>File to be submitted : p5.cpp </em>

<em> </em>

<em> </em>