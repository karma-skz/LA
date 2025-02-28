The subspace spanned by a non-empty subset $S$ of a vector space $V$ is the set of all linear combinations of vectors in $S$.

If $W_1$ and $W_2$ are finite dimensional subspaces of vector space $V,$ then prove that

1. $W_1+W_2$ is finite dimensional
2. *dim*$W_1 +$ *dim*$W_2$ = *dim*$(W_1\cap W_2) +$ *dim*$(W_1+W_2)$

Let $R$ be a non-zero row-reduced echelon matrix, then prove that the non-zero row vectors of $R$ form a basis for the row space of $R$.



1. a
By definition, the subspace $W$ spanned by $S$ is the smallest such subspace which contains $S.$

Now, we must prove two things.
1. $W$ only contains linear combinations of the vectors in $S.$
2. All the linear combinations of the vectors in $S$ are also present in $W.$

The second point is trivial, because since $W$ is a subspace, it contains any linear combination of the vectors in $S,$ because by definition, because it is closed.

Now that we have that all the linear combinations of the vectors in $S$ are also in $W,$ we must prove that there is no other element in $W.$

Let us assume that there is some $\vec a\in W$ which is not a linear combination of the vectors in $S = \{\vec x_1, \vec x_2, \ldots, \vec x_n\}$  
Thus we have that 
$\vec a \neq c_1\vec x_1 + c_2\vec x_2 + \ldots + c_n\vec x_n$    $\forall c_i\in F$ 

4. b
5. c