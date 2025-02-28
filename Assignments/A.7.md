
**Rank Nullity Theorem**  Assignment
If $V$ is a finite dimensional vector space over $F$,$$dim (V) = rank(T) + nullity(T) = dim(im(T)) + dim (ker(T))$$

Let us first define some linear transformation $T:V\rightarrow W$.
Let $N$ be a null space of $T$.
$\implies N$ is a subspace of $V$
$\forall\vec v\in N, T(\vec v) = \vec 0_W$

 $dim(N) = nullity (T) = k$
 and let
 $K=\{\vec \alpha_1, \vec \alpha_2, \ldots, \vec \alpha_k\}$ be a basis of $N$ 

Now, $K$ is linearly independent, and it is a subset of $V$. 
This means we can extend it to form a basis of $V$.
Let $dim(V) = n$ and $B = \{\vec \alpha_1, \vec \alpha_2,\ldots \vec \alpha_k, \vec \alpha_{k+1}, \ldots, \vec \alpha_n\}$ be a basis of $V$.

Now, $\{T(\vec \alpha_1), T(\vec \alpha_2), \ldots, T(\vec \alpha_k), T(\vec \alpha_{k+1}), \ldots, T(\vec \alpha_n)\}$
are all in the range of $T = im(T),$ which is some subspace of $W$.
We need to prove that $\{T(\vec \alpha_{k+1}), T(\vec \alpha_{k+2}), \ldots, T(\vec \alpha_n)\}$ forms a basis for $im(T).$

Let $\vec\beta\in im(T)$. 
$\implies\exists \vec\alpha\in V$ such that $\vec\beta = T(\vec\alpha)$
$\implies\exists c_1, c_2, \ldots, c_n$ such that $\vec\alpha = c_1\vec \alpha_1 + c_2\vec \alpha_2 + \ldots + c_n\vec \alpha_n$ 
because $B$ is a basis for $V$.
$\implies\vec\beta = T(\vec\alpha) = T(c_1\vec \alpha_1 + c_2\vec \alpha_2 + \ldots + c_n\vec \alpha_n)$
Also, $T$ is a linear transformation
$\implies T(\vec\gamma + \vec\delta) = T(\vec\gamma) + T(\vec\delta)$ 
So, $$\vec\beta = T(c_1\vec \alpha_1) + T(c_2\vec \alpha_2) + \ldots + T(c_n\vec \alpha_n)$$
but also, $T(x\vec\gamma) = xT(\vec\gamma)$
$$\vec\beta = c_1T(\vec\alpha_1) + c_2T(\vec\alpha_2) +\ldots c_kT(\vec\alpha_k) + c_{k+1}T(\vec\alpha_{k+1})+\ldots c_nT(\vec\alpha_n)$$
But we also have that $\forall\vec v\in N, T(\vec v) = \vec 0_W \implies T(\vec\alpha_i) = \vec0_W \forall 1\leq i\leq k$ 
Now, substituting this in the equation,
$$\vec\beta = c_1\vec0_W + c_2\vec0_W +\ldots c_k\vec0_W + c_{k+1}T(\vec\alpha_{k+1})+\ldots c_nT(\vec\alpha_n)$$
$\vec\beta = c_{k+1}T(\vec\alpha_{k+1})+\ldots c_nT(\vec\alpha_n)$
$\implies$ any vector $\vec\beta \in im(T)$ can be expressed as a linear combination of the vectors $T(\vec\alpha_{k+1}), \ldots, T(\vec\alpha_n) \in im(T).$
Thus, these vectors form a basis for $im(T).$
$\implies$ $dim(im(T)) = n - k = rank(T)$
and we already had
$dim(ker(T)) = k = nullity(T)$
Thus,
$$dim(V) = n = (n-k)+(k) = rank(T) + nullity(T) = dim(im(T)) + dim(ker(T))$$

$Q.E.D$






**Thm**  Assignment
Let $V$ and $W$ be two vector spaces over $F$.
$dim(V) = n$
$dim(W) = m$
Prove without using matrix notation that $$dim(\mathcal L(V,W)) = mn$$





