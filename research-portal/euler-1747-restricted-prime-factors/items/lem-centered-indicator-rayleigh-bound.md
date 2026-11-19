---
id: lem-centered-indicator-rayleigh-bound
kind: lemma
title: Centered indicator and its Rayleigh quotient bound
status: published
domain: mathematics
deps:
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-abs-value
  - math:lem-of-square-positive
  - math:def-sum-over-a-finite-index-set
  - math:lem-finite-sum-laws
  - math:def-canonical-natural
  - math:lem-of-naturals-positive
  - math:def-linear-combination-and-span
  - math:def-linear-independence
  - math:lem-span-is-the-set-of-linear-combinations
  - math:def-finite-cardinality
  - math:def-inner-product-space
  - math:def-inner-product-norm
  - math:def-linear-map
  - math:def-self-adjoint-and-normal-endomorphism
  - math:def-adjoint-of-a-linear-map-between-inner-product-spaces
  - math:def-linear-subspace
  - math:def-invariant-subspace-and-induced-quotient-operator
  - math:def-operator-norm-on-a-finite-dimensional-inner-product-space
  - math:def-orthogonal-vectors-sets-and-orthonormal-bases
  - math:def-linear-basis
  - math:thm-dimension-of-a-linear-subspace
  - math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces
  - math:thm-subset-of-a-finite-set
  - math:def-function-space
  - math:thm-reals-ordered-field
  - math:thm-complex-numbers-form-a-field
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-complex-conjugation-and-modulus-laws
  - math:def-dimension
  - math:thm-operator-norm-is-the-largest-singular-value
  - math:lem-of-abs-value
  - math:lem-complex-modulus-of-real-embedding-equals-real-absolute-value
formulation_deps:
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-canonical-natural
  - math:lem-of-naturals-positive
  - math:def-linear-combination-and-span
  - math:thm-dimension-of-a-linear-subspace
  - math:def-finite-cardinality
  - math:def-inner-product-space
  - math:def-inner-product-norm
  - math:def-linear-map
  - math:def-self-adjoint-and-normal-endomorphism
  - math:def-adjoint-of-a-linear-map-between-inner-product-spaces
  - math:def-linear-subspace
  - math:def-invariant-subspace-and-induced-quotient-operator
  - math:def-operator-norm-on-a-finite-dimensional-inner-product-space
  - math:def-orthogonal-vectors-sets-and-orthonormal-bases
  - math:thm-subset-of-a-finite-set
  - math:def-function-space
  - math:thm-reals-ordered-field
  - math:thm-complex-numbers-form-a-field
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-complex-conjugation-and-modulus-laws
  - math:def-dimension
  - math:thm-operator-norm-is-the-largest-singular-value
argument_deps:
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-abs-value
  - math:lem-of-square-positive
  - math:def-sum-over-a-finite-index-set
  - math:lem-finite-sum-laws
  - math:def-canonical-natural
  - math:lem-of-naturals-positive
  - math:def-linear-combination-and-span
  - math:def-linear-independence
  - math:lem-span-is-the-set-of-linear-combinations
  - math:def-finite-cardinality
  - math:def-inner-product-space
  - math:def-inner-product-norm
  - math:def-linear-map
  - math:def-self-adjoint-and-normal-endomorphism
  - math:def-adjoint-of-a-linear-map-between-inner-product-spaces
  - math:def-linear-subspace
  - math:def-invariant-subspace-and-induced-quotient-operator
  - math:def-operator-norm-on-a-finite-dimensional-inner-product-space
  - math:def-orthogonal-vectors-sets-and-orthonormal-bases
  - math:def-linear-basis
  - math:thm-dimension-of-a-linear-subspace
  - math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces
  - math:thm-subset-of-a-finite-set
  - math:def-function-space
  - math:thm-reals-ordered-field
  - math:thm-complex-numbers-form-a-field
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-complex-conjugation-and-modulus-laws
  - math:def-dimension
  - math:thm-operator-norm-is-the-largest-singular-value
  - math:lem-of-abs-value
  - math:lem-complex-modulus-of-real-embedding-equals-real-absolute-value
