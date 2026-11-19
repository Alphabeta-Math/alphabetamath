---
title: Right ideal classes of a quaternion order
status: published
research_item: def-author-291c0ff6bd53-quaternion-right-ideal-classes
dependency_level: 4
sources:
  references:
    - title: John Voight, Quaternion Algebras, Chapter 27, Adelic framework
      url: https://link.springer.com/chapter/10.1007/978-3-030-56694-4_27
      locator: Corollary 27.6.20 (division-algebra case) and Lemma 27.6.8, with the
        setting in §§27.5.1, 27.5.4 and 27.6
      statement: The set of locally principal right fractional $O$-ideals modulo the
        relation $J=bI$ for $b\in B^\times$ is finite.
      hypotheses: $F$ is a global field, $B$ is a finite-dimensional division algebra
        over $F$, $R$ is the ring of $S$-integers for an eligible set $S$ of
        places of $F$, and $O\subseteq B$ is an $R$-order.
      reading_limits: Checked the publisher's statements for the global ring, the
        completed right ideals and their equivalence, and the finiteness
        corollary. The finiteness result is invoked without reconstructing its
        adelic proof through Fujisaki's lemma.
---

## Prerequisites

- [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm)
- [def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions)
- [def-quaternion-right-ideal-and-reduced-norm](item-def-quaternion-right-ideal-and-reduced-norm)
- [math:def-equivalence-relation](https://alphabetamath.cc/item/def-equivalence-relation)
- [math:def-power-set](https://alphabetamath.cc/item/def-power-set)
- [math:def-axiom-schema-of-separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse)
- [` John Voight, Quaternion Algebras, Chapter 27, Adelic framework · Corollary 27.6.20 (division-algebra case) and Lemma 27.6.8, with the setting in §§27.5.1, 27.5.4 and 27.6 `](https://link.springer.com/chapter/10.1007/978-3-030-56694-4_27)


## Definition

Let $O$ be an order in the rational Hamilton algebra $B$, the algebra of Hamilton quaternions with rational coordinates. An order here is a subring with identity $1$ whose elements are all the integer linear combinations of some rational basis of $B$. Write $B^\times$ for the elements of $B$ that have a two-sided multiplicative inverse.

Let $X(O)$ consist of the locally principal right fractional $O$-ideals. A right fractional $O$-ideal is the integer span of a rational basis of $B$, stable under right multiplication by $O$. It is locally principal if at each prime $\ell$ its completion $I_\ell$ is of the form $x_\ell O_\ell$ for some invertible quaternion $x_\ell$ in the local algebra $B_\ell$. Here $I_\ell$ and $O_\ell$ are the spans over the $\ell$-adic integers in the Hamilton algebra over the $\ell$-adic numbers.

For $I,J\in X(O)$ define $I\sim J$ to mean $J=bI=\{by:y\in I\}$ for some $b\in B^\times$. The right ideal class set of $O$ is the quotient set of $X(O)$ under this equivalence relation. Its elements are the classes $[I]=\{J\in X(O):I\sim J\}$. The right ideal class number is the finite cardinality of this set, so it is one precisely when there is exactly one distinct class.

## Definition references

[The Hamilton algebra and its invertible elements](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm)

[Orders and their completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions)

[Locally principal right fractional ideals](item-def-quaternion-right-ideal-and-reduced-norm)

[Equivalence classes and quotient sets](https://alphabetamath.cc/item/def-equivalence-relation)

[Finite cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

## Justification

Use the orders and local spans of [def-author-24fda87362bc-quaternion-orders-and-lattice-completions](item-def-author-24fda87362bc-quaternion-orders-and-lattice-completions) and the right ideals of [def-quaternion-right-ideal-and-reduced-norm](item-def-quaternion-right-ideal-and-reduced-norm). Apply [Separation](https://alphabetamath.cc/item/def-axiom-schema-of-separation) to the power set $\mathcal P(B)$ from [math:def-power-set](https://alphabetamath.cc/item/def-power-set), retaining the subsets of $B$ that satisfy the right fractional ideal and local principality conditions. This gives $X(O)$ as a set. It contains $O$ because $O$ is stable under its own right multiplication and $O_\ell=1O_\ell$ at every prime.

In the algebra of [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm), left multiplication by $b\in B^\times$ is rational-linear, with inverse left multiplication by $b^{-1}$. Thus if $I$ is the integer span of a rational basis, $bI$ is the integer span of the image basis. For $y\in I$ and $o\in O$, $(by)o=b(yo)\in bI$. In the local algebra the same left multiplication commutes with the local scalar coefficients. Consequently $(bI)_\ell=bI_\ell$, and if $I_\ell=x_\ell O_\ell$ then $(bI)_\ell=(bx_\ell)O_\ell$. The image of $b^{-1}$ in the local algebra is still an inverse of $b$, so $bx_\ell$ has inverse $x_\ell^{-1}b^{-1}$. This proves $bI\in X(O)$.

The identity gives $I=1I$, $J=bI$ implies $I=b^{-1}J$, and $J=bI$ and $K=cJ$ give $K=(cb)I$ with inverse $b^{-1}c^{-1}$ for $cb$. Thus the relation is reflexive, symmetric and transitive. By [math:def-equivalence-relation](https://alphabetamath.cc/item/def-equivalence-relation), the classes therefore form a quotient set.

The algebra $B$ is four-dimensional over $\mathbb Q$ by [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm), and [lem-rational-hamilton-norm-and-inverse](item-lem-rational-hamilton-norm-and-inverse) gives a two-sided inverse in $B$ for every nonzero element. Take $F=\mathbb Q$ and $S=\{\infty\}$, the set consisting of the real place. Then $R=\mathbb Z$, and $O$ is an $R$-order because it is a unital subring and a full integral lattice. The completed ideals and orders at primes of $R$ are the $\mathbb Z_\ell$-spans in the definition, and the relation is the same left multiplication by $B^\times$. Consequently Voight's corollary makes this quotient finite. By [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality), it has a unique number of elements. That number is one exactly when the quotient is a singleton.

## External input

Voight's Corollary 27.6.20 gives finiteness of the right class set of an $R$-order in a finite-dimensional division algebra over a global field, where $R$ is the ring of $S$-integers for an eligible set $S$. In Lemma 27.6.8 the class set is formed from locally principal right fractional ideals, using completions at primes of $R$, with equivalence by left multiplication by $B^\times$.
