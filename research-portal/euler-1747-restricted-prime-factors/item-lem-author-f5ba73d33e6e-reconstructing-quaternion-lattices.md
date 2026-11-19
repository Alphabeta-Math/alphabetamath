---
title: Reconstructing a quaternion lattice from its finite completions
status: published
research_item: lem-author-f5ba73d33e6e-reconstructing-quaternion-lattices
dependency_level: 2
---

## Prerequisites

- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm)
- [def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions)
- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)


## Statement

In the rational Hamilton algebra $B=B(\mathbb Q)$, fix a full integral lattice $L$, the integer span of a rational basis of $B$. At each prime $\ell$, use the local Hamilton space $B_\ell=B(\mathbb Q_\ell)$ and embed $B$ into it by including each rational coefficient in $\mathbb Q_\ell$. The completion $L_\ell$ is the span of $L$ over the $\ell$-adic integers $\mathbb Z_\ell$. Let $J_\ell\subseteq B_\ell$ be the $\mathbb Z_\ell$-span of a $\mathbb Q_\ell$-basis, meaning four vectors in which each element of $B_\ell$ has a unique expression with coefficients in $\mathbb Q_\ell$. Assume $J_\ell=L_\ell$ for all but finitely many $\ell$.

The set $M=\{b\in B:b\in J_\ell\text{ for every prime }\ell\}$ is the unique full integral lattice with $M_\ell=J_\ell$ for every $\ell$. Every full integral lattice $A$ satisfies $A=\{b\in B:b\in A_\ell\text{ for every prime }\ell\}$ and $A_\ell=L_\ell$ for all but finitely many $\ell$.

## Statement references

[def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm)

[def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions)

[def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)

## Facts & Assumptions

[F1] A rational lattice basis remains a basis over $\mathbb Q_\ell$. Its $\mathbb Z_\ell$-span is the completion and is the closure of the rational lattice for convergence in those basis coordinates ([def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions)).

[F2] The normalized valuation $v_\ell$ on $\mathbb Q_\ell$ is additive on products of nonzero scalars. A scalar belongs to $\mathbb Z_\ell$ if its valuation is nonnegative, with zero included, and is a unit exactly at valuation zero. Here $\mathbb Q_\ell$ is the completion of $\mathbb Q$ for the absolute value $\ell^{-v_\ell(\cdot)}$ on nonzero rationals, with absolute value zero at zero. For nonzero rationals the valuation is the numerator exponent minus the denominator exponent ([def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)).