dependency_roles:
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:def-abs-value: mathematical-premise
  math:lem-of-square-positive: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:lem-finite-sum-laws: mathematical-premise
  math:def-canonical-natural: mathematical-premise
  math:lem-of-naturals-positive: mathematical-premise
  math:def-linear-combination-and-span: mathematical-premise
  math:def-linear-independence: mathematical-premise
  math:lem-span-is-the-set-of-linear-combinations: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-inner-product-space: mathematical-premise
  math:def-inner-product-norm: mathematical-premise
  math:def-linear-map: mathematical-premise
  math:def-self-adjoint-and-normal-endomorphism: mathematical-premise
  math:def-adjoint-of-a-linear-map-between-inner-product-spaces: mathematical-premise
  math:def-linear-subspace: mathematical-premise
  math:def-invariant-subspace-and-induced-quotient-operator: mathematical-premise
  math:def-operator-norm-on-a-finite-dimensional-inner-product-space: mathematical-premise
  math:def-orthogonal-vectors-sets-and-orthonormal-bases: mathematical-premise
  math:def-linear-basis: mathematical-premise
  math:thm-dimension-of-a-linear-subspace: mathematical-premise
  math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-function-space: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:lem-complex-conjugation-and-modulus-laws: mathematical-premise
  math:def-dimension: mathematical-premise
  math:thm-operator-norm-is-the-largest-singular-value: mathematical-premise
  math:lem-of-abs-value: mathematical-premise
  math:lem-complex-modulus-of-real-embedding-equals-real-absolute-value: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $Y$ be a nonempty finite set and $O\subseteq Y$ a nonempty subset. Write $|A|$ for the number of elements of a finite set $A$. On $V=\mathbb K^Y$, the space of functions $Y\to\mathbb K$ for $\mathbb K=\mathbb R$ or $\mathbb C$, use pointwise vector operations and the counting inner product $\langle u,v\rangle=\sum_{y\in Y}u(y)\overline{v(y)}$. The bar fixes real numbers and sends $a+ib$ to $a-ib$ for real $a,b$. Write $\|v\|=\sqrt{\langle v,v\rangle}$. In scalar expressions, a cardinality $n=|A|$ denotes the sum of $n$ copies of $1$ in $\mathbb R$, viewed in $\mathbb C$ by its real field embedding when needed.

Let $f=\mathbf1_O$ be the indicator of $O$, equal to $1$ on $O$ and $0$ elsewhere, and let $\mathbf1$ be the constant function equal to $1$. Put $\mu=|O|/|Y|$ and $h=f-\mu\mathbf1$. Then $h$ is orthogonal to $\mathbf1$, meaning $\langle h,\mathbf1\rangle=0$, and $\|h\|^2=|O|(1-\mu)$.

Suppose $T:V\to V$ is linear, meaning it preserves linear combinations, and self-adjoint, meaning $\langle Tu,v\rangle=\langle u,Tv\rangle$ for all $u,v\in V$. Assume $T\mathbf1=d\mathbf1$ for $d\in\mathbb R$. Suppose $h$ belongs to a linear subspace $W$ (a subset containing zero and closed under linear combinations) that is $T$-invariant, meaning $T(W)\subseteq W$. Assume the restriction $T|_W:w\mapsto Tw$ on $W$ has operator norm at most $L$, where $L\ge0$. This bound says $\|Tw\|\le L$ for every $w\in W$ with $\|w\|=1$, with the operator norm defined to be zero on the zero space. Then the Rayleigh quotient of $f$, the pairing $\langle f,Tf\rangle$ divided by $\langle f,f\rangle=|O|$, satisfies
$$\frac{\langle f,Tf\rangle}{|O|}\le d\mu+L(1-\mu).$$

## Statement references

[[math:def-canonical-natural]]

[[math:lem-of-naturals-positive]]

[[math:def-linear-combination-and-span]]

[[math:thm-dimension-of-a-linear-subspace]]

[[math:def-finite-cardinality]]

[[math:def-inner-product-space]]

[[math:def-inner-product-norm]]

[[math:def-linear-map]]

[[math:def-self-adjoint-and-normal-endomorphism]]

