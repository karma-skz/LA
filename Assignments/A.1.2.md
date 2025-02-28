**Assignment**
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