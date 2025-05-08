# Question 8
## Consider the functions $f:{1,2,3,4,5,6,7} -> {0,1,2,3,4,5,6,7,8,9,10}$. 
### a. How many of these functions are strictly increasing? Explain. (A function is strictly increasing provided if $a < b$ then $f(a) < f(b)$.)
To solve this problem, we simply must use combinations. There are 11 outputs and
7 inputs, so, as combinations are always counting outputs, we must write $C(11, 7)$ or $\begin{pmatrix} 11\cr7\cr\end{pmatrix}$. This is then plugged into the combination formula ($\frac{n!}{(n-k)!k!}$), will result in $\frac{11!}{(11-7)!7!)}$ to get you a final answer of **330**.
### b. How many of the functions are non-decreasing? Explain. (A function is non-decreasing provided if $a < b$, then $f(a) \leq f(b)$.) 
To solve this problem, we must think using sticks and stones. As the problem
says, this must have functions where $f(a) \leq f(b)$. The sticks in this problem are the number of inputs minus 1. This is because the sticks denote value changes, with each change, not each value. This gives you $7-1=6$ sticks. Adding this with the number of stones (the output values) gives you the top number of your choosing. The bottom number is the number of inputs. This gives you $\begin{pmatrix}11+7-1\cr7\cr\end{pmatrix}$ or $\begin{pmatrix}17\cr7\cr\end{pmatrix}$ or the combination $C(17,7)$. This, when plugged into the combination formula, gives you $\frac{17!}{(17-7)!7!}$ to get a final answer of **19448**.