[[math:def-adjoint-of-a-linear-map-between-inner-product-spaces]]

[[math:def-linear-subspace]]

[[math:def-invariant-subspace-and-induced-quotient-operator]]

[[math:def-operator-norm-on-a-finite-dimensional-inner-product-space]]

[[math:def-orthogonal-vectors-sets-and-orthonormal-bases]]

[[math:thm-subset-of-a-finite-set]]

[[math:def-function-space]]

[[math:thm-reals-ordered-field]]

[[math:thm-complex-numbers-form-a-field]]

[[math:def-finite-sum-in-a-commutative-monoid]]

[[math:lem-complex-conjugation-and-modulus-laws]]

[[math:def-complex-conjugate-real-imaginary-part-and-modulus]]

[[math:def-dimension]]

[[math:thm-operator-norm-is-the-largest-singular-value]]

## Justification

The indicator and constant functions specify a single value at every point of $Y$. Since $O\subseteq Y$ and $Y$ is finite, $O$ is finite by clause 1 of [[math:thm-subset-of-a-finite-set]]. Nonemptiness means that the natural cardinalities of $O$ and $Y$ are nonzero ([[math:def-finite-cardinality]]). Their real images under the canonical natural map ([[math:def-canonical-natural]]) are positive by [[math:lem-of-naturals-positive]] applied in the ordered field $\mathbb R$ ([[math:thm-reals-ordered-field]]), so $\mu$ is defined. The real field embedding into $\mathbb C$ ([[math:thm-complex-numbers-form-a-field]]) preserves both $1$ and addition, so the embedded count agrees with the sum of the same number of complex units $1$. The scalars form a field in either case ([[math:thm-reals-ordered-field]], [[math:thm-complex-numbers-form-a-field]]). By [[math:def-function-space]], pointwise addition and scalar multiplication make $V$ a vector space over $\mathbb K$, with the constant zero function as zero vector. The sums over $Y$ are independent of enumeration by [[math:def-finite-sum-in-a-commutative-monoid]], applied to the additive commutative monoids of $\mathbb K$ and $V$. In any enumeration, distributivity term by term gives linearity of the counting pairing in its first variable. Conjugation is additive, multiplicative and involutive by [[math:lem-complex-conjugation-and-modulus-laws]] in the complex case, and is the identity in the real case. Consequently conjugating the finite sum for $\langle v,u\rangle$ gives $\langle u,v\rangle$. By [[math:thm-complex-numbers-form-a-field]] and [[math:def-complex-conjugate-real-imaginary-part-and-modulus]], each term $v(y)\overline{v(y)}$ on the diagonal is the real number $a^2+b^2$ when $v(y)=a+ib$, with $b=0$ in the real case. In the ordered field $\mathbb R$ ([[math:thm-reals-ordered-field]]), a real square is zero when its base is zero and positive otherwise by [[math:lem-of-square-positive]]. Thus $a^2+b^2$ is nonnegative and is zero exactly when $a=b=0$, equivalently when $v(y)=0$. Enumerate $Y$ by $y_0,\ldots,y_{n-1}$, with $n=|Y|$ as a natural number. By [[math:def-finite-sum-in-a-commutative-monoid]] and [[math:def-sum-over-a-finite-index-set]], the sum of the real diagonal terms over $Y$ is the recursive real sum of this list. In the complex case the diagonal pairing is the image of this real sum because the real field embedding preserves zero and addition. Clause 4 of [[math:lem-finite-sum-laws]] now gives a nonnegative real sum and says that if the sum is zero, every summand is zero. Conversely, a list of all zero terms sums to zero. Therefore the diagonal pairing vanishes exactly when $v$ vanishes at every point. This verifies the inner-product axioms and gives the stated norm by the nonnegative square root.

