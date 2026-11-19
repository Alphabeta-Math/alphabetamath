---
id: def-euler-hurwitz-normalizer-orbit
kind: definition
title: Normalizer orbit, indicator and density
status: draft
domain: mathematics
deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-torus-normalizer
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-finite-cardinality
  - math:def-rationals
  - math:thm-subset-of-a-finite-set
  - math:def-cartesian-product
  - math:def-complex-numbers-and-arithmetic
  - math:lem-nat-embeds-int
  - math:def-int-operations
formulation_deps:
  - def-euler-prime-classes
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-torus-normalizer
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-finite-cardinality
  - math:def-rationals
  - math:def-cartesian-product
  - math:def-complex-numbers-and-arithmetic
  - math:lem-nat-embeds-int
argument_deps:
  - def-euler-hurwitz-projective-reduction
  - def-euler-hurwitz-torus-normalizer
  - math:def-group
  - math:def-subgroup
  - math:def-coset
  - math:def-subset-and-proper-subset
  - math:def-function
  - math:def-finite-cardinality
  - math:def-rationals
  - math:thm-subset-of-a-finite-set
  - math:def-cartesian-product
  - math:def-complex-numbers-and-arithmetic
  - math:lem-nat-embeds-int
  - math:def-int-operations
dependency_roles:
  def-euler-prime-classes: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  def-euler-hurwitz-torus-normalizer: mathematical-premise
  math:def-group: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-function: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:def-rationals: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-complex-numbers-and-arithmetic: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-int-operations: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, displayed orbit and indicator definitions
      reading_limits: Checked the displayed definitions on PDF page 4 for attribution.
dependency_level: 6
---

## Definition

Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Use the fixed projective reduction at $p$. Its group $G_p$ consists of classes of invertible two-by-two matrices over the field of residues modulo $p$, with matrices identified up to nonzero scalar multiples and products taken on representatives. The subgroup $\Gamma_p$ is the image of the units of the Hurwitz order under that reduction. A subgroup contains the group identity and is closed under products and inverses. The finite set $Y_p=\Gamma_p\backslash G_p$ consists of the right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$ for $g\in G_p$. In particular, the identity $e$ of $G_p$ gives the base coset $\Gamma_p e=\Gamma_p$.

Use the subgroup $K_p=N_{G_p}(C_p)$ from the same reduction. It is the normalizer of the subgroup $C_p$ specified in the torus construction, meaning that it consists of the elements $k\in G_p$ for which $\{kck^{-1}:c\in C_p\}=C_p$. Right translation is the function $Y_p\times K_p\to Y_p$ given by $y\cdot k=\Gamma_p(gk)$ for $(y,k)\in Y_p\times K_p$ with $y=\Gamma_p g$. A right action is such a rule satisfying $y\cdot e=y$ and $(y\cdot k_1)\cdot k_2=y\cdot(k_1k_2)$ for all $y\in Y_p$ and $k_1,k_2\in K_p$. The orbit of a point is the set of its translates. Define the normalizer orbit of the base coset by
$$\mathcal O_p=\{\Gamma_pk:k\in K_p\}\subseteq Y_p.$$

Define $f_p=\mathbf 1_{\mathcal O_p}$, the indicator function on $Y_p$, by setting $f_p(y)=1$ when $y\in\mathcal O_p$ and $f_p(y)=0$ otherwise. Both values are constant classes of the corresponding real numbers in $\mathbb C$, so $f_p$ is a function from $Y_p$ to $\mathbb C$.

For a finite set $S$, write $|S|$ for its cardinality, the natural number that counts its elements. Define the density of $\mathcal O_p$ in $Y_p$ as the rational fraction
$$\mu_p=\frac{|\mathcal O_p|}{|Y_p|}.$$
In this fraction, both cardinalities are interpreted as integers via the embedding $\iota:\mathbb N\to\mathbb Z$ given by $\iota(n)=[(n,0)]$.

## Definition references

[[def-euler-prime-classes]]

[[def-euler-hurwitz-projective-reduction]]

[[def-euler-hurwitz-torus-normalizer]]

[[math:def-group]]

[[math:def-subgroup]]

[[math:def-coset]]

[[math:def-subset-and-proper-subset]]

[[math:def-function]]

[[math:def-finite-cardinality]]

[[math:def-rationals]]

[[math:def-cartesian-product]]

[[math:def-complex-numbers-and-arithmetic]]

[[math:lem-nat-embeds-int]]

## Facts & Assumptions

[F1] For the fixed projective reduction at $p\in\mathcal P_3$, $\Gamma_p$ is a subgroup of $G_p$ and $Y_p$ is a nonempty finite set of right cosets. [[def-euler-hurwitz-projective-reduction]]

