
Discrete Mathematics
===
MTH 309 Course Notes. Will continuously update as the class goes on. 


Counting
---
1. __Multiplication rule__ 	
	We perform a task, which can be broken into k independent steps. Each step can be complete d in  <img src="http://latex.codecogs.com/gif.latex?n_{1},n_{2},...,n_{k}" border="1"/> ways. Entire task can be completed in <img src="http://latex.codecogs.com/gif.latex?n_{1},n_{2},...,n_{k}" border="1"/> .
2. __Addition rule__ 	
	If a task can be completed in k mutually exclusive ways, then <img src="http://latex.codecogs.com/gif.latex?N = n_{1}+n_{2}+...+n_{k}" border="0"/>  is the number of choices for the <img src="http://latex.codecogs.com/gif.latex?N = i_th" border="0"/> order.
3. __Permutation__ 	
	In general, the number of permutation of n objects is _n!_.
	
4. __Selection with Repetition__
	+ Ordered with repetition	
	There are <img src="http://latex.codecogs.com/gif.latex?n^{r}" border="0"/> ways to do an ordered r selection out of n objects
	+ Unordered with repetition	
	
		There are ![{n+r-1\choose r}][equation_unorderrep] ways to do an unordered r selection out of n objects
	
5. __Important equation__
	+ <img src="http://latex.codecogs.com/gif.latex?{n + 1\choose k}  =  {n\choose k}  +  {n\choose k-1}" border="0"/>

	+ <img src="http://latex.codecogs.com/gif.latex?{n\choose m}{m\choose r} = {n\choose r} + {n-r \choose m-r}"  border="0"/> 

	+ <img src="http://latex.codecogs.com/gif.latex?(x+y)^{n} = \sum_{k=0}^{n} {n\choose k}x^{n-k}y^{k}" border="0"/> 
	
	+ <img src="http://latex.codecogs.com/gif.latex?(2)^{n} = \sum_{k=0}^{n} {n\choose k}" border="0"/>
	
	+ <img src="http://latex.codecogs.com/gif.latex?0^{n} = \sum_{k=0}^{n} {n\choose k}(-1)^{k}" border="0"/>

	

Recurrence
---
Recurrence relation is representation of nth number <img src="http://latex.codecogs.com/gif.latex?a_{n}" border="0"/> in a sequence is connect to previous states <img src="http://latex.codecogs.com/gif.latex?a_{i}">, i<n. 

__Solving recurrence equation__		

+	Level 1
	+  Homogeneous
	
		<img src="http://latex.codecogs.com/gif.latex?a_{n} = Ca_{n-1}, a_{1} = A       -> a_{n} = AC^{n-1}">
	+ Non-homogeneous  
		1. Find special solution by substitute non-homogeneous part to the recurrence equation, and then calculate the equation, find the coefficient of special solution, _k_. 
		2. Substitute the special solution to the recurrence equation and then substitute the initial condition   ![a_{1}][equation1] to calculate the coefficient A. 
	
+ 	Level 2
	+  Homogeneous
		1. Given that ![a_{n}=pa_{n-1}+qa_{n-2}][level2_homodef], write the characteristic equation by replace ![a_{n}][a_n] by  ![\lambda^{2}][lamda^2] and others respectively. by solving the equation ![\lambda^{2}+p\lambda+q][charequation], we got ![\lambda_{1}][lambda1] and ![\lambda_{2}][lambda2]. Then substitute the two ![\lambda][lambda] to the given recurrence equation, an pseudo equation can be calculated: ![a_{n} = A\lambda_{1}^{n}+b\lambda_{2}^{n}][homo_2_pseudo]
		2. Substitute the initial conditions to the pseudo equation, calculate _A_ and _B_.  
	+ Non-homogeneous   


	
	
	
	
	
	
Reference
---
[equation_unorderrep]: http://latex.codecogs.com/gif.latex?{n+r-1\choose%20r}
[equation1]: http://latex.codecogs.com/gif.latex?a_{1}
[level2_homodef]: http://latex.codecogs.com/gif.latex?a_{n}=pa_{n-1}+qa_{n-2}
[a_n]:http://latex.codecogs.com/gif.latex?a_{n}
[lamda^2]:http://latex.codecogs.com/gif.latex?\lambda^{2}
[charequation]: http://latex.codecogs.com/gif.latex?\lambda^{2}+p\lambda+q
[lambda1]: http://latex.codecogs.com/gif.latex?\lambda_{1}
[lambda2]: http://latex.codecogs.com/gif.latex?\lambda_{2}
[lambda]: http://latex.codecogs.com/gif.latex?\lambda
[homo_2_pseudo]: http://latex.codecogs.com/gif.latex?a_{n}=A\lambda_{1}^{n}+b\lambda_{2}^{n}
