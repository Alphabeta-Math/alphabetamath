---
id: lem-euler-hurwitz-adelic-identification
kind: lemma
title: The finite adelic quotient and its stabilizer
status: draft
domain: mathematics
deps:
  - math:def-subgroup
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-finite-quaternion-adeles-and-projective-units
  - def-euler-hurwitz-adelic-level
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - math:def-double-cosets-of-two-subgroups
  - thm-hurwitz-order-integral-structure
  - def-author-6f52147f3ab3-finite-quaternion-ideles
  - def-author-291c0ff6bd53-quaternion-right-ideal-classes
  - thm-adelic-right-ideal-dictionary
  - cor-euler-hurwitz-right-class-number
  - lem-projective-integral-stabilizer-over-rationals
formulation_deps:
  - math:def-subgroup
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-finite-quaternion-adeles-and-projective-units
  - def-euler-hurwitz-adelic-level
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - math:def-double-cosets-of-two-subgroups
argument_deps:
  - math:def-subgroup
  - def-euler-prime-classes
  - def-euler-hamilton-quaternions
  - def-euler-hurwitz-order
  - def-author-6f52147f3ab3-hamilton-order-completions
  - def-finite-quaternion-adeles-and-projective-units
  - def-euler-hurwitz-adelic-level
  - thm-hurwitz-integral-splitting-at-odd-primes
  - def-euler-hurwitz-projective-reduction
  - math:def-coset
  - math:def-double-cosets-of-two-subgroups
  - thm-hurwitz-order-integral-structure
  - def-author-6f52147f3ab3-finite-quaternion-ideles
  - def-author-291c0ff6bd53-quaternion-right-ideal-classes
  - thm-adelic-right-ideal-dictionary
  - cor-euler-hurwitz-right-class-number
  - lem-projective-integral-stabilizer-over-rationals
dependency_roles:
  math:def-subgroup: mathematical-premise
  def-euler-prime-classes: mathematical-premise
  def-euler-hamilton-quaternions: mathematical-premise
  def-euler-hurwitz-order: mathematical-premise
  def-author-6f52147f3ab3-hamilton-order-completions: mathematical-premise
  def-finite-quaternion-adeles-and-projective-units: mathematical-premise
  def-euler-hurwitz-adelic-level: mathematical-premise
  thm-hurwitz-integral-splitting-at-odd-primes: mathematical-premise
  def-euler-hurwitz-projective-reduction: mathematical-premise
  math:def-coset: mathematical-premise
  math:def-double-cosets-of-two-subgroups: mathematical-premise
  thm-hurwitz-order-integral-structure: mathematical-premise
  def-author-6f52147f3ab3-finite-quaternion-ideles: mathematical-premise
  def-author-291c0ff6bd53-quaternion-right-ideal-classes: mathematical-premise
  thm-adelic-right-ideal-dictionary: mathematical-premise
  cor-euler-hurwitz-right-class-number: mathematical-premise
  lem-projective-integral-stabilizer-over-rationals: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 3, Lemma 3.2, equation (3.5) and the following paragraph
      reading_limits: Attribution for the identification and stabilizer claim in the
        two opening paragraphs of the proof of Lemma 3.2 on PDF page 3.
dependency_level: 6
---

## Statement

Let $p\in\mathcal P_3$, the primes congruent to $3$ modulo $4$. Let $B$ be the rational Hamilton quaternion algebra, with basis $1,i,j,k$ and products $i^2=j^2=-1$ and $ij=k=-ji$. Its Hurwitz order $\mathcal H$ is the subring with four coordinates all in $\mathbb Z$ or all in $\mathbb Z+\tfrac12$ in that basis. At each prime $\ell$, let $B_\ell$ be the same algebra over the $\ell$-adic field $\mathbb Q_\ell$ and $\mathcal H_\ell$ the span of $\mathcal H$ over the $\ell$-adic integers $\mathbb Z_\ell$ in $B_\ell$. Write $R^\times$ for the elements of a ring $R$ with two-sided multiplicative inverses.

