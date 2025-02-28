**Theorem** **Assignment** **Alternate Definition**
A non-empty subset $W⊂V$ is a subspace $\iff$ for each pair of vectors $\overline\alpha, \overline\beta \in W,$ and for each scalar $c\in F,$ the vector $c\cdot\overline\alpha + \overline\beta \in W$.

**Proof**
1. trivially, if $W$ is a subspace of $V,$
$\overline\alpha\in W, c\in F \implies c\cdot\overline\alpha \in W$     $\because$ $W$ is closed under scalar multiplication
$c\cdot\overline\alpha, \overline\beta\in W \implies c\cdot\overline\alpha + \overline\beta \in W$     $\because$ $W$ is closed under vector addition
Therefore, if $W⊂V$ is a subspace of $V$, it also follows that for each pair of vectors $\overline\alpha, \overline\beta \in W,$ and for each scalar $c\in F,$ the vector $c\cdot\overline\alpha + \overline\beta \in W$.
2. we have that for each pair of vectors $\overline\alpha, \overline\beta \in W,$ and for each scalar $c\in F,$ the vector $c\cdot\overline\alpha + \overline\beta \in W$.
Now, we must prove that $W$ is a subspace of $V$


1. There is a field $F$
2. There is a set of object $W$
3. Vector Addition
	1. let us take some $\overline x_1, \overline x_2 \in W$ such that $\overline x_1 = c_1\overline\alpha_1 + \overline\beta_1$ and $\overline x_2 = c_2\overline\alpha_2 + \overline\beta_2$. As per the definition of vector addition, $\overline x_1 + \overline x_2 =  c_1\overline\alpha_1 + (\overline\beta_1 + c_2\overline\alpha_2 + \overline\beta_2)$ where $\overline\beta_1 + c_2\overline\alpha_2 + \overline\beta_2$ is also a vector closed under $V$ which implies that $\forall \overline x_1, \overline x_2 \in W,$ we also have $\overline x_1+ \overline x_2 \in W$. Thus vector addition is closed under $W$.
	2. The Identity of Addition $\overline 0$ can be expressed as $\overline 0 = 0\cdot\overline0 + \overline 0$ and thus $\overline 0\in W$
	3. Because the property of commutativity, associativity, and identity of vector addition applies for all vectors in $V,$ the property of commutativity also holds for all vectors in $W,$ because all the vectors in $W$ also are vectors in $V$ because $W\subset V$  
	4. We already know that $\forall \overline x \in W, \exists (-\overline x)\in V$ such that $\overline x+(-\overline x)  = \overline 0$. Let $\overline x = c\overline\alpha + \overline\beta$. now, $-\overline x = (-1)\cdot\overline x = -c\overline\alpha +(-\overline\beta)$ and thus we also have $-\overline x \in W$. 
4. Scalar Multiplication
	1. let us take some $\overline x\in W$ and some $d\in F$. We have that $\overline x = c\overline \alpha +\overline \beta$ $\implies d\overline x = d(c\overline \alpha +\overline \beta)\implies d\overline x = cd\overline\alpha + d\overline \beta\implies d\overline x \in W$  because $cd\in F$ and $\overline\alpha, d\overline\beta\in V$  Thus, $W$ is closed under scalar multiplication.
	2. The identity of scalar multiplication is $1\in F$ and thus it also applies for $W$ if it applies for $V$ because $1\overline \alpha =\overline \alpha,$  $\forall \overline\alpha\in V$ and hence because $W\subset V$ it also applies for all $\overline \alpha \in W$ 
	3. Similarly, the following also apply for all $\overline \alpha \in W$ because $W\subset V$ and they apply $\forall \overline\alpha \in V$ 
		1. $c_1(c_2\overline\alpha) = (c_1c_2)\overline\alpha$ 
		2. $c(\overline\alpha+\overline\beta) = c\overline\alpha + c\overline\beta$ 
		3. $(c_1+c_2)\overline\alpha = c_1\overline\alpha + c_2\overline\alpha$ 
And thus, since the set $W\subset V$ observes all of the rules for a vector space, it must also  






1. On $\mathbb R^n$ define $\overline\alpha\oplus\overline\beta=\overline\alpha-\overline\beta$ and $c\overline\alpha=-c\overline\alpha$. Which of the axioms for the vector space are satisfied by $(\mathbb R^n,\mathbb R, \oplus, \cdot)$?
2. Let $V$ be the set of all complex valued functions $f$ on the real line such that $\forall t \in \mathbb R,$    $f(-t) = f((t))* = f*(t)$  where $f*(t)$ denotes the complex conjugation of $f(t)$.
	1. Show that $V$ with the operations $(f+g)(t) = f(t)+g(t)$ and $(cf)(t)=cf(t)$ is a vector space over the field $\mathbb R$
	2. Give an example of a function $f_n\in V$ which is not real valued.
3. A non-empty subset $W$ of a vector space $V$ is a subspace of $V$ if and only if, for each pair of vectors $\overline\alpha, \overline\beta \in W,$ and for each scalar $c\in F,$ the vector $c\cdot\overline\alpha + \overline\beta \in W$.








