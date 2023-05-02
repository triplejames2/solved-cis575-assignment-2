Download Link: https://assignmentchef.com/product/solved-cis575-assignment-2
<br>
<ol>

 <li>Assuming that <em>A</em>[1<em>..n</em>] is non-decreasing and that <em>x </em>occurs in <em>A</em>[1<em>..n</em>], consider the below program (which may be what you constructed in Assignment 1):</li>

</ol>

<em>lo,hi,q </em>← 1<em>,n,</em>(1 + <em>n</em>) div 2 <strong>while </strong><em>A</em>[<em>q</em>] 6= <em>x </em><strong>if </strong><em>A</em>[<em>q</em>] <em>&lt; x</em>

<em>lo </em>← <em>q </em>+ 1

<strong>else</strong>

<em>hi </em>← <em>q </em>− 1

<em>q </em>← (<em>lo </em>+ <em>hi</em>) div 2

<strong>return </strong><em>q</em>

If <em>n </em>= 1, the body of the while loop will not be executed; if <em>n </em>= 2, it will be executed once (if <em>A</em>[1] <em>&lt; x</em>) or not at all (if <em>A</em>[1] = <em>x</em>); if <em>n </em>= 3, it will be executed once (if <em>A</em>[2] 6= <em>x</em>) or not at all.

Let <em>U</em>(<em>m</em>) denote the maximum number of iterations of the while loop body when <em>A</em>[<em>lo..hi</em>] has <em>m </em>elements (that is, <em>m </em>= <em>hi </em>− <em>lo </em>+ 1). We can thus tabulate the first entries of <em>U </em>as follows:

<table width="225">

 <tbody>

  <tr>

   <td width="46"><em>m</em></td>

   <td width="20">1</td>

   <td width="20">2</td>

   <td width="20">3</td>

   <td width="20">4</td>

   <td width="20">5</td>

   <td width="20">6</td>

   <td width="20">7</td>

   <td width="20">8</td>

   <td width="20">9</td>

  </tr>

  <tr>

   <td width="46"><em>U</em>(<em>m</em>)</td>

   <td width="20">0</td>

   <td width="20">1</td>

   <td width="20">1</td>

   <td width="20"> </td>

   <td width="20"> </td>

   <td width="20"> </td>

   <td width="20"> </td>

   <td width="20"> </td>

   <td width="20"> </td>

  </tr>

 </tbody>

</table>

<ol>

 <li>: Find <em>U</em>(4). You must argue for your answers.</li>

 <li>Provide the remaining missing entries in the above table, that is, compute <em>U</em>(<em>m</em>) for <em>m </em>= 5<em>..</em> You do not need to argue for your answers.</li>

 <li>Use your table to write a <em>recurrence </em>(a recursive equation) that (for <em>m </em>≥ 2) expresses <em>U</em>(<em>m</em>) in terms of). You do not need to argue for your answer, but show that for <em>m </em>= 3<em>,</em>8 it coincides with your answer to (2).</li>

 <li>Find a general formula (not recursively defined) for <em>U</em>(<em>m</em>). You do not need to argue for your answer, but show that for <em>m </em>= 1<em>,</em>3<em>,</em>8 it coincides with your answer to (2).</li>

</ol>

<ol start="2">

 <li>For each of the following functions <em>f </em>of <em>n</em>, indicate how big the natural number <em>n </em>must be in order for <em>f</em>(<em>n</em>) to be at least 10,000, and for <em>f</em>(<em>n</em>) to be at least 100,000,000 (that is, 10<sup>8</sup>). You may give approximate answers but they should have at least two significant figures.</li>

</ol>

<em>n </em><em> n</em>lg(<em>n</em>)      <em>n</em>√<sup>3 </sup><em>n     n</em>√<em>n                n</em><sup>2 </sup><em>n</em><sup>4 </sup>(1<em>.</em>001)<em><sup>n </sup></em> (1<em>.</em>1)<em><sup>n </sup></em>2<em><sup>n </sup></em>100<em><sup>n </sup>n</em>!                <em>n<sup>n</sup></em>

<ol start="3">

 <li>Prove, using <em>only </em>the definition of “big-<em>O</em>” and <em>not </em>any auxiliary results stated on the slides or in the textbook(s), that

  <ol>

   <li>3<em>n</em><sup>4 </sup>+ 7<em>n</em><sup>3 </sup>+ 6<em>n</em><sup>2 </sup>+ 9<em>n </em>+ 5 ∈ <em>O</em>(<em>n</em><sup>4</sup>)</li>

   <li><em>n</em><sup>5</sup>− 7<em>n</em><sup>4 </sup>+ 2<em>n</em><sup>2</sup>− <em>n /</em>∈ <em>O</em>(<em>n</em><sup>4</sup>)</li>

  </ol></li>

</ol>