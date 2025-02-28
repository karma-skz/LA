1. If $A,B,C$ are matrices over a field $F$ such that the products $BC$ and $A(BC)$ are well defined, and so are the products $AB$ and $(AB)C,$ then prove that $$A(BC) = (AB)C$$
	Let us consider the matrices $A_{m×n}, B_{n×p}, C_{p×s}$ such that the $j^{th}$ element of the $i^{th}$ row be represented by $a_{ij}, b{ij},$ and $c_{ij}$ . If two matrices are being multiplied, the number of columns in the first matrix must be equal to the number of rows in the first. For this reason, the number of columns of $A$ must be equal to the number of rows of $BC,$ and the number of columns of $B$ must be equal to the number of rows of $C,$ because the products $A(BC)$ and $BC$ are well defined. And by this extension, we also have that the number of rows of $BC$ must be equal to the number of rows of $B$ because that is how the product of two matrices is defined. thus, we have $(BC)_{n×s}$.  Thus, since the number of rows of $B$ is equal to the number of rows of $A,$ by definition, the product matrix $AB_{m×p}$ is also well defined and the elements $(ab)_{ij}$ of $AB$ are defined such that $$(ab)_{ij} = \sum_{q=1}^n a_{iq} \cdot b_{qj}$$
	
	In this regard, let us evaluate the left hand side of the equation, first.
	We have that the product $BC$ is well defined. and each element $(bc)_{ij},$ which is the $j^{th}$ element of the $i^{th}$ row of the well defined product $BC$ is equal to:
	$$(bc)_{ij} = \sum_{r=1}^s b_{ir}\cdot c_{rj}$$This also means that the product $(A(BC))_{m×s}$ exists because the number of columns of $A$ is equal to the number of rows of $BC$. And by the definition of the product of two matrices, the $j^{th}$ element of the $i^{th}$ row of the matrix $(A(BC))_{m×s},$ $$(a(bc))_{ij} = \sum_{q=1}^n a_{iq}\cdot (bc)_{qj} = \sum_{q=1}^n{(a_{iq}\cdot\sum_{r=1}^s b_{qr}\cdot c_{rj})} =  \sum_{q=1}^n \sum_{r=1}^s\frac{(a_{iq}\cdot b_{qr}\cdot c_{rj})}{s}$$
	Now let us evaluate the right hand side. Again since the numbers of rows and columns are compatible, and there exists a well defined product matrix $(AB)_{m×p}$, there exists another well defined product matrix $((AB)C){m×s}$. We must now evaluate what each element of this matrix will be. We have that the $j^{th}$ element of the $i^{th}$ row is $$((ab)c)_{ij} = \sum_{r=1}^s (ab)_{ir}\cdot c_{rj} = \sum_{r=1}^s {(\sum_{q=1}^n a_{iq} \cdot b_{qr})}\cdot c_{rj} =\sum_{q=1}^n \sum_{r=1}^s\frac{(a_{iq}\cdot b_{qr}\cdot c_{rj})}{s} $$
	Thus, we have that every element $(a(bc))_{ij} = ((ab)c)_{ij}$. $\implies$ every $j^{th}$ element of the $i^{th}$ row of $A(BC)$ is equal to the corresponding $j^{th}$ element of the $i^{th}$ row of $(AB)C$. $\implies$ the matrices are equal $\implies$ $A(BC) = (AB)C$  
