---
title: Integral splitting of the Hurwitz order at odd primes
status: draft
research_item: thm-hurwitz-integral-splitting-at-odd-primes
dependency_level: 2
sources:
  references:
    - title: "John Voight, Quaternion Algebras, chapter 14: Quaternion algebras over
        global fields"
      url: https://link.springer.com/chapter/10.1007/978-3-030-56694-4_14
      locator: Example 14.2.13(i)
      reading_limits: Read the Hamilton discriminant example in the publisher's text
        for attribution.
    - title: "John Voight, Quaternion Algebras, chapter 15: Discriminants"
      url: https://link.springer.com/chapter/10.1007/978-3-030-56694-4_15
      locator: Lemma 15.5.3 and Example 15.5.7
      reading_limits: Read the split maximal-order case and the identification of the
        maximal Hurwitz order in chapter 15.
    - title: "John Voight, Quaternion Algebras, chapter 12: Ternary quadratic forms
        over local fields"
      url: https://link.springer.com/chapter/10.1007/978-3-030-56694-4_12
      locator: Lemmas 12.2.17 and 12.3.6
      reading_limits: Read the univariate lifting statement and the
        reduction-and-lifting argument for quadratic forms.
---

## Prerequisites

- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)
- [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)
- [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [math:def-field](https://alphabetamath.cc/item/def-field)
- [math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations)
- [math:thm-tensor-product-of-algebras-over-a-commutative-ring](https://alphabetamath.cc/item/thm-tensor-product-of-algebras-over-a-commutative-ring)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)
- [math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)
- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)
- [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)
- [math:thm-ring-matrix-arithmetic-laws](https://alphabetamath.cc/item/thm-ring-matrix-arithmetic-laws)
- [math:prop-canonical-quotient-ring-map](https://alphabetamath.cc/item/prop-canonical-quotient-ring-map)
- [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule)
- [math:thm-the-strong-pigeonhole-principle](https://alphabetamath.cc/item/thm-the-strong-pigeonhole-principle)
- [math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting)
- [math:def-polynomial-ring-over-a-commutative-ring](https://alphabetamath.cc/item/def-polynomial-ring-over-a-commutative-ring)
- [math:def-formal-derivative-of-a-polynomial](https://alphabetamath.cc/item/def-formal-derivative-of-a-polynomial)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)
- [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)
- [math:def-polynomial-evaluation-and-root](https://alphabetamath.cc/item/def-polynomial-evaluation-and-root)


## Statement

Let $\ell>2$ be a prime, so its only positive divisors are $1$ and $\ell$.

Let $B=\mathbb Q+\mathbb Qi+\mathbb Qj+\mathbb Qk$ be the rational Hamilton algebra with basis $1,i,j,k$ and $i^2=j^2=-1$, $ij=k=-ji$. Let $O=\mathbb Z+\mathbb Zi+\mathbb Zj+\mathbb Zw$ be its maximal Hurwitz order, where $w=(-1+i+j+k)/2$. An order is a subring with the same identity, equal to the integer span of finitely many elements and with rational span $B$. Maximality is with respect to inclusion.

Write $K=\mathbb Q_\ell$ for the completion of the rationals in the metric given off the diagonal by $d_\ell(x,y)=\ell^{-v_\ell(x-y)}$, where $v_\ell$ counts the exponent of $\ell$ in the numerator minus that in the denominator. Let $R=\mathbb Z_\ell\subseteq K$ be the ring of compatible residue classes modulo the powers of $\ell$, with arithmetic in each component. Compatibility means that each component reduces to the preceding one. Let $F=\mathbb F_\ell=\mathbb Z/\ell\mathbb Z$ be the field of integer residues modulo $\ell$.

In $B_K=B\otimes_{\mathbb Q}K$ and $O_R=O\otimes_{\mathbb Z}R$, the tensor products extend the original scalars to $K$ and $R$, respectively. The generating symbols $x\otimes s$ are additive in both entries and satisfy $cx\otimes s=x\otimes cs$ for each original scalar $c$. Their multiplication satisfies $(x\otimes s)(y\otimes t)=xy\otimes st$.

For a commutative ring $S$, $M_2(S)$ denotes the algebra of two-by-two matrices with entries in $S$, with entrywise addition, row-by-column multiplication and scalars acting as scalar matrices. An algebra isomorphism is a bijection preserving addition, multiplication, the identity and the scalar action.

There is a $K$-algebra isomorphism $\Phi:B_K\longrightarrow M_2(K)$ carrying the natural image of $O_R$ onto $M_2(R)$. The resulting entrywise reduction induces an $F$-algebra isomorphism $\bar\Phi:O/\ell O\longrightarrow M_2(F)$, where $O/\ell O$ is the ring of cosets modulo the ideal $\ell O=\{\ell x:x\in O\}$. The ideal is an additive subgroup closed under left and right multiplication by elements of $O$. For each $x=x_0+x_1i+x_2j+x_3k\in O$, its integer reduced norm $N(x)=x_0^2+x_1^2+x_2^2+x_3^2$ satisfies $\det\bar\Phi(x+\ell O)=N(x)\bmod\ell$, using $\det\begin{pmatrix}a&b\\c&d\end{pmatrix}=ad-bc$.

## Statement references

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure)

[math:def-subring](https://alphabetamath.cc/item/def-subring)

[math:def-quaternions](https://alphabetamath.cc/item/def-quaternions)

[math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)

[math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)

[math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)

[math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)

[math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)

[math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)

[math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)

[math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[math:def-field](https://alphabetamath.cc/item/def-field)

[math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations)

[math:thm-tensor-product-of-algebras-over-a-commutative-ring](https://alphabetamath.cc/item/thm-tensor-product-of-algebras-over-a-commutative-ring)

[math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)

[math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)

[math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)

[math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)

[math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)

[math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix)

## Facts & Assumptions

[F1] The rational Hamilton multiplication table is given by $i^2=j^2=-1$ and $ij=k=-ji$, with coefficients commuting with $1,i,j,k$. The order $O$ is closed under products and has integer basis $1,i,j,w$. A basis gives a unique linear expansion. Both $1,i,j,k$ and $1,i,j,w$ are rational bases of $B$, and $N(x)$ is integral for $x\in O$. [thm-hurwitz-order-integral-structure](item-thm-hurwitz-order-integral-structure) [math:def-quaternions](https://alphabetamath.cc/item/def-quaternions) [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis) [math:def-subring](https://alphabetamath.cc/item/def-subring)

[F2] Integer residue classes are equal exactly when their representatives differ by a multiple of the modulus. Their sums and products are those of representatives reduced modulo that modulus. For $R$ these operations are taken componentwise. The completion field $K$ contains $\mathbb Q$ and is canonically the fraction field of $R$, with the integer $n$ mapping to its compatible residue classes in $R$. [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers) [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q) [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals) [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field) [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes) [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n) [math:thm-integers-modulo-n-basic-algebra](https://alphabetamath.cc/item/thm-integers-modulo-n-basic-algebra) [math:def-addition-and-multiplication-modulo-n](https://alphabetamath.cc/item/def-addition-and-multiplication-modulo-n)

[F3] Modulo a prime the residue ring is a field, a commutative ring in which $0\ne 1$ and each nonzero element is invertible. Integer arithmetic is ordered ring arithmetic, and division by a positive integer $d$ gives a unique remainder in $\{0,\ldots,d-1\}$. [math:def-prime](https://alphabetamath.cc/item/def-prime) [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field) [math:def-field](https://alphabetamath.cc/item/def-field) [math:thm-int-ordered-ring](https://alphabetamath.cc/item/thm-int-ordered-ring) [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[F4] The number of elements of a finite set is the length of an enumeration without repetitions. A product of two finite sets has size the product of their sizes. A function from a larger finite set to a smaller one has two distinct inputs with the same value. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:thm-product-rule](https://alphabetamath.cc/item/thm-product-rule) [math:thm-the-strong-pigeonhole-principle](https://alphabetamath.cc/item/thm-the-strong-pigeonhole-principle)

[F5] If $f\in R[X]$ and $t\in R$ satisfy $f(t)\in\ell R$ and $f'(t)\notin\ell R$, Hensel's simple-root lifting theorem gives $a\in R$ with $f(a)=0$ and $a-t\in\ell R$. Here $R[X]$ consists of finite sums of powers of the formal variable $X$ with coefficients in $R$. The formal derivative sends $cX^n$ to $ncX^{n-1}$ for $n>0$, sends constants to zero and acts termwise. For $t\in R$, evaluation sends $\sum_i c_iX^i$ to $\sum_i c_it^i$ in $R$ using the identity coefficient map. [math:cor-p-adic-simple-root-lifting](https://alphabetamath.cc/item/cor-p-adic-simple-root-lifting) [math:def-polynomial-ring-over-a-commutative-ring](https://alphabetamath.cc/item/def-polynomial-ring-over-a-commutative-ring) [math:def-formal-derivative-of-a-polynomial](https://alphabetamath.cc/item/def-formal-derivative-of-a-polynomial) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring) [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism) [math:def-polynomial-evaluation-and-root](https://alphabetamath.cc/item/def-polynomial-evaluation-and-root)

[F6] Every tensor is a sum of elementary tensors, subject to the additive and balancing relations in the Statement. For algebras over the commutative base ring, products are taken factor by factor and $1\otimes1$ is the identity. The second tensor factor supplies the extended scalars. [math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations) [math:thm-tensor-product-of-algebras-over-a-commutative-ring](https://alphabetamath.cc/item/thm-tensor-product-of-algebras-over-a-commutative-ring) [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring) [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)

[F7] Row-by-column multiplication is associative, unital and distributes over addition on both sides. Scalar matrices commute with every matrix and multiply each entry by the scalar. The determinant of a two-by-two matrix is its diagonal product minus its off-diagonal product. [math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring) [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose) [math:thm-ring-matrix-arithmetic-laws](https://alphabetamath.cc/item/thm-ring-matrix-arithmetic-laws) [math:def-determinant-of-a-square-matrix](https://alphabetamath.cc/item/def-determinant-of-a-square-matrix) [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring) [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)

[F8] The quotient by a two-sided ideal uses the sum and product of representatives as representatives of the result. The map to cosets preserves addition, multiplication and identity, and sends precisely the elements of the ideal to zero. [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring) [math:prop-canonical-quotient-ring-map](https://alphabetamath.cc/item/prop-canonical-quotient-ring-map)

## Proof

**Given:** The rational Hamilton algebra $B$, its Hurwitz order $O$, and an odd prime $\ell$.

**Goal:** Construct the integral splitting, identify its reduction and prove the determinant formula.

1.1 Projection $\rho:R\to F$ to the first component preserves the ring operations. It is onto, since any integer representative of a residue defines a compatible tuple. If $x=(x_n)$ projects to zero, each representative of $x_{n+1}$ is divisible by $\ell$. Divide such a representative by $\ell$ and take its class modulo $\ell^n$ to obtain $y_n$. This is independent of the representative because a change by a multiple of $\ell^{n+1}$ changes the quotient by a multiple of $\ell^n$. Compatibility of the $x_n$ gives compatibility of the $y_n$ by the same division. At level $n$ the class $\ell y_n$ equals the reduction of $x_{n+1}$ and hence equals $x_n$. Thus $x=\ell y$ for $y=(y_n)\in R$. Conversely every multiple of $\ell$ projects to zero, so $\ker\rho=\ell R$. [F2, F3, F8]

1.2 Since $\ell>2$ is prime, $2$ does not divide it, so $\ell$ is odd. Each $\ell^n$ is odd, since a product of odd integers is odd by $(2h+1)(2j+1)=2(2hj+h+j)+1$. The residue of $(\ell^n+1)/2$ is therefore an inverse of $2$ modulo $\ell^n$. Reduction of the inverse at level $n+1$ gives an inverse at level $n$, which must be the same by uniqueness of inverses. These residues give $2^{-1}\in R$. [given, F2, F3]

2.1 Set $m=(\ell-1)/2$ and let $E=\{0,\ldots,m\}$, read as distinct residues in $F$. Squaring is injective on $E$, meaning two inputs with the same square must coincide. Indeed, $u^2=v^2$ in $F$ implies $(u-v)(u+v)=0$, so $u=v$ or $u=-v$ in $F$ by invertibility of each nonzero field element. In the latter case the sum of the integer representatives is in $[0,\ell-1]$ and divisible by $\ell$, so both are zero. Now $E\times\{0,1\}$ has $2(m+1)=\ell+1$ elements, whereas $F$ has $\ell$ by uniqueness of remainders. Map $(u,0)$ to $u^2$ and $(u,1)$ to $-1-u^2$. Each branch is injective, so a collision given by the pigeonhole principle supplies $a_0,b_0\in F$ with $a_0^2=-1-b_0^2$. Since $-1\ne0$, at least one of $a_0,b_0$ is nonzero. Interchange the two if necessary so that $a_0\ne0$. [F2, F3, F4, step 1.2]

2.2 For $O_R$ the basis $1,i,j,w$ extends to an $R$-basis, and for $B_K$ it extends to a $K$-basis. Indeed, for either original basis $(e_h)$, send $x\otimes s$ with $x=\sum_h c_he_h$ to the tuple $(c_hs)_h$. This respects addition and balancing, and the inverse sends $(s_h)_h$ to $\sum_h e_h\otimes s_h$ by those same relations. The induced map $O_R\to B_K$ is therefore coefficientwise inclusion in this basis and preserves products by the elementary tensor multiplication rule. We identify $O_R$ with its image. Since $k=2w+1-i-j$ and $2$ is invertible in $R$, the basis can be changed to $1,i,j,k$ by substituting either formula for $w$ or $k$. In this basis $O_R$ is exactly the elements of $B_K$ with all four coordinates in $R$. [F1, F2, F6, step 1.2]

3.1 Take integers $A,B_0$ representing $a_0,b_0$ and view them in $R$. For $f(X)=X^2+B_0^2+1$, one has $\rho(f(A))=0$ and $\rho(f'(A))=2a_0\ne0$ in $F$, since $\ell>2$. By step 1.1 these are the two tests for simple-root lifting. Obtain $a\in R$ with $f(a)=0$, and put $b=B_0\in R$. Then $a^2+b^2=-1$. [F2, F3, F5, step 1.1, step 2.1]

4.1 Let $I$ be the identity matrix and put $U=\begin{pmatrix}0&1\\-1&0\end{pmatrix}$ and $V=\begin{pmatrix}a&b\\b&-a\end{pmatrix}$. Multiplication gives $U^2=-I$, $V^2=(a^2+b^2)I=-I$, and $UV=\begin{pmatrix}b&-a\\-a&-b\end{pmatrix}=-VU$. Every product of $I,U,V,UV$ reduces with these relations to the same signed basis product as for $1,i,j,k$. Indeed, the relations move each $U$ to the left of each $V$ and reduce each square to $-I$. Thus the $K$-linear map $\Phi$ sending $1,i,j,k$ to $I,U,V,UV$ preserves multiplication by expansion in the basis. It preserves the identity and sends scalars to scalar matrices. [construct, F1, F6, F7, step 3.1, step 2.2]

5.1 For coordinates $x_0,x_1,x_2,x_3$, put $d=ax_2+bx_3$ and $e=bx_2-ax_3$. The image matrix has diagonal entries $x_0+d,x_0-d$ and off-diagonal entries $x_1+e,-x_1+e$, in upper then lower order. Conversely a matrix $(m_{st})$ determines $x_0=(m_{11}+m_{22})/2$, $x_1=(m_{12}-m_{21})/2$, $d=(m_{11}-m_{22})/2$ and $e=(m_{12}+m_{21})/2$. The column with entries $d,e$ equals $V$ times the column with entries $x_2,x_3$, so $-V$ recovers the last two coordinates because $V^2=-I$. All the inverse formulas work over both $K$ and $R$, since $a,b,2^{-1}\in R$. Hence $\Phi$ is bijective and takes $O_R$ onto $M_2(R)$. [F6, F7, step 1.2, step 2.2, step 4.1]

6.1 The determinant of the displayed image is $(x_0+d)(x_0-d)-(x_1+e)(-x_1+e)=x_0^2+x_1^2-d^2-e^2$. Expanding the squares gives $d^2+e^2=(a^2+b^2)(x_2^2+x_3^2)$, since the mixed terms cancel. By step 3.1, the determinant is therefore $x_0^2+x_1^2+x_2^2+x_3^2$, which is $N(x)$ for $x\in O$. [F1, F7, step 3.1, step 5.1]

7.1 The subset $\ell O$ is a two-sided ideal because integer scalars are central and $O$ is a ring. Reducing the matrix entries by $\rho$ gives a surjective ring map $M_2(R)\to M_2(F)$ whose elements mapping to zero are precisely $\ell M_2(R)$ by step 1.1. The restriction of $\Phi$ carries $\ell O_R$ onto $\ell M_2(R)$ since it respects scalars and is onto $M_2(R)$. The map $O\to O_R/\ell O_R$ takes the coefficients in $1,i,j,w$ to their residues. Every residue coefficient has an integer representative, and an integer coefficient maps to zero precisely when divisible by $\ell$, so this map is surjective with kernel $\ell O$. Consequently the composite from $O$ to $M_2(F)$ is onto and two inputs have the same image exactly when their difference lies in $\ell O$. It induces the stated bijection on cosets, preserving the ring operations and the $F$-scalar action given by integer representatives. The determinant is a polynomial in the entries with integer coefficients, so its value commutes with entrywise reduction. Step 6.1 now gives the stated norm identity on the quotient and completes the compatible splitting. [F1, F2, F6, F7, F8, step 1.1, step 2.2, step 5.1, step 6.1, discharge-construct] ∎

## Source notes

Voight's discriminant example gives the field splitting through ramification, and his split maximal-order case describes the integral matrix order. The proof here specializes the reduction and root-lifting method to the equation for two squares, then constructs the integral isomorphism and computes its reduction directly. [Quaternion algebras over global fields](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_14) [Discriminants](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_15) [Ternary quadratic forms over local fields](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_12)
