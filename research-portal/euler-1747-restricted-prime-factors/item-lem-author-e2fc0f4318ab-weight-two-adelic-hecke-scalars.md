---
title: Good-prime Hecke scalars in the weight-two adelic model
status: draft
research_item: lem-author-e2fc0f4318ab-weight-two-adelic-hecke-scalars
dependency_level: 3
---

## Prerequisites

- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:def-countable-choice](https://alphabetamath.cc/item/def-countable-choice)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [def-author-e2fc0f4318ab-weight-two-cusp-form](item-def-author-e2fc0f4318ab-weight-two-cusp-form)
- [def-author-e2fc0f4318ab-normalized-weight-two-newform](item-def-author-e2fc0f4318ab-normalized-weight-two-newform)
- [def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles)
- [lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)
- [math:thm-chinese-remainder-theorem](https://alphabetamath.cc/item/thm-chinese-remainder-theorem)
- [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)
- [def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)
- [math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)
- [math:def-function-space](https://alphabetamath.cc/item/def-function-space)
- [math:def-dirichlet-character-modulo-q](https://alphabetamath.cc/item/def-dirichlet-character-modulo-q)
- [lem-author-e2fc0f4318ab-classical-hecke-first-coefficient](item-lem-author-e2fc0f4318ab-classical-hecke-first-coefficient)
- [lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)
- [math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)


## Statement

Assume countable choice and let $f$ be a normalized weight-two cuspidal newform of level $N$ and character $\epsilon$, with Fourier coefficients $a_n$ at infinity. Fix a prime $\ell\nmid N$. Write $\mathbb A=\mathbb R\times\mathbb A_f$, where the finite adele ring $\mathbb A_f$ consists of tuples of $p$-adic numbers integral for all but finitely many primes $p$. Thus $\mathrm{GL}_2(\mathbb A)$ consists of a real invertible matrix and invertible $p$-adic matrices lying in $\mathrm{GL}_2(\mathbb Z_p)$ at all but finitely many $p$.

Let $K_0(N)$ be the group of tuples $k=(k_p)_p$ with $k_p\in\mathrm{GL}_2(\mathbb Z_p)$ and lower left entry in $N\mathbb Z_p$ at every $p$, embedded with real component the identity. For each $p\mid N$ let $e_p$ be its exponent in the prime factorization of $N$. Identify the unit ball $\mathbb Z_p$ in $\mathbb Q_p$ with the ring of compatible residues and reduce the lower right entry of $k_p$ modulo $p^{e_p}$. Combine these residues for the distinct maximal prime powers $p^{e_p}$ by the Chinese remainder theorem to obtain the unit class $d(k)$ modulo $N$. For $N=1$ the list is empty and $d(k)$ is the sole class modulo $1$.

Let $\Phi:\mathrm{GL}_2(\mathbb A)\to\mathbb C$ be invariant under left multiplication by $\mathrm{GL}_2(\mathbb Q)$ embedded by using the same rational matrix at every place. Suppose
$$\Phi(gk)=\epsilon(d(k))^{-1}\Phi(g),\qquad \Phi(h_\infty)=(f|_2 h)(i)$$
for all $g\in\mathrm{GL}_2(\mathbb A)$, $k\in K_0(N)$ and $h\in\mathrm{GL}_2^+(\mathbb R)$, the real matrices of positive determinant. Here $h_\infty$ denotes $h$ at the real place with identity at every prime.

On the complex vector space of functions from $\mathrm{GL}_2(\mathbb A)$ to $\mathbb C$ with pointwise operations, use the right-translation representation $(\pi(x)F)(g)=F(gx_\ell)$, where $x_\ell$ denotes insertion of $x\in\mathrm{GL}_2(\mathbb Q_\ell)$ at $\ell$ with identity elsewhere. Then $\Phi$ is fixed by $K=\mathrm{GL}_2(\mathbb Z_\ell)$. Let $\mathcal T_\ell$ and $\mathcal R_\ell$ be the Hecke operators of the indicators of $K\operatorname{diag}(\ell,1)K$ and $(\ell I)K$, respectively, summing one term per coset $xK$. If these two operators act on $\Phi$ by scalars, the scalars are respectively $a_\ell$ and $\epsilon(\ell)$.

## Facts & Assumptions

[F1] The finite adele ring uses coordinatewise operations and the rational embeddings give $|a/b|_p\le1$ for integers $a,b$ with $p\nmid b$, with equality if $p\nmid a$ ([def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles](item-def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles), justification of the diagonal rational embedding). The distinct maximal prime powers $p^{e_p}$ are pairwise coprime and have product $N$. The Chinese remainder map for this list is a unital ring isomorphism, also for the empty list at $N=1$ ([math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic), [math:thm-chinese-remainder-theorem](https://alphabetamath.cc/item/thm-chinese-remainder-theorem)). The canonical identification of the unit ball with the compatible-residue ring gives unital ring maps to $\mathbb Z/p^{e_p}\mathbb Z$. The construction by eventual residues gives usual reduction on an embedded integer, using the constant integer sequence ([math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp), [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)). The character is a group homomorphism from units modulo $N$ to $\mathbb C^\times$ ([math:def-dirichlet-character-modulo-q](https://alphabetamath.cc/item/def-dirichlet-character-modulo-q)).

[F2] The weight-two action has $(f|_2 A)|_2 B=f|_2(AB)$ for real matrices of positive determinant. The transformation for $\begin{pmatrix}1&1\\0&1\end{pmatrix}\in\Gamma_0(N)$ gives $f(z+1)=f(z)$ since its lower right entry is $1$ and $\epsilon(1)=1$ ([def-author-e2fc0f4318ab-weight-two-cusp-form](item-def-author-e2fc0f4318ab-weight-two-cusp-form), [math:def-dirichlet-character-modulo-q](https://alphabetamath.cc/item/def-dirichlet-character-modulo-q)). At the good prime the classical formula is $(T_\ell f)(z)=\ell^{-1}\sum_{b=0}^{\ell-1}f((z+b)/\ell)+\ell\epsilon(\ell)f(\ell z)$ and $T_\ell f=a_\ell f$ ([def-author-e2fc0f4318ab-normalized-weight-two-newform](item-def-author-e2fc0f4318ab-normalized-weight-two-newform), [lem-author-e2fc0f4318ab-classical-hecke-first-coefficient](item-lem-author-e2fc0f4318ab-classical-hecke-first-coefficient)).

[F3] Under countable choice the local group is Hausdorff, $K$ is compact and open, and the valuation is additive and zero on local scalar units ([lem-author-d45da46285be-triangular-cosets](item-lem-author-d45da46285be-triangular-cosets)). Determinant is multiplicative over the local field and the local integer ring ([math:thm-determinant-multiplicative](https://alphabetamath.cc/item/thm-determinant-multiplicative)). At exponent one the index-coset formula for integral matrices of determinant valuation one gives exactly the representatives $M_b=\begin{pmatrix}\ell&b\\0&1\end{pmatrix}$ for $0\le b<\ell$ and $M_*=\operatorname{diag}(1,\ell)$ ([lem-degree-two-spherical-index-cosets](item-lem-degree-two-spherical-index-cosets)).

[F4] The complex numbers form a field ([math:thm-complex-numbers-form-a-field](https://alphabetamath.cc/item/thm-complex-numbers-form-a-field)). For any set, the functions from that set to a field form a vector space under pointwise operations ([math:def-function-space](https://alphabetamath.cc/item/def-function-space)). For a complex representation of a Hausdorff group with a compact open subgroup, the spherical action on fixed vectors sums one term per coset $xK$ for the indicator of a compact double coset ([def-author-d45da46285be-spherical-hecke-algebra](item-def-author-d45da46285be-spherical-hecke-algebra)).

## Proof

**Given:** The normalized newform, the good prime and the invariance, covariance and real restriction of $\Phi$ stated above.

**Goal:** Establish $K$-fixedness and identify the scalars when the two operators act by scalars on $\Phi$.

1.1 The lower left condition defining $K_0(N)$ is preserved by multiplication since the lower left entry of a product is a sum of multiples of the two lower left entries. Inversion preserves it since the lower left entry of an inverse is the negative of the original entry divided by the determinant, which is a unit by determinant multiplicativity applied to the integral inverse. For $p\mid N$, reduction modulo $p^{e_p}$ sends $N$ to zero and $k_p$ to an invertible upper triangular matrix, with inverse given by the reduction of $k_p^{-1}$. Its diagonal product is a unit, so each diagonal entry is a unit. The lower right entries multiply under products of these triangular matrices. The Chinese remainder isomorphism therefore gives a well-defined unit class $d(k)$ and a group homomorphism $d$, including for $N=1$. [F1, F3, given]

2.1 For $x\in K$, $x_\ell$ lies in $K_0(N)$ since $N$ is a unit of $\mathbb Z_\ell$ by $\ell\nmid N$, and the other finite components are identities. Hence $d(x_\ell)=1$. Covariance and $\epsilon(1)=1$ give $\pi(x)\Phi=\Phi$. On the function space in [F4], evaluating at $gx_\ell$ preserves pointwise linear combinations. For each function $F$, $(\pi(x)\pi(y)F)(g)=F(gx_\ell y_\ell)=F(g(xy)_\ell)$ because insertion at $\ell$ preserves multiplication. Insertion of the identity gives the identity operator, so $\pi(x^{-1})$ is the inverse of $\pi(x)$. In particular $\pi(yk)\Phi=\pi(y)\Phi$ for $k\in K$, which makes each term in a coset sum independent of its representative. [F1, F3, F4, given, step 1.1]

3.1 Each matrix in $K\operatorname{diag}(\ell,1)K$ is integral and has determinant valuation one since the determinants of the two $K$ factors are units. Conversely, $M_b=\begin{pmatrix}1&b\\0&1\end{pmatrix}\operatorname{diag}(\ell,1)$ and $M_*$ is the conjugate of $\operatorname{diag}(\ell,1)$ by the coordinate swap in $K$. Thus all the representatives in [F3] belong to the named double coset, which consequently equals the integral determinant-valuation-one locus. The scalar matrix $M'_0=\ell I$ is central, so its double coset is the single coset $(\ell I)K$. Both supports are bi-invariant under $K$ and compact as finite unions of translates of $K$. Hence their indicators act by the finite coset sums in [F4] on the $K$-fixed vector from step 2.1. [F3, F4, step 1.1, step 2.1]

4.1 For each rational representative $M$ from step 3.1, take $k(M)$ to have $M^{-1}$ at finite primes other than $\ell$ and identity at $\ell$ and the real place. The entries of $M^{-1}$ have denominators that are powers of $\ell$ and $M$ is integral, so both matrices are integral away from $\ell$. The inverse is upper triangular, giving $k(M)\in K_0(N)$. The lower right entry of $M^{-1}$ is the inverse of the embedded integer $d_M$, the lower right entry of $M$. The unital reduction map sends it to the inverse of the usual residue of $d_M$, so $d(k(M))=[d_M]_N^{-1}$ by the Chinese remainder map. The factorization $h_\infty M_\ell=M\,(M^{-1}h)_\infty\,k(M)$ holds coordinate by coordinate. The assumed invariance and covariance give $\Phi(h_\infty M_\ell)=\epsilon(d_M)((f|_2 M^{-1})|_2 h)(i)$. [F1, F2, given, step 1.1, step 3.1]

5.1 The weight-two formula gives $(f|_2 M_b^{-1})(z)=\ell^{-1}f((z-b)/\ell)$ with $d_{M_b}=1$ and $(f|_2 M_*^{-1})(z)=\ell f(\ell z)$ with $d_{M_*}=\ell$. By period one of $f$, the sum with $-b$ equals the sum with $b$, since negation permutes the residues modulo $\ell$. Thus the sum in $\mathcal T_\ell\Phi$ at $h_\infty$ is $((T_\ell f)|_2 h)(i)=a_\ell\Phi(h_\infty)$. The matrix $(M'_0)^{-1}$ is a positive scalar matrix whose weight-two action is the identity, and $d_{M'_0}=\ell$. Hence $\mathcal R_\ell\Phi(h_\infty)=\epsilon(\ell)\Phi(h_\infty)$. Since $a_1=1$, $f$ is nonzero at some $x+iy$ with $y>0$, and $h=\begin{pmatrix}y&x\\0&1\end{pmatrix}$ sends $i$ there and has nonzero weight factor. Equality at this $h_\infty$ identifies both assumed scalars. [F2, F4, given, step 2.1, step 3.1, step 4.1] ∎
