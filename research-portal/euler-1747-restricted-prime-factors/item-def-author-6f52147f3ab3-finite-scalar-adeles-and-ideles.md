---
title: Finite scalar adeles and ideles
status: published
research_item: def-author-6f52147f3ab3-finite-scalar-adeles-and-ideles
dependency_level: 1
sources:
  references:
    - title: John Voight, Quaternion Algebras, Adelic framework
      url: https://link.springer.com/chapter/10.1007/978-3-030-56694-4_27
      locator: Chapter 27, equations (27.1.5)–(27.1.7), (27.1.17) and (27.2.2)
---

## Prerequisites

- [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball)
- [math:thm-metric-open-set-algebra](https://alphabetamath.cc/item/thm-metric-open-set-algebra)
- [math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)
- [def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)
- [math:def-topology-basis-subbasis](https://alphabetamath.cc/item/def-topology-basis-subbasis)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation)
- [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)
- [math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)
- [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)
- [math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)
- [math:thm-basis-criterion](https://alphabetamath.cc/item/thm-basis-criterion)
- [math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)
- [math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-countable](https://alphabetamath.cc/item/def-countable)
- [math:def-ring](https://alphabetamath.cc/item/def-ring)
- [math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)


## Definition

Let $\ell$ range over the primes. Use the $\ell$-adic absolute value on $\mathbb Q_\ell$ and its integer subring $\mathbb Z_\ell=\{t:|t|_\ell\le 1\}$. Give $\mathbb Q_\ell$ the metric topology of $d_\ell(s,t)=|s-t|_\ell$. Give $\mathbb Z_\ell$ and $\mathbb Q_\ell^\times$ their subspace topologies from $\mathbb Q_\ell$ and give $\mathbb Z_\ell^\times$ the subspace topology from $\mathbb Q_\ell^\times$.

The finite adele ring and its group of units, the finite scalar ideles, are

$$\mathbb A_f=\{(a_\ell)\in\prod_\ell\mathbb Q_\ell:a_\ell\in\mathbb Z_\ell\text{ for all but finitely many }\ell\},$$

$$\mathbb A_f^\times=\{(a_\ell)\in\prod_\ell\mathbb Q_\ell^\times:a_\ell\in\mathbb Z_\ell^\times\text{ for all but finitely many }\ell\}.$$

The operations are coordinatewise. Embed $\mathbb Q$ diagonally as constant tuples using the canonical embeddings $\mathbb Q\to\mathbb Q_\ell$.

A restricted product here consists of tuples belonging to the specified integral factors outside a finite set. Its basic opens are boxes $\prod_\ell V_\ell$, with each $V_\ell$ open in the local ambient factor and $V_\ell$ equal to the specified integral factor for all but finitely many $\ell$. The factors for the ring are $(\mathbb Q_\ell,\mathbb Z_\ell)$ and for the group they are $(\mathbb Q_\ell^\times,\mathbb Z_\ell^\times)$, with $\mathbb Z_\ell^\times=\{t:|t|_\ell=1\}$.

## Facts & Assumptions

**Given:** The prime-indexed local fields and their rings of integers.

[F1] The $\ell$-adic completion is a valued field, $\mathbb Z_\ell$ is its integer subring, and $\mathbb Z_\ell$ and $\mathbb Z_\ell^\times$ are open in $\mathbb Q_\ell$. Local addition and multiplication are continuous for the field metric. The reciprocal is continuous on the nonzero scalars for the restricted metric ([def-author-6f52147f3ab3-hamilton-order-completions](item-def-author-6f52147f3ab3-hamilton-order-completions), Justification 2.1 and 5.1–6.1). The rational embedding into each completion is the isometric constant-sequence map, and the local field operations are obtained by termwise addition and multiplication of Cauchy sequences ([math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers), [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)).

[F2] For nonzero integers $a,b$, the rational valuation satisfies $v_\ell(a/b)=v_\ell(a)-v_\ell(b)$ ([math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)). On a nonzero integer the valuation is the greatest exponent of a dividing power of $\ell$ ([math:def-p-adic-valuation](https://alphabetamath.cc/item/def-p-adic-valuation)). The absolute value is $|a/b|_\ell=\ell^{-v_\ell(a/b)}$ and $|0|_\ell=0$ ([math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)). An integer $\ell$ divides $a$ when $a=\ell q$ for some integer $q$ ([math:def-divides-in-z](https://alphabetamath.cc/item/def-divides-in-z)). A positive divisor of a nonzero integer has size at most the absolute value of that integer ([math:lem-divisor-bound](https://alphabetamath.cc/item/lem-divisor-bound)).

[F3] A unital ring homomorphism preserves addition, multiplication and the identity ([math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)). A unital ring with a unital ring homomorphism from $\mathbb Q$ whose image is central is a $\mathbb Q$-algebra ([math:def-algebra-over-a-commutative-ring](https://alphabetamath.cc/item/def-algebra-over-a-commutative-ring)).

[F4] Basic open sets form a basis when they are open and every open neighborhood contains a basic open neighborhood of its point ([math:def-topology-basis-subbasis](https://alphabetamath.cc/item/def-topology-basis-subbasis)). The basis criterion requires that the proposed family cover the set and refine a binary intersection about each of its points ([math:thm-basis-criterion](https://alphabetamath.cc/item/thm-basis-criterion)). In a product topology, basic opens restrict only finitely many factors ([math:def-product-topology](https://alphabetamath.cc/item/def-product-topology)).

[F5] Metric open sets contain a ball about each of their points ([math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)). Relatively open sets are traces of ambient open sets ([math:def-subspace-topology-top](https://alphabetamath.cc/item/def-subspace-topology-top)). A map is continuous at a point if each open neighborhood of its image contains the image of an open neighborhood of the point ([math:def-continuous-map-top](https://alphabetamath.cc/item/def-continuous-map-top)). A topological group is a group whose multiplication and inversion are continuous ([math:def-topological-group](https://alphabetamath.cc/item/def-topological-group)).

[F6] A finite set admits a bijective listing of natural-number length ([math:def-countable](https://alphabetamath.cc/item/def-countable)). Every subset of a finite set is finite ([math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)). For a finite list of nonempty sets one may select one element from each ([math:lem-finite-choice](https://alphabetamath.cc/item/lem-finite-choice)). Every prime is an integer greater than $1$ ([math:def-prime](https://alphabetamath.cc/item/def-prime)).

[F7] A ring has an abelian additive group, associative multiplication with identity, and both distributive laws ([math:def-ring](https://alphabetamath.cc/item/def-ring)). The two-sided units of a unital ring form a group under its multiplication ([math:lem-ring-units-form-a-group](https://alphabetamath.cc/item/lem-ring-units-form-a-group)). A subset of a group is a subgroup if it contains the ambient identity and is closed under products and inverses ([math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)).

[F8] For a metric $d$ on $X$, the open ball about $x\in X$ of radius $r>0$ is $B_d(x,r)=\{y\in X:d(x,y)<r\}$ ([math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball)). This ball is open in the topology induced by the metric ([math:thm-metric-open-set-algebra](https://alphabetamath.cc/item/thm-metric-open-set-algebra), clause 1).

[F9] The whole space is open by axiom (T1), and the intersection of two open sets in a topological space is open by axiom (T3) ([math:def-topological-space](https://alphabetamath.cc/item/def-topological-space)).

## Justification

**Goal:** Verify the scalar ring and its units, and justify the stated topologies.

1.1 For two finite sets, concatenate their finite listings and keep only the first occurrence of each entry. This lists their union without repetitions, so the union is finite. Outside the union of the exceptional sets of two tuples, their coordinates belong to the local integer subrings. Those subrings are closed under addition, multiplication and negation, so the corresponding coordinatewise operations preserve $\mathbb A_f$. The zero and identity tuples are integral at every prime. The additive group laws, the multiplicative identity and associativity laws, the two distributive laws, and commutativity of multiplication all hold in each coordinate field. Thus $\mathbb A_f$ is a commutative unital ring. Its two-sided units form a group by [F7]. A tuple in $\mathbb A_f$ is invertible precisely when every coordinate is nonzero and the termwise inverse also belongs to $\mathbb A_f$, since multiplication and the identity are coordinatewise. At any prime, a nonzero coordinate and its inverse are both integral exactly when its absolute value is $1$, since the two absolute values are reciprocal. If the tuple is invertible, the union of the tuple's and its inverse's exceptional sets is finite, and every coordinate off that union has absolute value $1$. Conversely, the absolute-value-one condition off a finite set makes both the tuple and its coordinatewise inverse integral there. This proves the displayed description of the unit group. [F1, F6, F7, given]

1.2 Negation satisfies $d_\ell(-s,-t)=d_\ell(t,s)=d_\ell(s,t)$. For an open set containing $-s$, take a ball of radius $r>0$ about $-s$ contained in that set. The ball of radius $r$ about $s$ is open and maps into the target ball by the distance equality. This proves continuity of negation. For $s\in\mathbb Q_\ell^\times$, a ball about $s$ for the restricted metric is the trace of the field ball of the same radius, since both use the same distance inequality. Each such trace is relatively open, and every relatively open neighborhood of $s$ contains one by the ambient metric criterion. The restricted metric therefore induces the stated subspace topology. To use local multiplication on $\mathbb Q_\ell^\times$, write an open target there as the trace of an open set of $\mathbb Q_\ell$. An ambient input rectangle mapping into that open set restricts to a relatively open rectangle of nonzero inputs, whose products remain nonzero. For inversion, the reciprocal is continuous on the nonzero inputs by [F1] and takes values there, so the same trace test applies to the target. [F1, F4, F5, F8]

2.1 In either restricted product, each tuple belongs to a basic box that uses the full ambient factors at its finitely many exceptional primes and the integral factors elsewhere. The full ambient factors are open by (T1) and $\mathbb Z_\ell$ is open by [F1]. The factor $\mathbb Z_\ell^\times$ is open in $\mathbb Q_\ell^\times$ because it is the trace of an open subset of the field. For any two basic boxes, their intersection is the coordinatewise intersection box. Its factors are open by (T3) and equal the integral factors off the union of the two exceptional sets. The covering and intersection properties give the stated basis. [F1, F4, F5, F9, step 1.1]

2.2 The diagonal zero tuple is integral everywhere. For $a/b\ne 0$, choose nonzero integers $a,b$ representing it. If $\ell$ does not divide $b$, no positive power of $\ell$ divides $b$, because any such divisibility would give $b=\ell(\ell^{k-1}q)$ with $k\ge 1$. Thus $v_\ell(b)=0$ and $v_\ell(a)\ge 0$, so $|a/b|_\ell\le 1$. The inverse $b/a$ is integral off the divisors of $a$ by the same calculation. Every prime dividing either integer lies in the finite interval $\{1,\ldots,M\}$ for $M=\max(|a|,|b|)$. This interval has the bijective listing $k\mapsto k+1$ for $0\le k<M$. The two prime-divisor sets and their union are finite as subsets of this interval. Thus the diagonal maps take $\mathbb Q$ into $\mathbb A_f$ and $\mathbb Q^\times$ into $\mathbb A_f^\times$. Each coordinate map preserves addition and multiplication by the termwise operations on constant sequences. It sends $1$ to the constant sequence of ones, which acts as the local identity by termwise multiplication. Therefore the diagonal map is a unital ring homomorphism. It is injective since every coordinate embedding is injective, and its image is central by commutativity of $\mathbb A_f$. This makes $\mathbb A_f$ a commutative $\mathbb Q$-algebra. [F1, F2, F3, F6, step 1.1]

3.1 Fix an input to an operation and a basic box containing its output. Enlarge the finite set of exceptional primes of the target box to include all exceptional primes of the input tuples. The resulting union is finite by applying the binary union argument of step 1.1 at most twice. At each prime in the enlarged set, local continuity gives open input neighborhoods mapping into the target factor, using an open rectangle for a binary operation. Select one such neighborhood or rectangle at each of these finitely many primes. At every other prime use the integral input factors. The integral subrings are closed under the ring operations. In the local multiplicative group $\mathbb Q_\ell^\times$, which is a group of units by [F7], $\mathbb Z_\ell^\times$ contains the same identity $1$ because $|1|_\ell=1$. Multiplicativity and $|t^{-1}|_\ell=|t|_\ell^{-1}$ show that products and inverses of elements of absolute value $1$ still have absolute value $1$. Thus $\mathbb Z_\ell^\times$ is a subgroup by [F7]. This choice produces a restricted-product input box, or a rectangle of two such boxes for a binary operation, mapping into the target box. Thus addition, multiplication and negation are continuous on the adele ring, and multiplication and inversion are continuous on the idele group, making it a topological group. [F1, F4, F5, F6, F7, step 1.1, step 2.1, step 1.2]

4.1 The box of all integral factors is open in each restricted product. Its intersection with a basic box restricts only finitely many coordinates by relatively open conditions, because each condition is the trace of a local ambient open set. Conversely, take a basic product-open set of the integral factors. Each of its finitely many restricted coordinate sets is the trace of a local ambient open set on the integral factor. The integral factor is itself ambient-open, so this trace is open in the ambient factor by (T3). Take these coordinate sets at the restricted primes and the integral factors elsewhere. The open box so obtained has the given product-open set as its intersection with the box of all integral factors. Thus the induced topology on that box is its product topology. [F1, F4, F5, F9, step 2.1] ∎
