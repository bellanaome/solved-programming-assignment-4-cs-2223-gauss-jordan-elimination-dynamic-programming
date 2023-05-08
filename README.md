Download Link: https://assignmentchef.com/product/solved-programming-assignment-4-cs-2223-gauss-jordan-elimination-dynamic-programming
<br>



<ol>

 <li>(4 Points) Explain why the <em>ForwardElimination </em>algorithm on page 210 of Levitin fails to provide a solution for:</li>

</ol>

<table width="193">

 <tbody>

  <tr>

   <td width="28"><em>x</em><sub>1</sub></td>

   <td width="25">+</td>

   <td width="36"><em>x</em><sub>2</sub></td>

   <td width="25">+</td>

   <td width="36"><em>x</em><sub>3</sub></td>

   <td width="25">=</td>

   <td width="16">6</td>

  </tr>

  <tr>

   <td width="28"><em>x</em><sub>1</sub></td>

   <td width="25">+</td>

   <td width="36"><em>x</em><sub>2</sub></td>

   <td width="25">+</td>

   <td width="36">2<em>x</em><sub>3</sub></td>

   <td width="25">=</td>

   <td width="16">9</td>

  </tr>

  <tr>

   <td width="28"><em>x</em><sub>1</sub></td>

   <td width="25">+</td>

   <td width="36">2<em>x</em><sub>2</sub></td>

   <td width="25">+</td>

   <td width="36">3<em>x</em><sub>3</sub></td>

   <td width="25">=</td>

   <td width="16">14</td>

  </tr>

 </tbody>

</table>

despite the fact that <em>x </em>= (1<em>,</em>2<em>,</em>3) or <em>x</em><sub>1 </sub>= 1, <em>x</em><sub>2 </sub>= 2, <em>x</em><sub>3 </sub>= 3 can be easily verified as a solution to the system.

How does the <em>BetterForwardElimination </em>algorithm on page 211 of Levitin remedy this?

<ol start="2">

 <li>(6 Points) Explain in some detail why the <em>BetterForwardElimination </em>algorithm on page 211 of Levitin fails to provide a solution for:</li>

</ol>

<table width="201">

 <tbody>

  <tr>

   <td width="36"><em>x</em><sub>1</sub></td>

   <td width="25">+</td>

   <td width="36"><em>x</em><sub>2</sub></td>

   <td width="25">+</td>

   <td width="36"><em>x</em><sub>3</sub></td>

   <td width="25">=</td>

   <td width="16">6</td>

  </tr>

  <tr>

   <td width="36"><em>x</em><sub>1</sub></td>

   <td width="25">+</td>

   <td width="36"><em>x</em><sub>2</sub></td>

   <td width="25">+</td>

   <td width="36">2<em>x</em><sub>3</sub></td>

   <td width="25">=</td>

   <td width="16">9</td>

  </tr>

  <tr>

   <td width="36">2<em>x</em><sub>1</sub></td>

   <td width="25">+</td>

   <td width="36">2<em>x</em><sub>2</sub></td>

   <td width="25">+</td>

   <td width="36">3<em>x</em><sub>3</sub></td>

   <td width="25">=</td>

   <td width="16">15</td>

  </tr>

 </tbody>

</table>

despite the fact that <em>x </em>= (1<em>,</em>2<em>,</em>3) or <em>x</em><sub>1 </sub>= 1, <em>x</em><sub>2 </sub>= 2, <em>x</em><sub>3 </sub>= 3 can be easily verified as a solution to the system.

What can be done to remedy this shortcoming in the algorithm?

1

<ol start="3">

 <li>(20 Points) The <strong>Gauss-Jordan elimination </strong>method differs from Gaussian elimination in that the elements above the main diagonal of the coefficient matrix are made zero at the same time and by the same use of a pivot row as the elements below the main diagonal. Thus, the coefficient matrix is transformed into a diagonal matrix rather than an upper-triangular matrix. Furthermore, if each pivot row is “divided by” its pivot (leading entry) prior to its use as a pivot row, the coefficient matrix is transformed into the identity matrix, and the back substitution step may be dispensed with entirely. That is, the solution <em>x </em>is simply the last column of the (transformed) augmented system matrix.</li>