For each $y\in Y$, let $\delta_y$ equal $1$ at $y$ and $0$ elsewhere. Write $B=\{\delta_y:y\in Y\}$. The map $y\mapsto\delta_y$ is a bijection onto $B$, since distinct points give distinct indicators by evaluation. For each $u\in V$, the equality $u=\sum_{y\in Y}u(y)\delta_y$ holds because the right side evaluates to $u(z)$ at each $z\in Y$. Enumerating $Y$ exhibits the sum as a finite linear combination of elements of $B$ ([[math:def-linear-combination-and-span]]). It belongs to the span of $B$ by [[math:lem-span-is-the-set-of-linear-combinations]], so $B$ spans $V$. For any injective finite list $(\delta_{y_j})$ in $B$, evaluation at $y_j$ of a combination $\sum_i c_i\delta_{y_i}=0$ gives $c_j=0$, because the points $y_i$ in the list are distinct. This holds at every index, so $B$ is linearly independent by [[math:def-linear-independence]]. Thus $B$ is a basis ([[math:def-linear-basis]]). The bijection from $Y$ to $B$ makes $B$ finite ([[math:def-finite-cardinality]]), so $V$ is finite-dimensional ([[math:def-dimension]]) and clause 1 of [[math:thm-dimension-of-a-linear-subspace]] makes $W$ finite-dimensional. The pairing restricts to an inner product on $W$ because its axioms continue to hold on vectors in $W$. Invariance ensures that the value $Tw$ lies in $W$, and the restriction inherits linearity from $T$. The operator norm hypothesis therefore applies to a linear map from a finite-dimensional inner product space to itself. If $W\ne\{0\}$, [[math:thm-operator-norm-is-the-largest-singular-value]] gives attainment of the maximum over the unit vectors of $W$, including when $T|_W=0$. If $W=\{0\}$, [[math:def-operator-norm-on-a-finite-dimensional-inner-product-space]] sets the norm of the restriction to zero. The denominator $\langle f,f\rangle=|O|$ is positive since the diagonal sum contributes one per element of $O$, and $\langle f,Tf\rangle$ is real by self-adjointness and conjugate symmetry. Likewise $\langle T\mathbf1,\mathbf1\rangle=d|Y|$ is real, so the scalar $d$ is necessarily real.

## Facts & Assumptions

[F1] For a finite set the cardinality is a natural number, nonzero when the set is nonempty ([[math:def-finite-cardinality]]). As a real scalar it is the corresponding sum of ones ([[math:def-canonical-natural]]), positive for a nonempty set ([[math:lem-of-naturals-positive]] in [[math:thm-reals-ordered-field]]). Its image in $\mathbb C$ is the corresponding sum of complex ones ([[math:thm-complex-numbers-form-a-field]]).

[F2] The counting pairing is linear in its first variable, conjugate-linear in its second, conjugate symmetric and positive definite. The induced norm is the nonnegative square root of the diagonal pairing ([[math:def-inner-product-space]], [[math:def-inner-product-norm]]).

[F3] A linear map preserves linear combinations, and self-adjointness identifies $T$ with its adjoint, whose defining identity gives $\langle Tu,v\rangle=\langle u,Tv\rangle$ ([[math:def-linear-map]], [[math:def-self-adjoint-and-normal-endomorphism]], [[math:def-adjoint-of-a-linear-map-between-inner-product-spaces]]).

[F4] A linear subspace inherits the vector operations, and invariance $T(W)\subseteq W$ gives the restriction $T|_W:W\to W$ ([[math:def-linear-subspace]], [[math:def-invariant-subspace-and-induced-quotient-operator]]).

[F5] On a nonzero finite-dimensional inner product space, the operator norm is the maximum of $\|Tw\|$ over vectors of norm one. On the zero space it is $0$ ([[math:def-operator-norm-on-a-finite-dimensional-inner-product-space]]).

[F6] Cauchy–Schwarz gives $|\langle u,v\rangle|\le\|u\|\|v\|$ for vectors in a real or complex inner product space ([[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces]]). The bars denote real absolute value on $\mathbb R$ ([[math:def-abs-value]]) and complex modulus on $\mathbb C$ ([[math:def-complex-conjugate-real-imaginary-part-and-modulus]]).

[F7] Orthogonality of two vectors means their inner product vanishes ([[math:def-orthogonal-vectors-sets-and-orthonormal-bases]]).

[F8] A sum indexed by a finite set in an additive commutative monoid can be evaluated in any enumeration ([[math:def-finite-sum-in-a-commutative-monoid]]).