2. Let $e$ be an elementary row operation and let $E$ be an elementary matrix of size $m×m$ such that $E=e(\mathbb1_{m×m})$. Prove that $e(A)=EA$ holds $\forall$ matrices $A$ of size $m×n$. 
	Let us begin by recalling the definition of an elementary  matrix: an elementary matrix is obtained from the identity matrix $\mathbb{1}_{m \times m}$ by performing a single elementary row operation.
	There are three types of elementary row operations.
	Let us represent $A$ as a row of columns: $A = [c_1,c_2,\ldots, c_n]$ and $E$ as a column of rows $E = [r_1,r_2, \ldots, r_m$]. Multiplying $EA$ is equivalent hence, to multiplying each row of $E$ with each column $A$. I.e. we need to mupltiply each $r_a$ by each $c_b$. Let $E_{ij}$ signify the $j^{th}$ element of the $i^{th}$ row.
	Now let us recall what the rows are as a result of matrix multiplication. Each $i^{th}$ row $\gamma_i$ of the product of matrices $A$ and $B$ is given by: $$\gamma_i =[\sum^p_{r=1}a_{ir}b_{r1}\sum^p_{r=1}a_{ir}b_{r2} \cdots \cdots \sum^p_{r=1}a_{ir}b_{rn}]$$
	This where $a_{ij}$ and $b_{ij}$ represent the $j^{th}$ element of the $i^{th}$ row of some matrices $A_{m\times p}$ and $B_{p\times n}$ being multiplied.
	
	1. Multiplication of a row by a scalar
		Let us the multiply the $i^{th}$ row of the matrix $\mathbb1_{m\times m}$ by $x$ . Now each $r_a$ has $1$ on the $E_{aa} =1$ and zeroes everywhere else, except $r_i$.  $r_i$ has $E_{ii} = x$ and zeroes everywhere else.
		Now, let us examine the rows of the product $EA$.
		By the definition of matrix multiplication, each row $\gamma_k$ of their product is given by $$\gamma_k =[\sum^m_{r=1}E_{kr}A_{r1}\sum^m_{r=1}E_{kr}A_{r2} \cdots \cdots \sum^m_{r=1}E_{kr}A_{rn}]$$
		Now for every row $\gamma_k, k\neq i,$ we have $E_{kk}=$ and $E_{kl} = 0, \forall l\neq k$. Now this also means that for every row $\gamma_k, k\neq i,$ 
		$$\gamma_k =[E_{kk}A_{k1} \space E_{kk}A_{k2}\cdots \cdots E_{kk}A_{kn}]$$but, $E_{kk} = 1 \implies$$$\gamma_k =[A_{k1} \space A_{k2}\cdots \cdots A_{kn}]$$ which is nothing but the $k^{th}$ row of $A$ itself. Now let us examine the row $\gamma_i$ $$\gamma_i = [\sum^m_{r=1}E_{ir}A_{r1}\sum^m_{r=1}E_{ir}A_{r2} \cdots \cdots \sum^m_{r=1}E_{ir}A_{rn}] = [E_{ii}A_{i1} , E_{ii}A_{i2} ,\cdots \cdots E_{ii}A_{in}]$$
		but, $E_{ii} = x\implies$		$$\gamma_i = [xA_{i1} , xA_{i2},\ldots xA_{in}]$$
		But this row is nothing but the $i^{th}$ row of $A$ multiplied by $x$. All the other rows remain the same. Thus, we have that this new matrix $EA$ is nothing but a result of the same elementary row operation performed on $A$. 
		I.e., $e(A) = EA$	
		
	2. Adding a scalar times another row to a row
		Let us add the $j^{th}$ row $x$ times to the $i^{th}$ row of the matrix $\mathbb1_{m\times m}$. Now each $r_a$ has $1$ on the $E_{aa} =1$ and zeroes everywhere else, except $r_i$.  $r_i$ has $E_{ii} = 1$ and $E_{ij} =x$.      
		Now, let us examine the rows of the product $EA$.
		By the definition of matrix multiplication, each row $\gamma_k$ of their product is given by $$\gamma_k =[\sum^m_{r=1}E_{kr}A_{r1}\sum^m_{r=1}E_{kr}A_{r2} \cdots \cdots \sum^m_{r=1}E_{kr}A_{rn}]$$
		Now for every row $\gamma_k, k\neq i,$ we have $E_{kk}=1$ and $E_{kl} = 0, \forall l\neq k$. Now this also means that for every row $\gamma_k, k\neq i,$ 		$$\gamma_k =[E_{kk}A_{k1} \space E_{kk}A_{k2}\cdots \cdots E_{kk}A_{kn}]$$
		but, $E_{kk} = 1 \implies$$$\gamma_k =[A_{k1} \space A_{k2}\cdots \cdots A_{kn}]$$ which is nothing but the $k^{th}$ row of $A$ itself. Now let us examine the row $\gamma_i$ $$\gamma_i = [\sum^m_{r=1}E_{ir}A_{r1}\sum^m_{r=1}E_{ir}A_{r2} \cdots \cdots \sum^m_{r=1}E_{ir}A_{rn}] = [E_{ii}A_{i1} + E_{ij}A_{j1}, E_{ii}A_{i2} + E_{ij}A_{j2},\cdots \cdots E_{ii}A_{in} + E_{ij}A_{jn}]$$
		but, $E_{ii} = 1, E_{ij}=x\implies$
		$$\gamma_i = [A_{i1} + xA_{j1}, A_{i2} + xA_{j2} \ldots A_{in} + xA_{jn}]$$But this row is nothing but the $j^{th}$ row of $A$ added to the $i^{th}$ row $x$ times. All the other rows remain the same. Thus, we have that this new matrix $EA$ is nothing but a result of the same elementary row operation performed on $A$. 
		I.e., $e(A) = EA$
	3. Interchanging two rows
		Let us switch the rows $i$ and $j$ of $\mathbb1_{m\times m}$. Thus, $\forall k \neq i, k\neq j,$ $E_{kk} = 1,$ and  $\forall l\neq k, E_{kl} = 0$. And for rows $i$ and $j$ we have $E_{ij} = 1,$ and $E_{ji} = 1$. All the other elements of the rows are still $0$. 
		Now let us examine the product $EA$.  
		By the definition of matrix multiplication, each row $\gamma_k$ of their product is given by $$\gamma_k =[\sum^m_{r=1}E_{kr}A_{r1}\sum^m_{r=1}E_{kr}A_{r2} \cdots \cdots \sum^m_{r=1}E_{kr}A_{rn}]$$
		Now for every row $\gamma_k, k\neq i, k\neq j,$ we have $E_{kk}=1$ and $E_{kl} = 0, \forall l\neq k$. Now this also means that for every row $\gamma_k, k\neq i, k\neq j$ 		$$\gamma_k =[E_{kk}A_{k1} \space E_{kk}A_{k2}\cdots \cdots E_{kk}A_{kn}]$$
		but, $E_{kk} = 1 \implies$$$\gamma_k =[A_{k1} \space A_{k2}\cdots \cdots A_{kn}]$$ which is nothing but the $k^{th}$ row of $A$ itself. Now let us examine the row $\gamma_i$ $$\gamma_i = [\sum^m_{r=1}E_{ir}A_{r1}\sum^m_{r=1}E_{ir}A_{r2} \cdots \cdots \sum^m_{r=1}E_{ir}A_{rn}] = [E_{ij}A_{j1}, E_{ij}A_{j2},\cdots \cdots E_{ij}A_{jn}$$
		And we also have that $E_{ij} = 1$		$$\gamma_i = [A_{j1} , A_{j2},\ldots A_{jn}]$$
		Similarly, for the row $\gamma_j$ $$\gamma_j = [\sum^m_{r=1}E_{jr}A_{r1}\sum^m_{r=1}E_{jr}A_{r2} \cdots \cdots \sum^m_{r=1}E_{jr}A_{rn}] = [E_{ji}A_{i1}, E_{ji}A_{i2},\cdots \cdots E_{ji}A_{in}$$
		And we also have that $E_{ji} = 1\implies$$$\gamma_j = [A_{i1} , A_{i2},\ldots A_{in}]$$
		Which means that the product $EA$ is nothing but $A,$ but with the $i^{th}$ and $j^{th}$ rows interchanged.
	$\therefore$ we conclude that 
	$EA = e(\mathbb1_{m×m})A = e(A), \forall$ matrices $A_{m\times n},$ because for each of the three types of elementary row operations, the same applies.
	$Q.E.D.$
	
3. If $A$ is an $n\times n$ matrix, prove that the following statements are equivalent:
	1. $A$ is invertible.
	2. $A$ is row-equivalent to the $n\times n$ identity matrix $\mathbb1_{n\times n}$ 
	3. $A$ is a product of elementary matrices.
	1. Let us assume that $A$ is invertible.
		This means $\exists$ a matrix $A^{-1}$ such that $A^{-1}\cdot A=A\cdot A^{-1}=\mathbb 1_{n\times n}$ 
		However, we also have that every matrix also has a row reduced echelon form.
		Let us say we perform some operations on $A$ to get its row reduced echelon matrix form. 
		This means that $\exists$ some series of elementary row operations we can use 
		
		
	2. Let us assume that $A$ is row-equivalent to the $n\times n$ identity matrix $\mathbb1_{n\times n}$ 
		Since $A$ is row-equivalent to the $n\times n$ identity matrix, it follows that by definition, there is a sequence of elementary row operations, which, if performed on $A,$ give $\mathbb1_{n\times n}$. Let us say that we need some $k$ elementary row operations for this. Then, necessarily, $\exists e_1, e_2, \ldots, e_k$ such that
		$e_k(\ldots e_2(e_1(A))) = \mathbb 1_{n\times n}$. 
		We also have that each matrix obtained from a single elementary row operation on some matrix $A$ can be expressed as the product of an elementary matrix and the matrix $A$. 
		$\implies$ $e_k(\ldots e_2(E_1A)) = \mathbb 1$
		$\implies e_k(\ldots E_2E_1A) = \mathbb1$
		$\implies E_k\ldots E_2E_1A = \mathbb 1$
		Thus, since each single elementary row operation can be expressed as the product of an elementary matrix and that matrix, it thus concludes that $A$ is also a product of elementary operations.
		since each elementary row operation has an inverse, so does its corresponding elementary matrix.
		
		
	3. Let us assume that $A$ is a product of elementary matrices.
		Because it is the product of elementary matrices, it can be expressed thus.
		$E_k\ldots E_2E_1A = \mathbb 1$ 
		Also, since all elementary matrices are square matrices, all of them are $n\times n$ matrices. Since their dimensions are all identical, it means that there exists a well defined product for each of them, which is associative. Thus, $\exists$ some matrix $E= E_k\ldots E_2E_1$. Thus we have that $EA=\mathbb 1 _ {n\times n}$. This means that $\exists$ a matrix $A^{-1}$ such that $A^{-1}A=\mathbb1$. I.e., $E=A^{-1}$ is the left inverse of $A$. But any square matrix which has a left inverse must also have a right inverse and must both be equal and hence $A$ must be invertible.
1. Let $A$ be a $n\times n$ matrix and $B$ be a $n\times 1$ vector with real entries. Consider the equation $AX = B$ $(X$ belongs to $R^m)$ which admits a unique solution. Then which of the following can we conclude?
	1. $m\geq n$
	2. $m\leq n$
	3. $m=n$ 
	4. $m>n$
	We can conclude that $m\leq n$ 
5. 




However, we also have that for every elementary row operation $e, \exists$ another elementary row operation $e^{-1}$ of the same type as $e,$ and performing the inverse operation on the matrix results in the original matrix. This means that we can perform the inverse of the same elementary row operations on both sides. We also have that performing a single elementary row operation on the identity matrix
		I.e.
		$$e_1^{-1}(e_2^{-1}(\dots e_k^{-1}(e_k(\ldots e_2(e_1(A)))))) = e_1^{-1}(e_2^{-1}(\dots e_k^{-1}(\mathbb1)))$$ $\downarrow$
		$$e_1^{-1}(e_2^{-1}(\dots e_{k-1}(\ldots e_2(e_1(A))))) = e_1^{-1}(e_2^{-1}(\dots (\mathbb1 \cdot E_k)))$$
		let us evaluate these expressions.


To prove that $e(A) = EA$ holds for all matrices $A$ of size $m \times n$, where $e$ is an elementary row operation and $E$ is an elementary matrix of size $m \times m$ such that $E = e(\mathbb{1}_{m \times m})$, let's break down the proof.

First, recall the definition of an elementary matrix. An elementary matrix is obtained from the identity matrix $\mathbb{1}_{m \times m}$ by performing a single elementary row operation.

Now, let's consider the product $EA$:

$EA = e(\mathbb{1}_{m \times m})A$

Since $e$ is an elementary row operation, we can express it as a product of elementary matrices. Let $E_1, E_2, \ldots, E_k$ be the elementary matrices corresponding to the sequence of elementary row operations that define $e$. Then, $e$ can be written as:

$e = E_k E_{k-1} \ldots E_2 E_1$

Now, let's express $e(\mathbb{1}_{m \times m})$ in terms of elementary matrices:

$E = e(\mathbb{1}_{m \times m}) = E_k E_{k-1} \ldots E_2 E_1$ 

Substituting this into the expression for $EA$, we get:

 $EA = E_k E_{k-1} \ldots E_2 E_1 A$ 

Now, let's consider the product $e(A)$. Since $e$ is an elementary row operation, $e(A)$ is obtained by applying the same sequence of elementary row operations to $A$. This means that $e(A)$ can also be expressed as a product of elementary matrices:

$e(A) = E_k E_{k-1} \ldots E_2 E_1 A$ 

Comparing the expressions for $EA$ and $e(A)$, we see that they are the same. Therefore, we have shown that $e(A) = EA$ holds for all matrices $A$ of size $m \times n$.