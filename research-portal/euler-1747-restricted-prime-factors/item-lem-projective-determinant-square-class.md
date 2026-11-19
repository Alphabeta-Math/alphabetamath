---
title: Determinant square class of a projective matrix
status: published
research_item: lem-projective-determinant-square-class
dependency_level: 1
---

## Prerequisites

- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group)
- [math:thm-quotient-group-laws](https://alphabetamath.cc/item/thm-quotient-group-laws)
- [math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)
- [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)
- [math:prop-legendre-symbol-on-units-is-homomorphism](https://alphabetamath.cc/item/prop-legendre-symbol-on-units-is-homomorphism)
- [math:lem-ring-elementary-consequences](https://alphabetamath.cc/item/lem-ring-elementary-consequences)


## Statement

Let $F$ be a field, let $F^\times$ be its multiplicative group of nonzero elements, and put $H=(F^\times)^2=\{u^2:u\in F^\times\}$. The square class of $t\in F^\times$ is the coset $tH=\{th:h\in H\}$. The group $\mathrm{PGL}_2(F)$ consists of invertible two-by-two matrices over $F$ up to multiplication by nonzero scalars. Write $[A]$ for the class represented by $A$.

The determinant induces a surjective group homomorphism
$$D_F:\mathrm{PGL}_2(F)\longrightarrow F^\times/H,\qquad D_F([A])=(\det A)H.$$
Here a group homomorphism preserves products, and surjective means every element of the target occurs as a value.

For the sign character, take a prime $p$, meaning an integer greater than one whose only positive divisors are $1$ and $p$. Assume $p$ is odd, meaning $2\nmid p$. Thus there is no integer $q$ with $p=2q$. Let $\mathbb F_p=\mathbb Z/p\mathbb Z$ be the field of integer residue classes modulo $p$, so integers represent the same class exactly when their difference is divisible by $p$. Write $[a]_p$ for the class of $a$. Addition and multiplication are given by $[a]_p+[b]_p=[a+b]_p$ and $[a]_p[b]_p=[ab]_p$. On $\mathbb F_p^\times$ the Legendre symbol has value $1$ on squares and $-1$ on all other elements. It induces a map $\overline{\lambda}_p$ on $F^\times/H$ for $F=\mathbb F_p$. The composite $\overline{\lambda}_p\circ D_{\mathbb F_p}$ is a nontrivial sign character, meaning a homomorphism to the multiplicative group of integer signs $\{1,-1\}$ that takes the value $-1$. Its value at $[A]$ is the Legendre symbol of $\det A$.

## Statement references

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-congruence-modulo-an-integer](https://alphabetamath.cc/item/def-congruence-modulo-an-integer)

## Facts & Assumptions

[F1] A field is a commutative ring with $0\ne 1$ and with its nonzero elements forming a group under multiplication ([math:def-field](https://alphabetamath.cc/item/def-field) and [math:lem-field-is-a-commutative-ring](https://alphabetamath.cc/item/lem-field-is-a-commutative-ring)). Multiplying by zero in this ring gives zero ([math:lem-ring-elementary-consequences](https://alphabetamath.cc/item/lem-ring-elementary-consequences)).

[F2] Write $\mathrm{GL}_2(F)$ for the group of invertible two-by-two matrices over $F$ under matrix multiplication. In the degree-two projective linear group, the representatives of $[A]$ are the matrices $uA=(uI)A$ for $u\in F^\times$. The matrix $uA$ has entries obtained by multiplying those of $A$ by $u$, and $I$ is the identity matrix with ones on the diagonal and zeros elsewhere. The product is $[A][B]=[AB]$. An invertible matrix $A$ has a two-sided inverse $A^{-1}$, with $AA^{-1}=A^{-1}A=I$. Matrix multiplication uses $(AB)_{ij}=a_{i1}b_{1j}+a_{i2}b_{2j}$ ([def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)).

[F3] For $A=\begin{pmatrix}a&b\\c&d\end{pmatrix}$ the two terms of the determinant formula give $\det A=ad-bc$ ([math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)). For square matrices of the same size over a commutative ring, $\det(AB)=\det(A)\det(B)$ ([math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)).

[F4] A subgroup contains the identity and is closed under products and inverses ([math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)). A subgroup $N$ of a group $G$ is normal if $gNg^{-1}=N$ for all $g\in G$ ([math:def-normal-subgroup](https://alphabetamath.cc/item/def-normal-subgroup)). Its left cosets are the sets $gN=\{gn:n\in N\}$ ([math:def-coset](https://alphabetamath.cc/item/def-coset)). For normal $N$, the quotient group $G/N$ consists of these cosets with product $(gN)(kN)=(gk)N$ ([math:def-quotient-group](https://alphabetamath.cc/item/def-quotient-group) and [math:thm-quotient-group-laws](https://alphabetamath.cc/item/thm-quotient-group-laws)). A map of groups is a homomorphism if it preserves products ([math:def-group-homomorphism](https://alphabetamath.cc/item/def-group-homomorphism)).

[F5] Every element of $\mathbb Z/p\mathbb Z$ is the residue class of some integer ([math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)). On residue classes, addition and multiplication are given by $[a]_p+[b]_p=[a+b]_p$ and $[a]_p[b]_p=[ab]_p$ ([math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)). For a prime $p$, the residue ring $\mathbb Z/p\mathbb Z$ with these operations is a field ([math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)). For a prime $p$ with $2\nmid p$ (an odd prime, using [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)), the Legendre symbol $\lambda_p$ on its nonzero classes assigns $1$ to squares and $-1$ to nonsquares ([math:def-legendre-symbol](https://alphabetamath.cc/item/def-legendre-symbol)). On the group of nonzero classes, this rule is well defined on residue classes and is a surjective group homomorphism to $\{1,-1\}$ ([math:prop-legendre-symbol-on-units-is-homomorphism](https://alphabetamath.cc/item/prop-legendre-symbol-on-units-is-homomorphism)).

## Proof

**Given:** A field $F$ and, for the sign character, a prime $p$ with $2\nmid p$ and $F=\mathbb F_p$.

**Goal:** Prove the determinant square-class formula defines a surjective group homomorphism and that its composite with the induced Legendre sign takes both signs.

1.1 The element $1=1^2$ belongs to $H$. For $u,v\in F^\times$, commutativity gives $u^2v^2=(uv)^2$, and $(u^2)^{-1}=(u^{-1})^2$ since $u^2(u^{-1})^2=(uu^{-1})^2=1$. Thus $H$ is a subgroup. Each $g\in F^\times$ commutes with every $h\in H$, so $ghg^{-1}=h$, which gives $gHg^{-1}=H$. Hence the cosets of $H$ form the quotient group $F^\times/H$ with the stated product. [F1, F4]

2.1 The two-by-two determinant formula gives $\det I=1$. For any $A\in\mathrm{GL}_2(F)$, multiplicativity gives $\det(A)\det(A^{-1})=\det I=1$, so $\det A\in F^\times$. If $[A']=[A]$, then $A'=(uI)A$ for some $u\in F^\times$. The same determinant formula gives $\det(uI)=u^2$, so $\det A'=u^2\det A$. Since $u^2\in H$, multiplication by $u^2$ carries $H$ onto itself with inverse multiplication by $(u^2)^{-1}\in H$. By commutativity, $(\det A')H=(\det A)(u^2H)=(\det A)H$. This proves independence of the choice of matrix representative. [F1, F2, F3, F4, step 1.1]

2.2 In the specialization $F=\mathbb F_p$ with $p$ prime and $2\nmid p$, the odd-prime hypothesis in [F5] holds. The units of this field are exactly the nonzero elements by [F1]. For $t\in F^\times$ and $h\in H$, take $u\in F^\times$ with $h=u^2$. Using the integer representatives from [F5], write $t=[a]_p$ and $u=[b]_p$. The modular product in [F5] gives $h=[b^2]_p$ and $th=[ab^2]_p$. Then $\lambda_p(th)=\lambda_p(t)\lambda_p(h)=\lambda_p(t)$ because $h$ is a nonzero square. Thus the formula $\overline{\lambda}_p(tH)=\lambda_p(t)$ gives a single sign for the entire coset. The quotient product and multiplicativity of $\lambda_p$ give $\overline{\lambda}_p((tH)(sH))=\lambda_p(ts)=\overline{\lambda}_p(tH)\overline{\lambda}_p(sH)$. Each sign occurs on a coset because it occurs on some $t\in F^\times$ by [F5]. [F1, F4, F5, step 1.1]

3.1 For any field $F$ and invertible $A,B$, $D_F([A][B])=(\det(AB))H=(\det(A)\det(B))H=D_F([A])D_F([B])$, using the two quotient products and determinant multiplicativity. Hence $D_F$ is a group homomorphism. [F2, F3, F4, step 1.1, step 2.1]

3.2 For any target coset $tH$, take $A=\begin{pmatrix}t&0\\0&1\end{pmatrix}$. Set $B=\begin{pmatrix}t^{-1}&0\\0&1\end{pmatrix}$. The matrix product formula gives $AB=\begin{pmatrix}tt^{-1}&0\\0&1\end{pmatrix}=I$ and $BA=\begin{pmatrix}t^{-1}t&0\\0&1\end{pmatrix}=I$, since $tt^{-1}=t^{-1}t=1$ and products with zero vanish. Thus $A$ is invertible, and its determinant is $t$. Therefore $D_F([A])=tH$, proving surjectivity. [F1, F2, F3, F4, step 2.1]

4.1 Since both $D_{\mathbb F_p}$ and $\overline{\lambda}_p$ preserve products, their composite preserves products. Each sign is attained by the composite because each sign is the image of a coset under $\overline{\lambda}_p$ and every coset is attained by $D_{\mathbb F_p}$. Thus the composite is nontrivial and its value at $[A]$ is $\overline{\lambda}_p((\det A)H)=\lambda_p(\det A)$, as claimed. [F4, F5, step 2.1, step 3.1, step 3.2, step 2.2] ∎