Write $G=PB^\times$ for the projective quaternion unit group. Its rational group is $G(\mathbb Q)=B^\times/\mathbb Q^\times$, whose classes identify rational quaternion units differing by nonzero rational scalar multiplication. At a prime $\ell$ the local group is $G(\mathbb Q_\ell)=B_\ell^\times/\mathbb Q_\ell^\times$, with the same convention over $\mathbb Q_\ell$. Put $K_\ell=\operatorname{im}(\mathcal H_\ell^\times\to G(\mathbb Q_\ell))$ and $K=\prod_\ell K_\ell$. The group $G(\mathbb A_f)$ of finite adelic projective units consists of tuples of local classes belonging to $K_\ell$ at all but finitely many primes, with componentwise multiplication. View $G(\mathbb Q)$ inside it by assigning a rational class its local classes at every prime.

Use the same integral splitting at $p$ for the local reduction $r_p:K_p\to G_p$ and the reduction $\rho_p$ on $\mathcal H^\times$. This splitting identifies $B_p$ with the algebra of two-by-two matrices over $\mathbb Q_p$ and $\mathcal H_p$ with the ring of two-by-two matrices over $\mathbb Z_p$. The group $G_p=\mathrm{PGL}_2(\mathbb F_p)$ consists of the classes of invertible two-by-two matrices over $\mathbb F_p=\mathbb Z/p\mathbb Z$ up to nonzero scalar multiplication, with the product induced by matrix multiplication. The map $r_p$ takes an integral invertible matrix representative to the projective class of its entrywise reduction modulo $p$. Write $U(p)$ for the subgroup of $K$ whose $p$-component reduces to the identity, $\Gamma_p=\rho_p(\mathcal H^\times)$ for the image of the Hurwitz units, and $Y_p=\Gamma_p\backslash G_p$ for the set of right cosets $\Gamma_p g=\{\gamma g:\gamma\in\Gamma_p\}$.

Every double coset $G(\mathbb Q)gU(p)=\{a g u:a\in G(\mathbb Q),\ u\in U(p)\}$ has a representative $k\in K$, called an integral representative. There is a bijection
$$G(\mathbb Q)\backslash G(\mathbb A_f)/U(p)\longrightarrow Y_p,\qquad G(\mathbb Q)kU(p)\longmapsto \Gamma_p r_p(k_p).$$
If a rational quaternion $b\in B^\times$ relates integral representatives by $k'=[b]ku$ for $k,k'\in K$ and $u\in U(p)$, there is a nonzero rational $c$ with $cb\in\mathcal H^\times$. The subgroup of rational classes preserving $K$ by left multiplication is $G(\mathbb Q)\cap K$. Its image under $k\mapsto r_p(k_p)$ is precisely $\Gamma_p$.

## Statement references

[[def-euler-prime-classes]]

[[def-euler-hamilton-quaternions]]

[[def-euler-hurwitz-order]]

[[def-author-6f52147f3ab3-hamilton-order-completions]]

[[def-finite-quaternion-adeles-and-projective-units]]

[[def-euler-hurwitz-adelic-level]]

[[thm-hurwitz-integral-splitting-at-odd-primes]]

[[def-euler-hurwitz-projective-reduction]]

[[math:def-subgroup]]

[[math:def-coset]]

[[math:def-double-cosets-of-two-subgroups]]

## Facts & Assumptions

[F1] The prime condition $p\equiv3\pmod4$ makes $p$ odd. In the rational Hamilton algebra described above, the Hurwitz order is the integer span of the rational basis $1,i,j,(-1+i+j+k)/2$. It is a maximal order, in particular a unital subring that is a full integral lattice in $B$. [[def-euler-prime-classes]] [[def-euler-hamilton-quaternions]] [[def-euler-hurwitz-order]] [[thm-hurwitz-order-integral-structure]]

[F2] The local algebra $B_\ell$ extends the Hamilton products to the field $\mathbb Q_\ell$, the completion of $\mathbb Q$ for the distance given by the $\ell$-adic absolute value. This absolute value sends a nonzero rational to $\ell^{-v}$, where $v$ is the exponent of $\ell$ in its numerator minus that in its denominator. The absolute value of $0$ is $0$. The ring $\mathbb Z_\ell$ is the closed unit ball $\{x\in\mathbb Q_\ell:|x|_\ell\le1\}$ and the local order is the span specified above. The diagonal map sends the rational projective group injectively into the finite adelic group of tuples, and $K$ is the image of $\prod_\ell\mathcal H_\ell^\times$ in that group. Both the diagonal image and $K$ are subgroups of $G(\mathbb A_f)$. [[def-author-6f52147f3ab3-hamilton-order-completions]] [[def-finite-quaternion-adeles-and-projective-units]]