[F3] Positive integers factor uniquely into primes, including the empty product for $1$ ([math:thm-fundamental-theorem-of-arithmetic](https://alphabetamath.cc/item/thm-fundamental-theorem-of-arithmetic)).

[F4] Pull a nonempty set of positive integers back along the canonical embedding of the natural numbers into the integers. The embedding is one-to-one, has image the nonnegative integers, and preserves and reflects order. Well-ordering gives a least natural number in the inverse image, and its integer image is the least member of the original set. ([math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int), [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)).

[F5] Division of an integer by a positive integer has an integer remainder at least zero and less than the divisor ([math:thm-division-algorithm-in-z](https://alphabetamath.cc/item/thm-division-algorithm-in-z)).

## Proof

**Given:** The reference lattice $L$ and the family of local spans $J_\ell$ in the statement.

**Goal:** Reconstruct the unique full integral lattice and establish the intersection and finite-exception properties.

1.1 A rational number belonging to every $\mathbb Z_\ell$ is an integer. For a nonzero rational number $r$, take a representation $r=a/b$ with $a\in\mathbb Z$ and the least positive integer denominator $b$, which exists by [F4]. If $b>1$, choose a prime $\ell$ dividing $b$ by [F3]. It cannot divide $a$, since cancelling it would give the smaller positive denominator $b/\ell$. Then $v_\ell(a)=0$ and $v_\ell(b)>0$, so $r\notin\mathbb Z_\ell$ by [F2]. Thus $b=1$ if $r$ belongs to every $\mathbb Z_\ell$. Zero and all other integers belong to every $\mathbb Z_\ell$. Test the coordinates of $b\in B$ in a basis of an arbitrary full integral lattice $A$. Membership in all $A_\ell$ means each of these rational coordinates belongs to every $\mathbb Z_\ell$, which gives the stated recovery of $A$. [F1, F2, F3, F4]

1.2 For an arbitrary full integral lattice $A$, clear the denominators in both changes of basis between $A$ and $L$ using one positive integer $d$. Then $dL\subseteq A$ and $dA\subseteq L$. At primes not dividing $d$, multiplication by $d$ preserves each $\mathbb Z_\ell$-span because $d$ is a scalar unit. The inclusions give $A_\ell=L_\ell$ there. [F1, F2, F3]

2.1 For each prime $\ell$ with $J_\ell\ne L_\ell$, express each basis vector of $L_\ell$ in the chosen local basis of $J_\ell$ and each basis vector of $J_\ell$ in the basis of $L_\ell$. Choose a positive integer $n_\ell$ so that multiplying these coefficients by $\ell^{n_\ell}$ puts them in $\mathbb Z_\ell$. This is possible because the nonzero entries have integer valuations and there are finitely many entries. The scaled basis vectors give $\ell^{n_\ell}L_\ell\subseteq J_\ell$ and $\ell^{n_\ell}J_\ell\subseteq L_\ell$. Put $D=\prod_{\ell:J_\ell\ne L_\ell}\ell^{n_\ell}$. At each exceptional prime $D$ is $\ell^{n_\ell}$ times a local scalar unit, and elsewhere $D$ is a local scalar unit. Thus $D L_\ell\subseteq J_\ell\subseteq D^{-1}L_\ell$ at every prime. Applying step 1.1 to $L$ gives $DL\subseteq M\subseteq D^{-1}L$. [F1, F2, F3, step 1.1]

3.1 Each $J_\ell$ contains zero and is closed under subtraction, since subtracting its linear combinations subtracts their coefficients in $\mathbb Z_\ell$. These properties hold for $M$ by the intersection condition and for $K=DM$ by scalar multiplication. By step 2.1, $D^2 L\subseteq K\subseteq L$. Also, a rational vector $w$ belongs to $K$ exactly when $w\in D J_\ell$ for every $\ell$, by dividing by $D$. In the basis of $L$, for each $j=1,\ldots,4$ consider the $j$th coordinates of elements of $K$ whose first $j-1$ coordinates vanish. The resulting coordinate set $S_j\subseteq\mathbb Z$ contains zero and is closed under subtraction, since a difference of two vectors in $K$ with those vanishing coordinates still has those coordinates zero. It thus contains every integer multiple of any of its elements, using additive inverses and repeated addition. It contains $D^2$ by taking $D^2$ times the $j$th basis vector of $L$. Let $c_j$ be its least positive integer by [F4]. For any $t\in S_j$, division by $c_j$ gives $t=qc_j+r$ with $0\le r<c_j$ by [F5]. The difference $r=t-qc_j$ lies in $S_j$, so minimality gives $r=0$. Hence $S_j=c_j\mathbb Z$. Take a vector $k_j$ of this form with $j$th coordinate $c_j$. Successively subtracting integer multiples of $k_1,\ldots,k_4$ clears every coordinate of any element of $K$. The vectors are rationally independent because the first nonzero coefficient in a rational relation would contribute a nonzero coordinate at its index. Their rational span contains $D^2L$, which spans $B$. Hence $K$ is a full integral lattice, and dividing its basis by $D$ gives a basis for $M$. [F1, F2, F4, F5, step 2.1]

4.1 Taking local spans gives $D^2L_\ell\subseteq K_\ell\subseteq D J_\ell\subseteq L_\ell$. These sets are equal at primes not dividing $D$. Fix a prime $\ell$ dividing $D$ and let $a=v_\ell(D)$ and $E=D^2/\ell^{2a}$. For $z\in D J_\ell\subseteq L_\ell$, the scalar $E$ is a unit at $\ell$, so $E^{-1}z\in L_\ell$. By the closure property in [F1], choose $y\in L$ with $y-E^{-1}z\in\ell^{2a} L_\ell$, by approximating each coordinate to distance at most $\ell^{-2a}$. Hence $Ey-z\in D^2L_\ell$. At every other prime $q$, the scalar $\ell^{2a}$ is a unit, so $Ey\in E L_q=D^2L_q\subseteq D J_q$. At $\ell$, the containment $Ey-z\in D^2L_\ell\subseteq D J_\ell$ gives $Ey\in D J_\ell$ as well. By the description of $K$ in step 3.1, $Ey\in K$. Then $z\in K_\ell$ because $Ey\in K_\ell$ and $Ey-z\in D^2L_\ell\subseteq K_\ell$. This proves $K_\ell=D J_\ell$ for every prime, so $M_\ell=J_\ell$. Uniqueness follows from step 1.1, and step 1.2 gives the asserted finite-exception property. [F1, F2, F3, step 1.1, step 1.2, step 2.1, step 3.1] ∎
