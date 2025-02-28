
1. Show that the set of all real $2\times2$ matrices $=M_{2\times2}$ of the form
$$\begin{bmatrix} a&b\\-b&a\end{bmatrix}$$
where $a,b\in\mathbb R$ with the usual matrix operations form a field. 

First let us define the operations of addition and multiplication.

For some $X,Y\in M$ such that
$X=\begin{bmatrix} a &b\\-b&a\end{bmatrix}$ and $Y=\begin{bmatrix} c &d\\-d&c\end{bmatrix}$
let us define
$X+Y=\begin{bmatrix} a +c&b+d\\-b-d&a+c\end{bmatrix}$
and $XY = \begin{bmatrix} ac-bd &ad+bc\\-ad-bc&ac-bd\end{bmatrix}$
let us now examine some properties.

Closure under addition
let us say that $a+c=x$ and $b+d=y$
by the properties of closure of real numbers under addition, $x,y\in\mathbb R$ and $X+Y=\begin{bmatrix} a +c&b+d\\-b-d&a+c\end{bmatrix}=\begin{bmatrix} x&y\\-y&x\end{bmatrix}$ where $x,y\in \mathbb R$ and thus $X, Y\in M \implies X+Y \in M$
thus the set $M$ is closed under addition.
Closure under multiplication
let us say that $x=ac-bd$ and $y= ad+bc$ by the properties of closure of real numbers under addition and multiplication, $x,y\in\mathbb R$  
$XY = \begin{bmatrix} ac-bd &ad+bc\\-ad-bc&ac-bd\end{bmatrix} = \begin{bmatrix} x&y\\-y&x\end{bmatrix}$ where $x,y\in \mathbb R$ and thus $X, Y\in M \implies XY \in M$
thus the set $M$ is closed under multiplication.

Now that we know that the set is closed under addition and multiplication let us consider for any three matrices $X,Y,Z\in M,$ such that $X=\begin{bmatrix} a &b\\-b&a\end{bmatrix},$ $Y=\begin{bmatrix} c &d\\-d&c\end{bmatrix},$ and $Z=\begin{bmatrix} e &f\\-f&e\end{bmatrix}$

Commutativity of addition
$X+Y=\begin{bmatrix} a +c&b+d\\-b-d&a+c\end{bmatrix}$ and $Y+X=\begin{bmatrix} c+a&d+b\\-d-b&c+a\end{bmatrix}$  and because the addition of real numbers is commutative, $X+Y=Y+X\forall X,Y\in M$ thus addition is commutative in this set

Commutativity of Multiplication
$XY=\begin{bmatrix} ac-bd &ad+bc\\-ad-bc&ac-bd\end{bmatrix}$



$\overline\beta = c_1\overline\alpha_1 + c_2\overline\alpha_2 + c_3\overline\alpha_3$
where $\overline\alpha_1 = (1,0,-1), \overline\alpha_2 = (0,1,1), \overline\alpha_3 = (1,1,1),$ and $c_1, c_2, c_3 \in \mathbb C$ 

$\therefore, \overline\beta = (c_1+c_3, c_2+c_3, -c_1+c_2+c_3)$ and $c_1, c_2, c_3 \in \mathbb C$ that is they are any complex numbers.

Thus, let us find the solution to this system.

$\begin{bmatrix}1&0&1\\0&1&1\\-1&1&1\end{bmatrix}$ $\begin{bmatrix} c_1\\c_2\\c_3\end{bmatrix}$ $=$ $\begin{bmatrix} x_1\\x_2\\x_3\end{bmatrix}$ such that $x_1, x_2, x_3\in\mathbb C$ 

we need to find the possible value of $x_1, x_2,$ and $x_3$ 
because $\overline\beta=(x_1,x_2,x_3)$ and thus since, by the properties of closure of complex numbers, any $c_1, c_2, c_3\in\mathbb C,$ it also follows that $x_1, x_2, x_3\in \mathbb C$ and vice versa. (by augmented matrix conversion to $\mathbb 1 _{3\times3}$  the inverse of )
thus the any vector in $\mathbb C^3$ can be expressed as a linear combination of $\overline\alpha_1, \overline\alpha_2, \overline\alpha_3$ 