1. Let us say that there is some field $(X,+,\cdot)$ , which is of characteristic zero.

Because it is a field, it must contain at least two identity elements.
$1$ : the identity of multiplication
and
$0$ : the identity of addition
$\therefore 0,1\in X$
$(X,+,\cdot)$ is of characteristic zero
$\implies \forall n\in \mathbb{N}, (1+1+1\cdots\cdots$$n$ times$) \neq 0$ 
also, since it is a field, it has the following properties
1. Associativity, Commutativity, and Closure (under addition and multiplication)
2. Distributive property of multiplication over addition
3. Identity (of multiplication and addition)
4. Inverse (multiplicative and additive)

Thus, we have

since binary operators have the property of closure, any addition or multiplication must result in the operators being closed on that field.
	Any field must contain at least two distinct elements: $0$ and $1,$ the identity elements of that field.
	Hence, we have $0, 1\in X$   
	But, the additive inverse of $1$ must also be in $X$
	Let us call this element $-1$. We have $-1+1=0$
	Let $1+1 = 2 \implies$	$2\in X\implies 2+1=3\in X$ (closure of a binary operator in a field)
	By mathematical induction, 
	for some $n\in\mathbb{N}, n\geq2\implies n+1\in X$
	$\therefore\mathbb{N}\subset X$ 
	$\therefore x\in X\implies -x\in X \implies \forall n\in \mathbb{N}, also -n\in X$
	$\therefore \mathbb{Z} \subseteq X$
	but also, $z\in \mathbb{Z}, z\ne0\implies z^{-1}=\frac{1}{z}\in X$  (existence of a unique multiplicative inverse for all elements of a field)
	 but the field is also closed under multiplication
	 $\implies \forall z_1, z_2\in \mathbb{Z}, z_2\ne0, z_1\cdot \frac{1}{z_2}=\frac{z_1}{z_2}\in X$  
	 but also $\mathbb{Q}=$ {$\frac{z_1}{z_2}: z_1, z_2\in\mathbb{Z}, z_2\ne0$}
	 $\therefore \mathbb{Q}\subseteq X \implies$ Any field which is not of characteristic $0$ must contain every rational number.
	 $Q.E.D.$ 

2. 
Prove the following theorem:
To each elementary row operation $e,$ there is a corresponding elementary row operation $e_1$ such that

$e_1(e(A))=e(e_1(A))=A$
i.e., $e_1(A) = e^{-1}(A)$

I.e. prove that there exists an inverse of the elementary row operation and is another elementary row operation of the same type.


Let us take an $m$x$n$ matrix $A$.
1. Let us say consider some elementary row operation as follows, for some row $r$.
   $e(A)_{ij} = A_{ij}$ if $i\neq r$
   $e(A)_{rj} = cA_{rj},$   $c\neq0$
   
   Let us now consider the following row operation:
   $e_1(A)_{ij} = A_{ij}$ if $i\neq r$
   $e_1(A)_{rj} = c^{-1}A_{rj}, c\neq0$
   
   $e_1 (e(A_{ij})) = e_1(A_{ij}) = A_{ij}$   $i\neq r$
   $e_1 (e(A_{ij})) = e_1(cA_{ij}) = c^{-1}(cA_{ij})=A_ij$   $i=r$
   $e (e_1(A_{ij})) = e(c^{-1}A_{ij}) = c(c^{-1}A_{ij})=A_{ij}$   $i= r$
   thus we have that
   $\forall A_{ij}, e(e_1(A_{ij}))=e_1(e(A_{ij}))=A_{ij}$
   $\implies e(e_1(A))=e_1(e(A))=A$


2. Let us now consider the following two elementary row operation  
   $e(A)_{ij} = A_{ij}$ if $i\neq r$
   $e(A)_{rj} = A_{rj}+cA_{sj},$   $c\neq0, r\neq s$
   $e_1(A)_{ij} = A_{ij}$ if $i\neq r$
   $e(A)_{rj} = A_{rj}-cA_{sj},$   $c\neq0, r\neq s$
   thus, 
   
   $e_1 (e(A_{ij})) = e_1(A_{ij}) = A_{ij}$   $i\neq r$
   $e_1 (e(A_{ij})) = e_1(A_{ij}+cA_{sj}) = -cA_{sj}+(A_ij+cA_{sj})=A_ij$   $i=r$
   $e (e_1(A_{ij})) = e(A_{ij}-cA_{sj}) = cA_{sj}+(A_ij-cA_{sj})=A_ij$   $i=r$
   
   thus we have that
   $\forall A_{ij}, e(e_1(A_{ij}))=e_1(e(A_{ij}))=A_{ij}$
   $\implies e(e_1(A))=e_1(e(A))=A$