[F9] In the ordered real field ([[math:thm-reals-ordered-field]]), every real number $r$ satisfies $r\le |r|_{\mathbb R}$ ([[math:lem-of-abs-value]]). When $r$ is viewed in $\mathbb C$, its complex modulus equals $|r|_{\mathbb R}$ ([[math:lem-complex-modulus-of-real-embedding-equals-real-absolute-value]]).

## Proof

**Given:** $Y,O,f,\mu,h$ as in the statement and, for the bound, $T,d,W,L$ satisfying its hypotheses.

**Goal:** Show that $h$ is orthogonal to $\mathbf1$ with $\|h\|^2=|O|(1-\mu)$, then establish the quotient bound.

1.1 In the counting sums, $f$ takes value $1$ at the $|O|$ indices in $O$ and $0$ at every other index. Discarding the zero terms leaves sums of ones, which give the scalar counts by [F1]. Thus $\langle f,\mathbf1\rangle=\langle f,f\rangle=|O|$ and $\langle\mathbf1,\mathbf1\rangle=|Y|$. Linearity gives $\langle h,\mathbf1\rangle=|O|-\mu|Y|=0$. Therefore $h$ is orthogonal to $\mathbf1$, and conjugate symmetry gives $\langle\mathbf1,h\rangle=0$. [given, F1, F2, F7, F8]

2.1 In $\langle f,f\rangle=\langle h+\mu\mathbf1,h+\mu\mathbf1\rangle$ both cross terms vanish by step 1.1. Since $\mu$ is real, $\|h\|^2=|O|-\mu^2|Y|=|O|(1-\mu)$. [step 1.1, F2, algebra]

2.2 Self-adjointness and $T\mathbf1=d\mathbf1$ give $\langle\mathbf1,Th\rangle=\langle T\mathbf1,h\rangle=d\langle\mathbf1,h\rangle=0$ and $\langle h,T\mathbf1\rangle=d\langle h,\mathbf1\rangle=0$. Expanding $\langle f,Tf\rangle$ using $f=h+\mu\mathbf1$ now gives $\langle f,Tf\rangle=d\mu^2|Y|+\langle h,Th\rangle=d\mu|O|+\langle h,Th\rangle$. Also $\langle h,Th\rangle=\langle Th,h\rangle=\overline{\langle h,Th\rangle}$, so the centered pairing is real. [given, step 1.1, F2, F3, algebra]

3.1 For real $a\ge0$ and $v\in V$, sesquilinearity gives $\|av\|^2=a^2\|v\|^2$, so $\|av\|=a\|v\|$ by uniqueness of the nonnegative square root. If $h=0$, then $Th=0$ by linearity and $\|Th\|\le L\|h\|$. If $h\ne0$, then $s=\|h\|>0$ by positive definiteness. The vector $w=h/s$ belongs to $W$ and the scaling identity gives $\|w\|=\|h\|/s=1$. Thus $\|Tw\|\le L$, and $Th=sTw$ by linearity. Scaling gives $\|Th\|=s\|Tw\|\le L\|h\|$. In both cases, write $r=\langle h,Th\rangle$, which is real by step 2.2. For $\mathbb K=\mathbb R$, the bars in [F6] give $|r|_{\mathbb R}$. For $\mathbb K=\mathbb C$, they give the modulus of the embedded real $r$, which equals $|r|_{\mathbb R}$ by [F9]. In either case [F9] gives $r\le|r|_{\mathbb R}$. Applying Cauchy–Schwarz to $h,Th\in V$ gives $|r|_{\mathbb R}\le\|h\|\|Th\|\le L\|h\|^2$. [given, step 2.2, F2, F3, F4, F5, F6, F9]

4.1 Substitute the bound from step 3.1 and the norm identity from step 2.1 into step 2.2. Dividing by the positive number $|O|$ yields $\langle f,Tf\rangle/|O|\le d\mu+L(1-\mu)$. If $O=Y$, then $h=0$ and $\mu=1$, so the identity in step 2.2 gives equality. Together with steps 1.1 and 2.1 this proves all assertions. [F1, step 1.1, step 2.1, step 2.2, step 3.1] ∎