</ol>

Modify the <em>BetterForwardElimination </em>algorithm to perform Gauss-Jordan elimination to solve a system of <em>n </em>linear equations in <em>n </em>unknowns with the form <em>Ax </em>= <em>b</em>, where <em>A </em>is an <em>n </em>× <em>n </em>matrix of real coefficients<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a>, and <em>b </em>is a column vector with <em>n </em>real entries.

Use your algorithm to find the unique solution to the system:

<em>x</em><sub>1 </sub>+ <em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>+ <em>x</em><sub>4 </sub>+ <em>x</em><sub>5 </sub>+ <em>x</em><sub>6 </sub>+ <em>x</em><sub>7 </sub>+ <em>x</em><sub>8 </sub>= 0 <em>x</em><sub>1 </sub>+ 2<em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>+ <em>x</em><sub>4 </sub>+ <em>x</em><sub>5 </sub>+ <em>x</em><sub>6 </sub>+ 2<em>x</em><sub>7 </sub>+ <em>x</em><sub>8 </sub>= 0 <em>x</em><sub>1 </sub>+ <em>x</em><sub>2 </sub>+ 3<em>x</em><sub>3 </sub>+ <em>x</em><sub>4 </sub>+ <em>x</em><sub>5 </sub>+ 3<em>x</em><sub>6 </sub>+ <em>x</em><sub>7 </sub>+ <em>x</em><sub>8 </sub>= 0 <em>x</em><sub>1 </sub>+ <em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>+ 4<em>x</em><sub>4 </sub>+ 4<em>x</em><sub>5 </sub>+ <em>x</em><sub>6 </sub>+ <em>x</em><sub>7 </sub>+ <em>x</em><sub>8 </sub>= 0 11<em>x</em><sub>1 </sub>+ <em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>+ <em>x</em><sub>4 </sub>+ <em>x</em><sub>5 </sub>+ <em>x</em><sub>6 </sub>+ <em>x</em><sub>7 </sub>+ <em>x</em><sub>8 </sub>= 20 <em>x</em><sub>1 </sub>+ <em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>+ <em>x</em><sub>4 </sub>− <em>x</em><sub>5 </sub>− <em>x</em><sub>6 </sub>− <em>x</em><sub>7 </sub>− <em>x</em><sub>8 </sub>= 34 <em>x</em><sub>1 </sub>+ 2<em>x</em><sub>2 </sub>+ 3<em>x</em><sub>3 </sub>+ 4<em>x</em><sub>4 </sub>+ 5<em>x</em><sub>5 </sub>+ 6<em>x</em><sub>6 </sub>+ 7<em>x</em><sub>7 </sub>+ 8<em>x</em><sub>8 </sub>= −51 <em>x</em><sub>1 </sub>− <em>x</em><sub>2 </sub>+ <em>x</em><sub>3 </sub>− <em>x</em><sub>4 </sub>+ <em>x</em><sub>5 </sub>− <em>x</em><sub>6 </sub>+ <em>x</em><sub>7 </sub>− <em>x</em><sub>8 </sub>= −6

<ol start="4">

 <li>(30 Points) The Dwarf King has locked the Heart of the Mountain, the jewel known as the Arkenstone, in one of the vaults in the deepest treasure room under the Lonely Mountain. The square floor of the room consists of 64 smaller squares, alternating gold and silver. (It is believed that ancient Persians, having discovered the chamber long after the age of Dwarves, were inspired by its beauty to create games played on such a surface.) Upon each square the King has arrayed a varying number of the most wondrous gemstones: emeralds, rubies, sapphires, diamonds, and more, as shown here:</li>

</ol>