3. Now consider the following two row operations
   $e(A)_{ij} = A_{ij}$ if $i\neq r, i\neq s, r\neq s$
   $e(A)_{rj} = A_{sj},$   $i=r$ 
   $e(A)_{sj}=A_{rj},$   $i=s$
   and
   $e_1(A)_{ij} = A_{ij}$ if $i\neq r, i\neq s, r\neq s$
   $e_1(A)_{rj} = A_{sj},$   $i=r$ 
   $e_1(A)_{sj}=A_{rj},$   $i=s$

these are clearly the inverse of each other because switching two rows and switching them back results in the same matrix either way.


Therefore, for each elementary row operation $e, \exists$ a corresponding inverse elementary row operation $e_1$ of the same type.


3. 
	1. a
		1. $A=\begin{bmatrix} 1&2\\-1&11 \end{bmatrix}$ $X=\begin{bmatrix} x\\ y\end{bmatrix}$ $Y=\begin{bmatrix} 18\\ 23\end{bmatrix}$
			1. add the first row to the second row     $A_1=\begin{bmatrix} 1&2\\0&13 \end{bmatrix}$ $Y_1=\begin{bmatrix} 18\\ 41\end{bmatrix}$
			2. multiply the second row by$\frac 1{13}$$A_2=\begin{bmatrix} 1&2\\0&1 \end{bmatrix}$ $Y_2=\begin{bmatrix} 18\\ \frac{41}{13}\end{bmatrix}$
			3. subtract twice the second row from the first $A_3=\begin{bmatrix} 1&0\\0&1 \end{bmatrix}$ $Y_3=\begin{bmatrix} \frac{152}{13}\\ \frac{41}{13}\end{bmatrix}$
			4. $A_3X=Y_3$
			5. $\implies x=\frac{152}{13}, y=\frac{41}{13}$ 
		2. $A=\begin{bmatrix} -2&9\\8&-10 \end{bmatrix}$$X=\begin{bmatrix} x\\ y\end{bmatrix}$$Y=\begin{bmatrix} 5\\ 62\end{bmatrix}$
			1. multiply the first row by $\frac{-1}{2}$    $A_1=\begin{bmatrix} 1&\frac{-9}2\\8&-10 \end{bmatrix}$ $Y_1=\begin{bmatrix} \frac{-5}{2} \\ 62 \end{bmatrix}$ 
			2. subtract eight times the first row from the second $A_2=\begin{bmatrix} 1&\frac{-9}2\\0&26 \end{bmatrix}$ $Y_2=\begin{bmatrix} \frac{-5}{2} \\ 82 \end{bmatrix}$ 
			3. multiply the second row by $\frac1{26}$ $A_3=\begin{bmatrix} 1&\frac{-9}2\\0&1 \end{bmatrix}$ $Y_3=\begin{bmatrix} \frac{-5}{2} \\ \frac{41}{13} \end{bmatrix}$ 
			4. subtract the second row $\frac{-9}{2}$ times from the first row $A_4=\begin{bmatrix} 1&0\\0&1 \end{bmatrix}$ $Y_4=\begin{bmatrix} \frac{152}{13}\\ \frac{41}{13}\end{bmatrix}$ 
			5. $A_4X=Y_4$
			6. $\implies x=\frac{152}{13}, y=\frac{41}{13}$ 
		Thus, these two systems are equivalent.
	2. b
		1. $A=\begin{bmatrix} 1&1&1\\0&1&2\\1&0&3\end{bmatrix}$ $X=\begin{bmatrix} x\\ y\\ z\end{bmatrix}$$Y=\begin{bmatrix} 6\\5\\ 6\end{bmatrix}$
			1. subtract the first row from and add the second row to the third row $A_1=\begin{bmatrix} 1&1&1\\0&1&2\\0&0&4\end{bmatrix}$ $Y_1=\begin{bmatrix} 6\\5\\ 5\end{bmatrix}$
			2. multiply the third row by $\frac 14$ $A_2=\begin{bmatrix} 1&1&1\\0&1&2\\0&0&1\end{bmatrix}$ $Y_2=\begin{bmatrix} 6\\5\\ \frac54\end{bmatrix}$
			3. subtract the third row once from the first row and twice from the second row $A_3=\begin{bmatrix} 1&1&0\\0&1&0\\0&0&1\end{bmatrix}$ $Y_3=\begin{bmatrix} \frac{19}4\\\frac52\\ \frac54\end{bmatrix}$
			4. subtract the second row from the first row $A_4=\begin{bmatrix} 1&0&0\\0&1&0\\0&0&1\end{bmatrix}$ $Y_4=\begin{bmatrix} \frac94\\\frac52\\ \frac54\end{bmatrix}$
			5. $A_4X=Y_4\implies$ $x=\frac94, y=\frac52, z=\frac54$
		2.  $A=\begin{bmatrix} 3&2&-1\\3&1&-1\\0&1&1\end{bmatrix}$ $X=\begin{bmatrix} x\\ y\\ z\end{bmatrix}$ $Y=\begin{bmatrix} 12\\10\\3\end{bmatrix}$ 
			1. subtract the first row from the second row and then multiply that row by $-1$ $A_1=\begin{bmatrix} 3&2&-1\\0&1&0\\0&1&1\end{bmatrix}$ $Y_1=\begin{bmatrix} 12\\2\\ 3\end{bmatrix}$
			2. subtract the second row from the third and then subtract the second from the first twice and add the third once to the first. multiply the first row by $\frac13$ $A_2=\begin{bmatrix} 1&0&0\\0&1&0\\0&0&1\end{bmatrix}$ $Y_2=\begin{bmatrix} 3\\2\\ 1\end{bmatrix}$
			3. $A_2X=Y_2\implies$ $x=3, y=2, z=1$
		3.  $A=\begin{bmatrix} 1&1&-1\\2&1&0\\1&0&-1\end{bmatrix}$ $X=\begin{bmatrix} x\\ y\\ z\end{bmatrix}$  $Y=\begin{bmatrix} 4\\8\\2\end{bmatrix}$
			1. subtract the third row from the second twice, then subtract the second from the first $A_1=\begin{bmatrix} 1&0&-3\\0&1&2\\1&0&-1\end{bmatrix}$ $Y_1=\begin{bmatrix} 0\\4\\ 2\end{bmatrix}$
			2. subtract the first from the third, subtract the third from the second and multiply by the third by $\frac12$ $A_2=\begin{bmatrix} 1&0&-3\\0&1&0\\0&0&1\end{bmatrix}$ $Y_2=\begin{bmatrix} 0\\2\\ 1\end{bmatrix}$
			3. add the third row thrice to the first row $A_3=\begin{bmatrix} 1&0&0\\0&1&0\\0&0&1\end{bmatrix}$ $Y_3=\begin{bmatrix} 3\\2\\1\end{bmatrix}$
			4. $A_3X=Y_3\implies$ $x=3, y=2, z=1$
		Thus, the third system is equivalent to the second but not the first.