4. A vector space must possess the following properties as per the definition of a vector space

A *vector space* $V$ consists of the following.
1. A field $F$ of scalars.
2. A set of objects called *vectors*.
3. A rule (a binary operation) called *vector addition* which associates with each pair of vectors $\overline\alpha,\overline\beta\in V$ a vector $(\overline\alpha + \overline\beta)\in V$, called the *sum* of $\overline\alpha$ and $\overline\beta$ such that
	1. addition is commutative
		1. $\overline\alpha + \overline\beta = \overline\beta+\overline\alpha,$    $\forall \overline\alpha, \overline\beta\in V$
	2. addition is associative
		1. $(\overline\alpha + \overline\beta )+ \overline\gamma = \overline\alpha+(\overline\beta + \overline\gamma),$    $\forall \overline\alpha, \overline\beta, \overline\gamma \in V$
	3. $\exists$ a unique vector $\overline0$ called the *zero vector*, such that $\overline\alpha + \overline0 = \overline\alpha,$     $\forall \overline\alpha\in V$  
	4. for each $\overline\alpha \in V,$   $\exists$ a unique $-\overline\alpha\in V$ such that $\overline\alpha + (-\overline\alpha) = \overline0$  
4. A rule (a binary operation) called scalar multiplication which associates with each scalar $c\in F$ and vector $\overline\alpha \in V$ a vector $c\overline\alpha\in V$ called the product of $c$ and $\overline\alpha$ such that
	1. $1\overline\alpha = \alpha$                         also $\implies-\overline\alpha = (-1)\overline\alpha$
	2. $(c_1c_2)\overline\alpha = c_1(c_2\overline\alpha)$
	3. $c(\overline\alpha+\overline\beta) = c\overline\alpha + c\overline\beta$
	4. $(c_1 + c_2)\overline\alpha = c_1\overline\alpha + c_2\overline\alpha$

A vector space $V$ is defined over a field $F$ and has two operations, vector addition and scalar multiplication. These conditions are necessary and sufficient for the definition of a vector space.


Now let us individually examine each of these.
1. The vector space has a field of scalars: $\mathbb R$  
2. The vector space has a set of vectors: $\mathbb R^n$
3. It has a rule called vector addition given by $\overline\alpha\oplus\overline\beta=\overline\alpha-\overline\beta$.
	1. Is it commutative?
		1. Take some $\overline\alpha,\overline\beta\in\mathbb R^n$ 
		2. $\overline\alpha\oplus\overline\beta = \overline\alpha - \overline\beta$ and $\overline\beta\oplus\overline\alpha = \overline\beta - \overline\alpha$
		3. $\overline\alpha - \overline\beta\neq\overline\beta - \overline\alpha\implies$ Vector addition is not commutative.
	2. Is it associative?
		1. Take some $\overline\alpha,\overline\beta, \overline\gamma\in\mathbb R^n$ 
		2. $\overline\alpha\oplus(\overline\beta \oplus\overline\gamma) = \overline\alpha - (\overline\beta\oplus\overline\gamma) = \overline\alpha - (\overline\beta-\overline\gamma) = \overline\alpha - \overline\beta+\overline\gamma$ and $(\overline\alpha\oplus\overline\beta )\oplus\overline\gamma = (\overline\alpha \oplus\overline\beta)-\overline\gamma = (\overline\alpha - \overline\beta)-\overline\gamma = \overline\alpha - \overline\beta-\overline\gamma$
		3. $\overline\alpha\oplus(\overline\beta \oplus\overline\gamma)\neq(\overline\alpha\oplus\overline\beta) \oplus\overline\gamma\implies$ Vector addition is not associative.
	4. Does it have a unique $\overline0$?
		1. Take some $\overline\alpha\in\mathbb R$
		2. $\overline\alpha \oplus \overline0 = \overline\alpha - \overline0 = \overline\alpha$
		3. Thus $\exists\overline0\in \mathbb R$
	5. Does it have a unique $-\overline \alpha$?
		1. Take some $\overline\alpha\in\mathbb R$
		2. $\overline\alpha\oplus(\overline\alpha) =\overline\alpha-\overline\alpha= \overline 0$ 
		3. Every vector is its own additive inverse.
4. It has a rule called scalar multiplication given by
5. $c\cdot\overline\alpha=-c\overline\alpha$
	1. and thus let us verify the properties of scalar multiplication
	2. $1\cdot \overline\alpha = -\overline\alpha\neq\overline\alpha$ thus it does not have an identity of scalar multiplication
	3. $(c_1c_2)\cdot\overline\alpha\neq c_1(c_2\cdot\overline\alpha)$
		1. $(c_1c_2)\cdot\overline\alpha = -c_1c_2\overline\alpha$
		2. $c_1(c_2\cdot\overline\alpha) = c_1(-c_2\overline\alpha) = (-c_1)(-c_2)\overline\alpha = c_1c_2\overline\alpha$
	4. $(c_1+c_2)\cdot\overline\alpha =c_1\cdot\overline\alpha+c_2\cdot\overline\alpha$  
		1. $(c_1+c_2)\cdot\overline\alpha = -(c_1+c_2)\overline\alpha$
		2. $c_1\cdot\overline\alpha+c_2\cdot\overline\alpha = -c_1\overline\alpha-c_2\overline\alpha = -(c_1+c_2)\overline\alpha$ 
	5. $c\cdot(\overline\alpha\oplus\overline\beta)=c\cdot\overline\alpha\oplus c\cdot\overline\beta$ 
		1. $c\cdot(\overline\alpha\oplus\overline\beta) = -c(\overline\alpha-\overline\beta) = -c\overline\alpha+c\overline\beta$ 
		2. $c\cdot\overline\alpha\oplus c\cdot\overline\beta = -c\overline\alpha-(-c\overline\beta) = -c\overline\alpha+c\overline\beta$ 

