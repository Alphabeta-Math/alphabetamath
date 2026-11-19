---
title: Eight representatives in the normalizer per qualifying left-unit class
status: draft
research_item: lem-euler-hurwitz-normalizer-unit-count
dependency_level: 8
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 4, §3.3, class multiplicity preceding (3.6)
      reading_limits: Checked the multiplicity sentence and its surrounding
        definitions on PDF page 4 for attribution.
---

PDF p. 4: ` §3.3, class multiplicity preceding (3.6) `

## Prerequisites

- [def-euler-prime-classes](item-def-euler-prime-classes)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)
- [def-euler-hurwitz-order](item-def-euler-hurwitz-order)
- [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)
- [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)
- [math:def-group](https://alphabetamath.cc/item/def-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-group-action](https://alphabetamath.cc/item/def-group-action)
- [math:def-free-group-action](https://alphabetamath.cc/item/def-free-group-action)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)
- [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)
- [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)
- [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)
- [math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)
- [math:def-coset](https://alphabetamath.cc/item/def-coset)
- [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)
- [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)
- [lem-euler-hurwitz-units-in-normalizer](item-lem-euler-hurwitz-units-in-normalizer)
- [lem-euler-hurwitz-quotient-size](item-lem-euler-hurwitz-quotient-size)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-equivalence-relation](https://alphabetamath.cc/item/def-equivalence-relation)
- [math:def-function](https://alphabetamath.cc/item/def-function)


## Statement

Let $m>0$ be an odd integer, meaning $m=2r+1$ for some integer $r$. Let $p\in\mathcal P_3$, the set of primes congruent to $3$ modulo $4$, and suppose $p\nmid m$. A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself. Here $p\equiv3\pmod 4$ means $4$ divides $p-3$, and $p\nmid m$ means there is no integer $s$ with $m=ps$.

Write $B$ for the rational Hamilton quaternion algebra. Its elements have unique expressions $a+bi+cj+dk$ with rational coefficients, and multiplication is associative and determined by $i^2=j^2=-1$, $ij=k=-ji$, distributivity and commutation with rational scalars. Let $\mathcal H$ be the Hurwitz order, the subring of $B$ consisting of quaternions whose coordinates are all integers or all integers plus $\tfrac12$. The reduced norm is $N(a+bi+cj+dk)=a^2+b^2+c^2+d^2$. The norm shell is $Q_m=\{\alpha\in\mathcal H:N(\alpha)=m\}$. Write $\mathcal H^\times$ for the units, the elements of $\mathcal H$ with a two-sided inverse in $\mathcal H$. The left-unit class of $\alpha\in Q_m$ is the set $\mathcal H^\times\alpha=\{u\alpha:u\in\mathcal H^\times\}$. A representative of such a class is any of its elements.

Let $\mathbb F_p$ be the field of integer residues modulo $p$, where integers represent the same residue if their difference is a multiple of $p$. Let $G_p$ be the group of projective classes of invertible two-by-two matrices over $\mathbb F_p$, with matrices identified up to nonzero scalar multiples and products taken on representatives. Its identity $e$ is the class of the identity matrix. Use the fixed projective reduction $\rho_p(x)$ for $x\in\mathcal H$ with $p\nmid N(x)$. It is the class of the matrix assigned to the residue of $x$ under the fixed identification of $\mathcal H/p\mathcal H$ with the two-by-two matrix algebra over $\mathbb F_p$. Here two quaternions have the same residue when their difference lies in $p\mathcal H=\{ph:h\in\mathcal H\}$.

Write $\Gamma_p=\{\rho_p(u):u\in\mathcal H^\times\}$ for the subgroup of unit images. A subgroup contains the group identity and is closed under products and inverses. Let $C_p$ be the subgroup of projective classes of the matrices of the nonzero residues $a+b\bar i$ with $a,b\in\mathbb F_p$ and $\bar i$ the residue of $i$. Write $K_p=\{g\in G_p:gC_pg^{-1}=C_p\}$ for its normalizer, where $gC_pg^{-1}=\{gcg^{-1}:c\in C_p\}$. The quotient set $Y_p=\Gamma_p\backslash G_p$ consists of right cosets $\Gamma_pg=\{\gamma g:\gamma\in\Gamma_p\}$. The orbit $\mathcal O_p=\{\Gamma_pk:k\in K_p\}$ is the set of these cosets obtained by right multiplication of the identity coset $\Gamma_p$ by elements of $K_p$.

The reduction of a left-unit class represented by $\alpha$ is the coset $\Gamma_p\rho_p(\alpha)$, which is independent of the representative. Each class whose reduction lies in $\mathcal O_p$ has exactly eight representatives $\beta$ with $\rho_p(\beta)\in K_p$. A class whose reduction lies outside $\mathcal O_p$ has zero such representatives.

## Statement references

[def-euler-prime-classes](item-def-euler-prime-classes)

[math:def-prime](https://alphabetamath.cc/item/def-prime)

[math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)

[def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions)

[def-euler-hurwitz-order](item-def-euler-hurwitz-order)

[def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell)

[lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)

[math:def-group](https://alphabetamath.cc/item/def-group)

[math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[math:def-group-action](https://alphabetamath.cc/item/def-group-action)

[math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)

[math:thm-z-mod-p-is-a-field](https://alphabetamath.cc/item/thm-z-mod-p-is-a-field)

[def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction)

[def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer)

[math:def-normalizer-of-a-subgroup](https://alphabetamath.cc/item/def-normalizer-of-a-subgroup)

[math:def-coset](https://alphabetamath.cc/item/def-coset)

[def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)

[math:def-equivalence-relation](https://alphabetamath.cc/item/def-equivalence-relation)

[math:def-function](https://alphabetamath.cc/item/def-function)

## Facts & Assumptions

[F1] Multiplication in $B$ is associative. The Hurwitz order contains $1$ and is closed under products in $B$. Membership in $Q_m$ means belonging to the order with reduced norm $m$. In $B$, $N(xy)=N(x)N(y)$ and every element with nonzero norm has a two-sided inverse in $B$. [def-euler-hamilton-quaternions](item-def-euler-hamilton-quaternions) [def-euler-hurwitz-order](item-def-euler-hurwitz-order) [def-euler-hurwitz-norm-shell](item-def-euler-hurwitz-norm-shell) [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)

[F2] The Hurwitz units form a group with the inherited multiplication. Each has norm $1$. In particular the eight coordinate units $\pm1,\pm i,\pm j,\pm k$, with both signs at each basis element, are eight distinct members of this group. [lem-euler-hurwitz-unit-list](item-lem-euler-hurwitz-unit-list)

[F3] A group has associative multiplication, a two-sided identity and a two-sided inverse for each element. A left action is a rule $(u,\alpha)\mapsto u\cdot\alpha$ with $1\cdot\alpha=\alpha$ and $(uv)\cdot\alpha=u\cdot(v\cdot\alpha)$. A left action is free if, for each point $\alpha$, the only group element fixing $\alpha$ is the identity. [math:def-group](https://alphabetamath.cc/item/def-group) [math:def-group-action](https://alphabetamath.cc/item/def-group-action) [math:def-free-group-action](https://alphabetamath.cc/item/def-free-group-action)

[F4] For the stated $p$, projective reduction is defined on elements of $\mathcal H$ with norm not divisible by $p$, preserves products there, and sends $1$ to $e$. The unit images form the subgroup $\Gamma_p$. The construction of $C_p$ gives the subgroup $K_p$ specified in the Statement. A subgroup is closed under products and inverses. [def-euler-hurwitz-projective-reduction](item-def-euler-hurwitz-projective-reduction) [def-euler-hurwitz-torus-normalizer](item-def-euler-hurwitz-torus-normalizer) [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)

[F5] For a right coset $\Gamma_p g$ the defining set consists of the products $\gamma g$ with $\gamma\in\Gamma_p$. Hence $g\in\Gamma_p g$, and if $h=\gamma g$ with $\gamma\in\Gamma_p$, then $\Gamma_p h=\Gamma_p g$, since right multiplication by $\gamma$ permutes $\Gamma_p$ with inverse right multiplication by $\gamma^{-1}$. The orbit consists exactly of the cosets $\Gamma_p k$ with $k\in K_p$. [math:def-coset](https://alphabetamath.cc/item/def-coset) [def-euler-hurwitz-normalizer-orbit](item-def-euler-hurwitz-normalizer-orbit)

[F6] For the same projective reduction and $p\in\mathcal P_3$, the intersection $\Gamma_p\cap K_p$ consists of the four distinct classes of $1,i,j,k$. For a unit $w$, $\rho_p(w)=e$ holds exactly when $w=1$ or $w=-1$, since the projective identity is the class of nonzero scalar matrices and the only units with scalar reduction are $1,-1$. [lem-euler-hurwitz-units-in-normalizer](item-lem-euler-hurwitz-units-in-normalizer) [lem-euler-hurwitz-quotient-size](item-lem-euler-hurwitz-quotient-size) [def-degree-two-projective-linear-group](item-def-degree-two-projective-linear-group)

[F7] A bijection is a function which is one-to-one and onto. The cardinality of a finite set is the length of a listing of all its elements without repetition. Composing such a listing with a bijection gives a listing of the same length without repetition. [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[F8] A reflexive, symmetric and transitive relation on a set is an equivalence relation. The equivalence class of $\alpha$ consists of all elements related to $\alpha$. [math:def-equivalence-relation](https://alphabetamath.cc/item/def-equivalence-relation)

[F9] A rule defines a function from one set to another when it assigns each element of the first set exactly one value in the second set. [math:def-function](https://alphabetamath.cc/item/def-function)

## Justification

Step 1.1 identifies $\mathcal H^\times\alpha$ with the equivalence class of $\alpha$ under the relation of differing by left multiplication by a unit. Step 2.1 shows that the representative can vary while the right coset stays the same, so the reduction has a unique value in $Y_p$ for every class.

## Proof

**Given:** A positive odd $m$, a prime $p\in\mathcal P_3$ with $p\nmid m$, and the fixed projective reduction at $p$.

**Goal:** Count the elements of each left-unit class whose projective reductions belong to $K_p$.

1.1 For $u\in\mathcal H^\times$ and $\alpha\in Q_m$, the product $u\alpha$ lies in $\mathcal H$ and has norm $N(u)N(\alpha)=m$. Thus multiplication on the left gives an action on $Q_m$, since $1\alpha=\alpha$ and $(uv)\alpha=u(v\alpha)$. Differing by left multiplication by a unit is reflexive by $1$, symmetric by the inverse of a unit, and transitive by the product of units. The equivalence class of $\alpha$ is therefore $\mathcal H^\times\alpha$, because its elements are precisely the $\beta=u\alpha$ for units $u$. If $\beta$ lies in that class, symmetry and transitivity show that an element is related to $\alpha$ exactly when it is related to $\beta$, so the two classes coincide. For any $\alpha\in Q_m$ the norm $m$ is nonzero, so $\alpha$ has an inverse in $B$. If $w\alpha=\alpha$, right multiplication by $\alpha^{-1}$ gives $w=1$, so the action is free. If $u\alpha=v\alpha$, then $(v^{-1}u)\alpha=v^{-1}(v\alpha)=\alpha$ by the action laws. Freeness gives $v^{-1}u=1$, hence $u=v$. [F1, F2, F3, F8]

2.1 Projective reduction is defined on every element of $Q_m$ because $p\nmid m$, and it is defined on every Hurwitz unit since its norm is $1$. Fix a class $\mathcal H^\times\alpha$ and put $g=\rho_p(\alpha)$. For any representative $\beta=u\alpha$, multiplicativity gives $\rho_p(\beta)=\rho_p(u)g$. Since $\rho_p(u)\in\Gamma_p$, its right coset is $\Gamma_p\rho_p(\beta)=\Gamma_p g$. Each class therefore determines a single coset in $Y_p$, giving a function from the set of left-unit classes to $Y_p$. [given, F1, F2, F4, F5, F9, step 1.1]

3.1 If some representative reduces to an element of $K_p$, then its coset belongs to $\mathcal O_p$ by the orbit formula. Conversely, if $\Gamma_pg\in\mathcal O_p$, there is $h\in K_p$ with $\Gamma_p h=\Gamma_pg$. Since $h\in\Gamma_p h$, the equality gives $h=\gamma g$ for some $\gamma\in\Gamma_p$. By the definition of $\Gamma_p$ there is a unit $v$ with $\rho_p(v)=\gamma$. The element $\beta_0=v\alpha$ is in the class, and $\rho_p(\beta_0)=h\in K_p$. [F4, F5, step 1.1, step 2.1]

4.1 In a class with such a representative $\beta_0$, every element is $u\beta_0$ for a unique Hurwitz unit $u$: the class relation gives existence, and the injectivity proved from freeness in step 1.1 gives uniqueness. Since $\rho_p(u\beta_0)=\rho_p(u)\rho_p(\beta_0)$ and $\rho_p(\beta_0)\in K_p$, closure of $K_p$ under products gives $\rho_p(u\beta_0)\in K_p$ whenever $\rho_p(u)\in\Gamma_p\cap K_p$. Conversely, if $\rho_p(u\beta_0)\in K_p$, multiply it on the right by $\rho_p(\beta_0)^{-1}\in K_p$ to obtain $\rho_p(u)\in K_p$. This image is always in $\Gamma_p$ because $u$ is a unit. [F2, F3, F4, step 1.1, step 3.1]

5.1 If $\rho_p(u)\in\Gamma_p\cap K_p$, there is $q\in\{1,i,j,k\}$ with $\rho_p(u)=\rho_p(q)$. Reduction sends the inverse of a unit to the inverse of its image, by applying it to the two inverse equations. Hence $\rho_p(q^{-1}u)=e$. The scalar-reduction criterion gives $q^{-1}u=1$ or $-1$, so $u=q$ or $-q$. Conversely, for each of the four possible $q$, both $q$ and $-q=q(-1)$ reduce to $\rho_p(q)$ since $\rho_p(-1)=e$. Their images lie in the intersection. Thus the units meeting the condition in step 4.1 are exactly the eight distinct coordinate units. [F2, F3, F4, F6, step 4.1]

6.1 For each of the eight units $u$, the product $u\beta_0$ is a single qualifying representative, so multiplication on the right by $\beta_0$ defines a function to the set of representatives reducing into $K_p$. Each qualifying representative has exactly one preimage by step 4.1, so this function is a bijection. Therefore there are exactly eight such representatives if the class reduces into $\mathcal O_p$. The first implication of step 3.1 gives zero if it reduces outside $\mathcal O_p$. [F7, F9, step 3.1, step 4.1, step 5.1] ∎