5.  Let us consider an $m$x$n$ matrix $A_{mn}$ 
Let the first column of $A$  containing a non-zero element be column $j,$ and the first such non-zero element be in row $i$.
Let us now take this $a_{ij}\neq 0$ and perform the following elementary row operations. 
1. multiply row $r_i$ with  $\frac1{a_{ij}}$ 
2. swap rows $r_i$ and $r_1$
As a result of these elementary row operations, the first column containing a non-zero element is column $j$, and the first row containing a non-zero element is now row $r_1$.  Now, if there is any other row $r_k$ which contains a non-zero element in column $j,$ then we will subtract row $r_1,$  $a_{kj}$ times from that row $r_k$. Now, the only element in column $j$ which is not zero is $a_{1j}=1$.

Now, let us take the next such column $p$ which has its first non zero element in row $q$. Also, $p>j, q\neq1$. Now, repeat such a process. That is, 
1. multiply row $r_q$ with $\frac1{a_{qp}}$ 
2. swap the row $r_q$ and $r_2$
3. subtract the row $r_2,$ $a_{sp}$ times, from each row $r_s$ with a non-zero element in column $p$ and

Repeat this three-step process for each remaining column with non-zero elements, such that the column number is less than $m$. 

Thus, we will have obtained the row-reduced echelon form of the matrix, because we have satisfied the four conditions above which are both necessary and sufficient for a matrix to be considered a row-reduced echelon matrix.

$R$ is considered a row reduced echelon matrix if and only if:
1. The first non zero element of each row of the matrix should be $1$.
2. For each column in which the leading entry ($1$) is, all the other elements should be $0$.
3. Every zero-row (a row which has all $0$ entries) of $R$  occurs below every non-zero row.
3. if the rows $1,2, \cdots\cdots , r$ are the non-zero rows of $R$ and if the leading non-zero entry of row $i$ occurs in column $k_i (i=1, \cdots r),$ then $k_1<k_2<k_3<\cdots<k_r$  




























Thus, $-1\neq 1$ because otherwise the field would be of characteristic $2$, not $0$.
	Now, 
	$1\in X\implies 1+1\in X, 1+1\neq0 \because$ it is not of characteristic $0$. 
	We also have that $1+1\neq-1$ because then the field would be of characteristic $3$.