Thus it holds the following axioms of vector spaces:
1. It has a field of scalars $\mathbb R$
2. It has a set of vectors $\mathbb R^n$ 
3. It has a unique additive identity and inverse for vector addition. 
4. Scalar multiplication is distributive over vector addition and scalar addition.




Let $V$ be the set of all complex valued functions $f$ on the real line such that $\forall t \in \mathbb R,$    $f(-t) = f((t))* = f*(t)$  where $f*(t)$ denotes the complex conjugation of $f(t)$.
	1. Show that $V$ with the operations $(f+g)(t) = f(t)+g(t)$ and $(cf)(t)=cf(t)$ is a vector space over the field $\mathbb R$
	2. Give an example of a function $f_n\in V$ which is not real valued.

consider the properties of vector addition:
1. Let us see if it is closed
   $(f+g)(t)=f(t)+f(t)$
   now consider 
   $f(t) = x_1+iy_1$ and $g(t)=x_2 + iy_2$
    
   



1. It has a field of scalars $\mathbb R$
2. It has a set of objects (functions). Let us call this set $V$ and define it thus:$$V=\{f:\mathbb R \rightarrow \mathbb C\}$$
3. Let us verify the properties of vector addition
	1. Closure
	   Take some $f,g\in V$. We have that $f(t), g(t)\in \mathbb C,\forall t\in\mathbb  R$ .
	   $\implies (f+g)(t) = f(t)+g(t)\in\mathbb C\implies (f+g)(t)\in\mathbb C$  because of the closure of $\mathbb C$ under addition.
	2. Commutativity
	   Take some $f,g\in V$. We have that $(f+g)(t)=f(t)+g(t)=g(t)+f(t)=(g+f)(t)$ because of the commutativity of addition in $\mathbb C,$ and $f(t), g(t)\in \mathbb C$.
	3. Associativity
	   Take some $f,g,h\in V$. We have that $((f+g)+h)(t)=(f(t)+g(t))+h(t)=f(t)+(g(t)+h(t))=(f+(g+h))(t)$ because of the property of associativity of addition in $\mathbb C$ and all of the functions are complex valued. 
	4. Identity
	   We have the zero-function $z\in V$ such that $z(t)=0,\forall t\in \mathbb R$. Thus we have that $\forall f\in V,t\in \mathbb R$   $(f+z)(t) = f(t)+z(t)=f(t)+0=f(t)=(z+f)(t)$ because  the identity of addition in $\mathbb C=0$ and all of the functions are complex valued.
	5. Inverse
	   $f\in V$. $\forall f\in V,$ we have $\exists-f\in V$ such that $(-f)(t)=-(f(t))$ where $-(f(t))$ is the additive inverse of $f(t)$ which exists because all the functions are complex valued and there exists a unique additive inverse for all the elements in $\mathbb C$.
	   $\therefore, f(t)+(-f)(t)= f(t)+(-f(t)) = 0$ 
   And thus we see that $V$ obeys all the properties of vector addition.
4. Let us verify the properties of scalar multiplication 
	1. $(1\cdot f)(t)= 1\cdot(f(t))=f(t)$ because $f(t)$ is always a complex number, and $1$ is the identity of multiplication in $\mathbb C.$
	2. $(c_1(c_2\cdot f))(t) = c_1(c_2f(t)) = (c_1c_2)(f(t)) = ((c_1c_2)f)(t)$ because $c_1, c_2, f(t)\in \mathbb C$ and multiplication is associative in $\mathbb C$ 
	3. $(c(f+g))(t)=c((f+g)(t))=c(f(t)+g(t))=c(f(t))+c(g(t))=(cf)(t)+(cg)(t)$ because $c, (f+g)(t), f(t),g(t)\in \mathbb C$ and multiplication is distributive over addition in $\mathbb C$.
	4. $((c_1+c_2)f)(t)= (c_1+c_2)(f(t))=c_1(f(t))+c_2(f(t))=(c_1f)(t)+c_2f(t)$ because $c_1, c_2, f(t)\in \mathbb C$ and multiplication is distributive over addition in $\mathbb C.$ 
   And thus we see that $V$ obeys all the properties of scalar multiplication. 

And since $V$ obeys all the properties defined for a vector space, we see that $V$ is in fact and in deed, in its own right, a vector space.