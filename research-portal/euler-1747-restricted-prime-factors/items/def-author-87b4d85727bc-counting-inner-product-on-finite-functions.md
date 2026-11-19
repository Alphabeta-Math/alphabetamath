---
id: def-author-87b4d85727bc-counting-inner-product-on-finite-functions
kind: definition
title: Counting inner product on functions on a finite set
status: published
domain: mathematics
deps:
  - math:def-finite-cardinality
  - math:thm-complex-numbers-form-a-field
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-function-space
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-inner-product-space
  - math:lem-complex-conjugation-and-modulus-laws
  - math:lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product
  - math:thm-reals-ordered-field
formulation_deps:
  - math:def-finite-cardinality
  - math:thm-complex-numbers-form-a-field
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-function-space
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-inner-product-space
argument_deps:
  - math:def-finite-cardinality
  - math:thm-complex-numbers-form-a-field
  - math:def-complex-conjugate-real-imaginary-part-and-modulus
  - math:def-function-space
  - math:def-finite-sum-in-a-commutative-monoid
  - math:def-inner-product-space
  - math:lem-complex-conjugation-and-modulus-laws
  - math:lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product
  - math:thm-reals-ordered-field
dependency_roles:
  math:def-finite-cardinality: mathematical-premise
  math:thm-complex-numbers-form-a-field: mathematical-premise
  math:def-complex-conjugate-real-imaginary-part-and-modulus: mathematical-premise
  math:def-function-space: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:def-inner-product-space: mathematical-premise
  math:lem-complex-conjugation-and-modulus-laws: mathematical-premise
  math:lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Definition

Let $X$ be a nonempty finite set, meaning it can be listed without repetition as $n$ elements for some positive integer $n=|X|$. Write $\mathbb C^X$ for all functions $f:X\to\mathbb C$, where $\mathbb C$ is the field of complex numbers. Its operations are pointwise, so $(f+h)(x)=f(x)+h(x)$, $(\lambda f)(x)=\lambda f(x)$ for $\lambda\in\mathbb C$, and the zero function has value $0$ at every $x$.

The **counting inner product** on $\mathbb C^X$ is
$$\langle f,h\rangle_X=\sum_{x\in X}f(x)\overline{h(x)}.$$
For a complex number $z=a+bi$ with $a,b$ real and $i^2=-1$, its conjugate is $\overline z=a-bi$. The sum adds the indicated complex values, with one term per point of $X$ in any enumeration. The inner product is linear in the first variable, meaning $\langle af+bg,h\rangle_X=a\langle f,h\rangle_X+b\langle g,h\rangle_X$ for complex $a,b$. It is conjugate symmetric, meaning $\langle f,h\rangle_X=\overline{\langle h,f\rangle_X}$, and positive definite, meaning $\langle f,f\rangle_X$ is nonnegative real and equals $0$ exactly for the zero function.

## Definition references

[[math:def-finite-cardinality]]

[[math:thm-complex-numbers-form-a-field]]

[[math:def-complex-conjugate-real-imaginary-part-and-modulus]]

[[math:def-function-space]]

[[math:def-finite-sum-in-a-commutative-monoid]]

[[math:def-inner-product-space]]

## Facts & Assumptions

[F1] The complex numbers form a field extending the reals as a subfield, with every complex number uniquely of the form $a+bi$ for real $a,b$. Complex conjugation sends $a+bi$ to $a-bi$, fixes real numbers, and preserves products. [[math:thm-complex-numbers-form-a-field]] [[math:def-complex-conjugate-real-imaginary-part-and-modulus]] [[math:lem-complex-conjugation-and-modulus-laws]]

[F2] A finite set has a unique cardinality $n$ and admits a bijection with $\{0,\ldots,n-1\}$. The sum in the additive commutative monoid of a field, meaning addition is associative and commutative with identity $0$, is independent of the enumeration. [[math:def-finite-cardinality]] [[math:def-finite-sum-in-a-commutative-monoid]]

[F3] For a field $F$ and set $X$, the functions $X\to F$ form a vector space under the pointwise operations. [[math:def-function-space]] An inner product in the linear-first convention is a complex-valued pairing that is linear in its first variable, conjugate symmetric, and positive definite. [[math:def-inner-product-space]]

[F4] For a nonempty finite set $X$ and $n=|X|$ viewed as a positive real number, $L(f,h)=n^{-1}\sum_{x\in X}f(x)\overline{h(x)}$ is an inner product on $\mathbb C^X$ with the pointwise operations. [[math:lem-standard-hermitian-form-on-functions-on-a-nonempty-finite-set-is-an-inner-product]]

[F5] The real numbers form an ordered field, so the product of two positive real numbers is positive. [[math:thm-reals-ordered-field]]

## Justification

The summands are complex values of a function on the finite set $X$. The finite-sum construction therefore gives a single complex value from the summands, in any order.

## Proof

**Given:** A nonempty finite set $X$ and the field $\mathbb C$ with its conjugation.

**Goal:** Verify the pointwise function space and the counting inner product.

1.1 Apply [F3] with the field $\mathbb C$ from [F1] to obtain the vector space $\mathbb C^X$. For each $x$, the conjugate and product defining the summand are complex numbers by [F1]. Therefore [F2] gives a single complex value for the counting pairing, independent of the enumeration. [F1, F2, F3]

2.1 Since $X$ is nonempty and finite, apply [F4] to obtain $L$ with $n>0$. Multiplying its formula by $n$ in the field gives $\langle f,h\rangle_X=nL(f,h)$. First-variable linearity follows by distributing this factor across the linearity identity of $L$. Conjugate symmetry holds because $n$ is real and $\overline{nL(h,f)}=n\overline{L(h,f)}=nL(f,h)$. By [F4], $L(f,f)$ is real and nonnegative. Since $n$ is real, $nL(f,f)$ is real by [F1]. It is zero if $L(f,f)=0$ by the field laws, and positive if $L(f,f)>0$ by [F5]. Hence it is nonnegative and vanishes exactly for $f=0$ by [F4]. Thus the counting pairing is an inner product in the stated convention. [F1, F3, F4, F5, step 1.1] ∎
