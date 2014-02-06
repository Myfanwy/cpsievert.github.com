Stat 226 - Lecture 8
========================================================
date: 02/06/14
transition: rotate
incremental: true

Back to Empirical Rule
========================================================

<div align="center">
<img src="empirical.gif" width="650" height="400">
</div>

* OK, but what if I want to find something like $P(Z < -0.5)$?
* This is what Table A is for!

Visualizing Table A
========================================================
incremental:false

<div align="center">
<iframe src="http://glimmer.rstudio.com/cpsievert/cdf/" width="650" height="600"></iframe>
</div>


Some useful facts
========================================================

* Using Table A requires reducing probability statements down to $P(Z < a)$, for some number $a$.
* Given $X \sim N(\mu, \sigma^2)$:
  * $P(X > a) = 1 - P(X < a)$
  * $P(a < X < b) = P(X < b) - P(X < a)$
* Given $Z \sim N(0, 1)$ for any __positive__ number $a$:
  * $P(Z > a) = P(Z < -a)$
  
Your turn
========================================================
incremental:false

* Find the following probabilities using Table A:
  * $P(Z < -1.64)$
  * $P(Z > -0.56)$
  * $P(-1 < Z < 2.27)$
  * $P(Z > 4)$
  
Finding probabilities for any X
========================================================

* Last time we learned how $X \sim N(\mu, \sigma)$ translates to $Z \sim N(0,1)$ via a __z-score__:

<div align="center" class="fragment">$$z = \frac{x-\mu}{\sigma}$$</div>
* Suppose $X \sim N(10, 25)$. 

* $P(X > 15) =$ <div style="display:inline-block" class="fragment"> $P(X-10 > 5) =$ </div> <div style="display:inline-block" class="fragment"> $P(\frac{X-10}{5} > \frac{15-10}{5}) =$ </div> <div style="display:inline-block" class="fragment"> $P(Z > 1)$
* <div style="display:inline-block" class="fragment"> $P(Z > 1) =$ <div style="display:inline-block" class="fragment"> $P(Z < -1) =$ </div> <div style="display:inline-block" class="fragment"> .1587 </div>

Your Turn
========================================================

* Find the following probabilities using Table A:
* Given $X \sim N(150, 100)$, find:
  * $P(X < 137)$
  * $P(X > 137)$
  * $P(140 < X < 165)$
* Given $Y \sim N(-10, 3^2)$, find:
  * $P(Y > -9)$
  * $P(-9 < Y < -7)$
  
Percentiles
========================================================

* __Definition__: The $p^{th}$ percentile is a value, say $v$, where $p$ percent of observations are lower than $v$.
* __Example__:
  * Remember that for the normal distribution, mean = median!
  * Thus, the median of the __standard__ normal is...<div style="display:inline-block" class="fragment"> 0! </div>
  * Therefore the __50th percentile__ of the standard normal is ...<div style="display:inline-block" class="fragment"> 0! </div>
  
Visualizing Percentiles
========================================================

<div align="center">
<iframe src="http://glimmer.rstudio.com/cpsievert/cdf/" width="650" height="600"></iframe>
</div>

Your Turn
========================================================
incremental:false

* Find the value of $z^*$ for each of the following scenarios:
  * P(Z < z^*) = 0.025 (__Note__: $z^*$ is called the 2.5th percentile)
  * P(Z < z^*) = 0.975 (__Note__: $z^*$ is called the 97.5th percentile)
  * P(Z < z^*) = 0.25 (__Note__: $z^*$ is called the 25th percentile)

Finding percentiles for any X
========================================================

* As before, $X \sim N(\mu, \sigma)$ translates to $Z \sim N(0,1)$ via a __z-score__:

<div align="center" class="fragment">$$z = \frac{x-\mu}{\sigma}$$</div>

* Rearranging this equation a bit gives us:

<div align="center" class="fragment">$$z \times \sigma + \mu = x$$</div>

* Thus, if $z^*$ is the $p^{th}$ percentile of the __standard__ normal, then $\mu + \sigma \times z^*$ is the $p^{th}$ percentile of $X \sim N(\mu, \sigma)$!

Average Debt
========================================================

* __Example:__ Let $X$ be the debt of an ISU undergraduate upon graduation (in thousands of dollars). Suppose $X$ is known to have a mean of 20 and standard deviation of 5.
  * How much debt does it take to have __more__ debt than 95% of other undergraduates?
  * In other words, what value of $z^*$ gives us $P(Z < z^*) = 0.95$?
  * From Table A, $z^* =$ 1.64 or 1.65 (either one is fine).
  * Using our 'backwards z-score calculation': $x = \mu + \sigma \times z^* = 20 + 5 \times 1.65 =$ 28.25
  * So, if you have $28,500 in debt upon graduating, you have more debt than 95% of graduates!
  
Your Turn
========================================================
incremental:false

* Suppose $X \sim N(12, 2^2)$. Find the value of $x^*$ for each of the following scenarios:
  * P(X < x^*) = 0.33 (__Note__: $z^*$ is called the 33rd percentile)
  * P(X < x^*) = 0.66 (__Note__: $z^*$ is called the 66th percentile)
  * P(X < x^*) = 0.01 (__Note__: $z^*$ is called the 1st percentile)