[F3] By [F1], the odd-prime integral splitting theorem applies to the Hurwitz order at $p$. It gives an isomorphism from $B_p$ to $M_2(\mathbb Q_p)$ carrying $\mathcal H_p$ onto $M_2(\mathbb Z_p)$. Use the same splitting for both reductions. This identifies $K_p$ with the invertible matrices over $\mathbb Z_p$ modulo unit scalar matrices. The map $r_p$ preserves products and is onto $G_p$. Its composition with the local projective class map on $\mathcal H^\times$ equals $\rho_p$. The image $\Gamma_p=\rho_p(\mathcal H^\times)$ is a subgroup of $G_p$ because the reduction on Hurwitz units preserves products, the identity and inverses. The prescribed level has all factors $K_\ell$ for $\ell\ne p$ and at $p$ consists of classes with identity image under $r_p$. [[thm-hurwitz-integral-splitting-at-odd-primes]] [[def-euler-hurwitz-adelic-level]] [[def-euler-hurwitz-projective-reduction]]

[F4] A subgroup contains the ambient identity and is closed under products and inverses. For a subgroup $H$ of a group, the right coset $Hg$ consists of $hg$ with $h\in H$. In particular $Hg'=Hg$ exactly when $g'=hg$ for some $h\in H$. The identity gives $g'=1g'\in Hg'$, so equality puts $g'$ in $Hg$. Conversely $g'=hg$ implies $Hg'=(Hh)g=Hg$, since right multiplication by $h$ maps $H$ onto itself with inverse right multiplication by $h^{-1}$. [[math:def-subgroup]] [[math:def-coset]]

[F5] For an order $O$ that is the integer span of a rational basis of $B$, write $\widehat B^\times$ for the tuples of local quaternion units that lie in $O_\ell^\times$ for all but finitely many $\ell$, and $\widehat O^\times=\prod_\ell O_\ell^\times$. A locally principal right fractional $O$-ideal is a full integer span of a rational basis of $B$ that is stable under right multiplication by $O$ and whose local span at each $\ell$ is $x_\ell O_\ell$ for some $x_\ell\in B_\ell^\times$. The right ideal class set is the quotient of these ideals by $I\sim J$ if $J=bI$ for some $b\in B^\times$. The dictionary identifies this set with $B^\times\backslash\widehat B^\times/\widehat O^\times$, sending the identity double coset to the class of $O$. For $O=\mathcal H$, projection by scalar classes then induces a bijection from these double cosets to $G(\mathbb Q)\backslash G(\mathbb A_f)/K$. [[def-author-6f52147f3ab3-finite-quaternion-ideles]] [[def-author-291c0ff6bd53-quaternion-right-ideal-classes]] [[thm-adelic-right-ideal-dictionary]]

[F6] For $O=\mathcal H$ the right ideal class set has the sole class $[\mathcal H]$. [[cor-euler-hurwitz-right-class-number]]

[F7] For an order $O$ in the rational Hamilton algebra, if the rational class of $b\in B^\times$ has a local representative in $O_\ell^\times$ at every prime $\ell$, there exists $c\in\mathbb Q^\times$ with $cb\in O^\times$. Conversely, every element of $O^\times$ has its local classes in the images of the local unit groups at all primes. [[lem-projective-integral-stabilizer-over-rationals]]

[F8] For subgroups $D,U$ of a group $M$, the double coset $DgU$ consists of the products $agu$ with $a\in D$ and $u\in U$. [[math:def-double-cosets-of-two-subgroups]]

## Proof

**Given:** $B,\mathcal H,p,G,K,U(p)$ as in the Statement, with a single choice of the integral splitting at $p$ for both reductions.

**Goal:** Identify the double coset set with $Y_p$ by the displayed map and verify the rescaling claim and the residual action at $p$.