[F2] In that same reduction $K_p=N_{G_p}(C_p)$ is a subgroup of $G_p$. [[def-euler-hurwitz-torus-normalizer]]

[F3] Group multiplication is closed and associative and has a two-sided identity. A subgroup has the ambient identity and is closed under products and inverses. The right coset represented by $g$ is the set of products $\gamma g$ with $\gamma$ in the subgroup. [[math:def-group]] [[math:def-subgroup]] [[math:def-coset]]

[F4] A membership condition within a set determines a unique subset. A subset of $A\times B$ with exactly one pair $(a,b)$ for each $a\in A$ defines a function $A\to B$. [[math:def-subset-and-proper-subset]] [[math:def-function]] [[math:def-cartesian-product]]

[F5] A subset of a finite set is finite. Every finite set has a unique natural number as its cardinality, and that cardinality is zero exactly for the empty set. A fraction of integers with nonzero denominator denotes a rational number. [[math:thm-subset-of-a-finite-set]] [[math:def-finite-cardinality]] [[math:def-rationals]]

[F6] For sets $A$ and $B$, the Cartesian product $A\times B$ consists of exactly the ordered pairs $(a,b)$ with $a\in A$ and $b\in B$. [[math:def-cartesian-product]]

[F7] The complex numbers contain the constant classes of the real numbers $0$ and $1$, written $0$ and $1$ in $\mathbb C$. [[math:def-complex-numbers-and-arithmetic]]

[F8] The map $\iota(n)=[(n,0)]$ from the naturals to the integers is injective. It sends natural zero to integer zero $[(0,0)]$. [[math:lem-nat-embeds-int]] [[math:def-int-operations]]

## Justification

The domain of right translation consists of the pairs in $Y_p\times K_p$, and the rule must give the same output coset for every representative of its first coordinate. Once the orbit is fixed as a subset of the finite coset set, its membership determines which of the two complex constants the indicator takes. The nonempty ambient set supplies a nonzero natural cardinality whose integer image is the denominator of the density.

## Proof

**Given:** $p\in\mathcal P_3$ and the fixed projective reduction and its normalizer subgroup from [F1] and [F2].

**Goal:** Verify the right action and the definitions of $\mathcal O_p$, $f_p$ and $\mu_p$.

1.1 For $\Gamma_p g\in Y_p$ and $k\in K_p$, the product $gk$ lies in $G_p$, so $\Gamma_p(gk)\in Y_p$. By associativity, $\Gamma_p(gk)=\{(\gamma g)k:\gamma\in\Gamma_p\}=\{xk:x\in\Gamma_p g\}$. This last set depends only on the coset. If two elements of $G_p$ represent the same coset, they therefore give the same translated coset. Inside $(Y_p\times K_p)\times Y_p$, take the subset of pairs $((y,k),z)$ with $y=\Gamma_p g$ and $z=\Gamma_p(gk)$ for some $g\in G_p$. The existence and representative independence just proved give exactly one such $z$ for each input $(y,k)\in Y_p\times K_p$, so this subset is the graph of the stated function. [F1, F2, F3, F4, F6]

2.1 Right translation by $e$ gives $\Gamma_p(ge)=\Gamma_p g$. For $k_1,k_2\in K_p$, the product $k_1k_2$ lies in $K_p$ and translating successively gives $\Gamma_p((gk_1)k_2)=\Gamma_p(g(k_1k_2))$. These are the right action laws. At the base coset, translation by $k$ gives $\Gamma_p(ek)=\Gamma_p k$. Thus $\mathcal O_p$ consists of exactly those $y\in Y_p$ equal to $\Gamma_p k$ for some $k\in K_p$. This membership condition determines a unique subset of $Y_p$, which contains $\Gamma_p$ by taking $k=e$. [F2, F3, F4, step 1.1]

3.1 For each coset $y\in Y_p$, exactly one of $y\in\mathcal O_p$ and $y\notin\mathcal O_p$ holds. In $Y_p\times\mathbb C$, take the subset of pairs $(y,z)$ with $y\in\mathcal O_p$ and $z=1$, or with $y\notin\mathcal O_p$ and $z=0$. Both constants belong to $\mathbb C$ by [F7], so this graph gives exactly one complex value for each coset and defines $f_p$. [F1, F4, F6, F7, step 2.1]

4.1 By [F1] and step 2.1, $\mathcal O_p$ is a subset of the nonempty finite set $Y_p$. By [F5], the orbit is finite and both cardinalities are natural numbers, with $|Y_p|\ne0$ because $Y_p$ is nonempty. The embedding in [F8] makes both entries integers and gives $\iota(|Y_p|)\ne\iota(0)=0$ by injectivity. The displayed fraction therefore defines a unique rational number. This completes the justification of the orbit, its indicator and its density. [F1, F5, F8, step 2.1, step 3.1] ∎