<table width="511">

 <tbody>

  <tr>

   <td width="65">Vault 1</td>

   <td width="64">Vault 2</td>

   <td width="64">Vault 3</td>

   <td width="64">Vault 4</td>

   <td width="64">Vault 5</td>

   <td width="64">Vault 6</td>

   <td width="64">Vault 7</td>

   <td width="65">Vault 8</td>

  </tr>

  <tr>

   <td width="65">89</td>

   <td width="64">70</td>

   <td width="64">73</td>

   <td width="64">83</td>

   <td width="64">90</td>

   <td width="64">22</td>

   <td width="64">44</td>

   <td width="65">92</td>

  </tr>

  <tr>

   <td width="65">46</td>

   <td width="64">23</td>

   <td width="64">99</td>

   <td width="64">77</td>

   <td width="64">10</td>

   <td width="64">42</td>

   <td width="64">1</td>

   <td width="65">72</td>

  </tr>

  <tr>

   <td width="65">85</td>

   <td width="64">52</td>

   <td width="64">27</td>

   <td width="64">5</td>

   <td width="64">94</td>

   <td width="64">91</td>

   <td width="64">82</td>

   <td width="65">62</td>

  </tr>

  <tr>

   <td width="65">22</td>

   <td width="64">93</td>

   <td width="64">68</td>

   <td width="64">11</td>

   <td width="64">56</td>

   <td width="64">63</td>

   <td width="64">49</td>

   <td width="65">35</td>

  </tr>

  <tr>

   <td width="65">13</td>

   <td width="64">78</td>

   <td width="64">48</td>

   <td width="64">19</td>

   <td width="64">78</td>

   <td width="64">11</td>

   <td width="64">90</td>

   <td width="65">94</td>

  </tr>

  <tr>

   <td width="65">31</td>

   <td width="64">5</td>

   <td width="64">63</td>

   <td width="64">10</td>

   <td width="64">32</td>

   <td width="64">40</td>

   <td width="64">14</td>

   <td width="65">13</td>

  </tr>

  <tr>

   <td width="65">73</td>

   <td width="64">38</td>

   <td width="64">24</td>

   <td width="64">49</td>

   <td width="64">18</td>

   <td width="64">6</td>

   <td width="64">40</td>

   <td width="65">74</td>

  </tr>

  <tr>

   <td width="65">79</td>

   <td width="64">71</td>

   <td width="64">18</td>

   <td width="64">20</td>

   <td width="64">34</td>

   <td width="64">51</td>

   <td width="64">93</td>

   <td width="65">65</td>

  </tr>

 </tbody>

</table>

Row 8

Row 7

Row 6

Row 5

Row 4

Row 3

Row 2

Row 1

The vault containing the Arkenstone is sealed with powerful magic which can only be broken by someone who has walked the Most Precious Path. Bilbo Baggins, the Hobbit burglar, having once possessed the Arkenstone, wishes to behold it once again. Devise and implement in C++ a dynamic programming algorithm which will allow Mr. Baggins to collect the greatest number of gemstones given that he:

<ul>

 <li>begins by collecting the gems on the square of his choice in Row 1, and then moves to

  <ul>

   <li>the square directly ahead of the one he currently occupies, or</li>

   <li>the square (diagonally) ahead and to the left of the one he currently occupies, provided that he is not already against the left wall of the treasure room, or</li>

   <li>the square (diagonally) ahead and to the right of the one he currently occupies, provided that he is not already against the right wall of the treasure room;</li>

  </ul></li>

 <li>collects the gems from the newly-visited square, and</li>

 <li>repeats this process until,</li>

 <li>he collects gems from a square on Row 8, whereupon the spell sealing the corresponding door will be broken and the vault will yield its treasure if and only if Bilbo has walked the Most Precious Path.</li>

</ul>

Your output should include:

<ul>

 <li>Bilbo’s starting square,</li>

 <li>a representation of his path,</li>

 <li>the total number of gems collected on the way, and</li>

 <li>the number of the vault wherein the King has secreted the Arkenstone.</li>

</ul>

<a href="#_ftnref1" name="_ftn1">[1]</a> Note: We may revisit this algorithm later, but for now you can assume that an 8 × 9 array of reals (or doubles!) will suffice.