1.1 By [F1], the dictionary in [F5] applies to $O=\mathcal H$. By [F6] the double coset set $B^\times\backslash\widehat B^\times/\widehat{\mathcal H}^\times$ has one element. Under the scalar projection of [F5], its sole element maps to the identity double coset $G(\mathbb Q)K$ by [F2]. Thus every $g\in G(\mathbb A_f)$ is $ak$ with $a\in G(\mathbb Q)$ and $k\in K$. It follows that every double coset modulo $U(p)$ on the right can be represented by an element of $K$. [F1, F2, F5, F6, F8]

1.2 Put $R(k)=r_p(k_p)$ for $k\in K$. This preserves products because multiplication is componentwise and $r_p$ preserves products. An arbitrary element of $G_p$ lifts under $r_p$ to a $p$-component in $K_p$, and adjoining identity components at all other primes gives a lift under $R$. Thus $R$ is onto. The set of elements sent to the identity is exactly $U(p)$ by the factor descriptions in [F3]. [F2, F3]

2.1 A rational class preserves $K$ by left multiplication exactly when it belongs to $G(\mathbb Q)\cap K$, since left multiplication by $a$ sends the identity to $a$, and each element of $K$ multiplies $K$ onto itself. Take any $a\in G(\mathbb Q)\cap K$ and choose a representative $b\in B^\times$ of $a$. Every local class of $b$ belongs to $K_\ell$. Apply [F7] with $O=\mathcal H$ to find $c\in\mathbb Q^\times$ with $cb\in\mathcal H^\times$. By [F3], $R(a)=\rho_p(cb)$. Conversely, every Hurwitz unit represents a rational class in $K$ by [F7] and gives its $\rho_p$-image under $R$. Thus $R(G(\mathbb Q)\cap K)=\Gamma_p$. [F1, F2, F3, F4, F7, step 1.2]

3.1 Take $k,k'\in K$ in the same double coset. Since $k'\in G(\mathbb Q)k'U(p)$ by the subgroup identities, equality of the double cosets of $k$ and $k'$ puts $k'$ in $G(\mathbb Q)kU(p)$. By [F8], $k'=aku$ for some $a\in G(\mathbb Q)$ and $u\in U(p)$. Then $a=k'u^{-1}k^{-1}\in K$ by the subgroup laws in [F4], since $K$ contains $U(p)$. For a specified relation $k'=[b]ku$, the same calculation puts $[b]$ in $G(\mathbb Q)\cap K$, so step 2.1 gives a rational rescaling of $b$ into $\mathcal H^\times$. By step 2.1, $R(a)\in\Gamma_p$. Since $u\in U(p)=\ker R$, we have $R(k')=R(a)R(k)$. Since $\Gamma_p$ is a subgroup by [F3], the right coset criterion in [F4] gives $\Gamma_pR(k')=\Gamma_pR(k)$. This proves that the map is well defined. [F2, F3, F4, F8, step 1.2, step 2.1]

4.1 Conversely, assume $\Gamma_pR(k')=\Gamma_pR(k)$ with $k,k'\in K$. By [F4] applied to the subgroup $\Gamma_p$ of [F3], there is $\gamma\in\Gamma_p$ with $R(k')=\gamma R(k)$. By step 2.1 there is $a\in G(\mathbb Q)\cap K$ with $R(a)=\gamma$. The element $u=(ak)^{-1}k'$ lies in $K$ and satisfies $R(u)=R(ak)^{-1}R(k')=1$. Hence $u\in U(p)$ and $k'=aku$. Since $a\in G(\mathbb Q)$ and $u\in U(p)$, multiplication by $a$ on the right permutes $G(\mathbb Q)$ and multiplication by $u$ on the left permutes $U(p)$. Thus $G(\mathbb Q)k'U(p)=G(\mathbb Q)kU(p)$ by the product description in [F8]. This proves injectivity of the map. Surjectivity follows because $R$ is onto and any lift $k\in K$ represents a double coset. Together with steps 1.1 and 3.1 this proves the bijection. Steps 2.1 and 3.1 prove the stabilizer and rescaling claims. [F3, F4, F8, step 1.1, step 1.2, step 2.1, step 3.1] ∎
