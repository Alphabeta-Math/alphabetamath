---
id: thm-jacobi-signed-ordered-four-square-count
kind: theorem
title: Jacobi’s signed, ordered four-square count
status: draft
domain: mathematics
deps:
  - math:def-function
  - math:def-inverse-relation-composition-and-restriction
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-cartesian-product
  - math:def-ordered-pair
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-sum-of-four-squares-representation
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-p-adic-valuation
  - math:def-group-power
  - math:def-divides-in-z
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-nat-embeds-int
  - math:def-finite-cardinality
  - math:thm-int-ordered-ring
  - math:def-semigroup-and-monoid
  - math:lem-nat-discrete
  - math:lem-nat-order-is-membership
  - math:def-injection-surjection-bijection
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:lem-divisor-bound
  - math:def-int-abs
  - math:def-prime
formulation_deps:
  - math:def-function
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-cartesian-product
  - math:def-ordered-pair
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-subset-and-proper-subset
  - math:def-sum-of-four-squares-representation
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-p-adic-valuation
  - math:def-group-power
  - math:def-divides-in-z
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-nat-embeds-int
  - math:def-finite-cardinality
argument_deps:
  - math:def-function
  - math:def-inverse-relation-composition-and-restriction
  - math:thm-int-ordered-ring
  - math:def-semigroup-and-monoid
  - math:def-int-operations
  - math:def-group-power
  - math:def-finite-sum-in-a-commutative-monoid
  - math:lem-nat-embeds-int
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-int-order
  - math:lem-nat-discrete
  - math:def-integers
  - math:def-subset-and-proper-subset
  - math:lem-nat-order-is-membership
  - math:def-injection-surjection-bijection
  - math:def-finite-cardinality
  - math:def-cartesian-product
  - math:thm-product-rule
  - math:thm-subset-of-a-finite-set
  - math:def-divides-in-z
  - math:lem-divisor-bound
  - math:def-int-abs
  - math:def-prime
  - math:def-p-adic-valuation
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-sum-of-four-squares-representation
dependency_roles:
  math:def-function: mathematical-premise
  math:def-inverse-relation-composition-and-restriction: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-sum-of-four-squares-representation: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-p-adic-valuation: mathematical-premise
  math:def-group-power: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-finite-sum-in-a-commutative-monoid: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:thm-product-rule: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:lem-divisor-bound: mathematical-premise
  math:def-int-abs: mathematical-premise
  math:def-prime: mathematical-premise
provenance:
  statement: ai-altered
  proof: literature-derived
external_input: true
sources:
  references:
    - title: An Elementary Proof of Jacobi’s Four-Square Theorem
      url: https://www.fq.math.ca/Scanned/41-3/ewell.pdf#page=1
      locator: p. 224, §1, Theorem 1 and its preceding definitions
      statement: r_4(n) = 8(2 + (-1)^n) sigma(Od(n)), where sigma sums positive
        divisors and Od(n) = n / 2^b(n), with b(n) the largest exponent for
        which 2^b(n) divides n.
      hypotheses: n is a positive integer. r_4(n) counts all ordered integer
        quadruples with square sum n. Coordinates can be negative, zero or
        positive.
      reading_limits: Checked Theorem 1 and the definitions of the counted quadruples,
        positive divisor sum and odd part in the PDF text on p. 224, and the
        final even and odd coefficient formulas on p. 228. The analytic proof in
        §2 is imported.
dependency_level: 0
---

## Statement

For a positive integer $u$ (so $u>0$), let $\mathcal R_4(u)$ be the set of ordered quadruples of integers with square sum $u$. Here $\mathbb Z^4$ denotes $(\mathbb Z\times\mathbb Z)\times(\mathbb Z\times\mathbb Z)$, where $\mathbb Z$ is the set of integers and $(x_1,x_2,x_3,x_4)$ denotes the ordered pair $((x_1,x_2),(x_3,x_4))$.
$$\mathcal R_4(u)=\{(x_1,x_2,x_3,x_4)\in\mathbb Z^4:x_1^2+x_2^2+x_3^2+x_4^2=u\}.$$
Two quadruples are equal exactly when they agree at every position, by applying the equality rule for ordered pairs to the outer pair and to the two inner pairs. Each distinct quadruple is counted once. Zero and both signs of a nonzero integer are allowed in every coordinate.

Let $v_2(u)$ be the greatest natural number $k$ for which $2^k\mid u$, with $0\in\mathbb N$. Write $u_{\mathrm{odd}}=u/2^{v_2(u)}$ for the odd part of $u$. For a positive integer $m$, let $D(m)=\{d\in\mathbb Z:d>0,\ d\mid m\}$, where $d\mid m$ means $m=dq$ for some integer $q$. The finite sum $\sum_{d\mid m}d$ adds each element of $D(m)$ once.

The operations in the formula are integer operations. Powers use natural exponents. Write $\iota:\mathbb N\to\mathbb Z$ for the usual embedding. In $(-1)^u$, the exponent means the unique natural $n$ with $\iota(n)=u$. The natural cardinality $|\mathcal R_4(u)|$ is read as its image under $\iota$ in the equality below. Then the number of elements of $\mathcal R_4(u)$ is
$$|\mathcal R_4(u)|=8\bigl(2+(-1)^u\bigr)\sum_{d\mid u_{\mathrm{odd}}}d.$$

## Statement references

[[math:def-integers|Integers]]

[[math:def-int-order|Positivity in the integers]]

[[math:def-int-operations|Integer operations]]

[[math:def-cartesian-product|Cartesian product]]

[[math:def-ordered-pair|Ordered pair]]

[[math:thm-the-characterising-property-of-ordered-pairs|Equality of ordered pairs]]

[[math:def-subset-and-proper-subset|Separation notation]]

[[math:def-sum-of-four-squares-representation|Representation as a sum of four integer squares]]

[[math:def-natural-numbers|Natural numbers]]

[[math:def-nat-order|Order on the natural numbers]]

[[math:def-p-adic-valuation|Exponent of the largest dividing prime power]]

[[math:def-group-power|Powers with nonnegative exponents]]

[[math:def-divides-in-z|Integer divisibility]]

[[math:def-finite-sum-in-a-commutative-monoid|Sum indexed by a finite set]]

[[math:def-function|Function with a declared domain and codomain]]

[[math:lem-nat-embeds-int|Embedding of the natural numbers into the integers]]

[[math:def-finite-cardinality|Number of elements of a finite set]]

## Justification

The ordered-ring laws for integers give the commutative monoids $(\mathbb Z,\cdot,1)$ and $(\mathbb Z,+,0)$ used for powers and sums, respectively. [[math:thm-int-ordered-ring]] [[math:def-semigroup-and-monoid]] [[math:def-int-operations]]

Every positive integer is at least $1$. Indeed, it is the image of a positive natural number under the order-preserving embedding, and $1$ is the immediate successor of $0$ in the natural order. Likewise, the only integers in the interval from $1$ to $2$ are its endpoints, since $2$ is the immediate successor of $1$ in the natural order. [[math:lem-nat-embeds-int]] [[math:def-nat-order]] [[math:lem-nat-discrete]]

For an integer $B\ge 0$, let $I_B=\{y\in\mathbb Z:0\le y\le B\}$, formed by separation in $\mathbb Z$. Write $B=\iota(b)$ for the unique natural $b$ given by the embedding. Let $\operatorname{succ}(b)=b\cup\{b\}$ be its natural successor. The natural numbers $j\le b$ are precisely the elements of $\operatorname{succ}(b)$ by the identification of the natural order with membership. [[math:def-subset-and-proper-subset]] [[math:def-int-order]] [[math:def-natural-numbers]] [[math:lem-nat-embeds-int]] [[math:lem-nat-order-is-membership]]

Define $f$ by restricting the graph of $\iota$ to first coordinates in $\operatorname{succ}(b)$. The restriction has domain $\operatorname{succ}(b)$ and is single valued because $\iota$ is a function on all of $\mathbb N$. For every $j\in\operatorname{succ}(b)$, order preservation gives $0\le\iota(j)\le B$, so $f:\operatorname{succ}(b)\to I_B$. [[math:def-function]] [[math:def-inverse-relation-composition-and-restriction]] [[math:lem-nat-embeds-int]]

Injectivity of $\iota$ makes $f$ injective. For $y\in I_B$, the description of the image of $\iota$ gives $y=\iota(j)$ for a natural $j$. Since $y\le B=\iota(b)$ and $\iota$ reflects order, $j\le b$, hence $j\in\operatorname{succ}(b)$ and $f(j)=y$. Thus $f$ is surjective, making $I_B$ finite. [[math:lem-nat-embeds-int]] [[math:def-injection-surjection-bijection]] [[math:def-finite-cardinality]]

In any tuple in $\mathcal R_4(u)$, each square is nonnegative, since a negative integer has the same square as its positive opposite, and a product of positive integers is positive. Thus each $x_i^2$ is at most $u$. If $x_i>u$, then $x_i>u\ge1$ gives $x_i(x_i-1)\ge0$, so $x_i^2\ge x_i>u$. If $x_i<-u$, the same inequality for $-x_i$ gives $x_i^2>u$. Hence each coordinate lies in $J=\{x\in\mathbb Z:-u\le x\le u\}$. [[math:thm-int-ordered-ring]] [[math:def-subset-and-proper-subset]]

Define $T:J\to I_{2u}$ by $T(x)=x+u$ and $S:I_{2u}\to J$ by $S(y)=y-u$. Addition preserves the order, so $0\le x+u\le 2u$ for $x\in J$ and $-u\le y-u\le u$ for $y\in I_{2u}$. Form the graphs by separation in $J\times I_{2u}$ and $I_{2u}\times J$, respectively, keeping the pairs with the stated second coordinate. The bounds and the single value of each integer expression make these graphs functions of the declared types. [[math:def-function]] [[math:thm-int-ordered-ring]] [[math:def-cartesian-product]] [[math:def-subset-and-proper-subset]]

The ring laws give $T(S(y))=y$ for $y\in I_{2u}$ and $S(T(x))=x$ for $x\in J$. The first identity makes $S$ injective, and the second makes it surjective. Transport along $S$ makes $J$ finite. [[math:def-injection-surjection-bijection]] [[math:def-finite-cardinality]]

Three applications of the binary finite product rule make $(J\times J)\times(J\times J)$ finite. The square-sum predicate separates $\mathcal R_4(u)$ inside $\mathbb Z^4$, and the coordinate bounds make it a subset of this finite product. It is therefore finite, so its cardinality is defined. [[math:thm-int-ordered-ring]] [[math:def-cartesian-product]] [[math:thm-product-rule]] [[math:def-subset-and-proper-subset]] [[math:thm-subset-of-a-finite-set]] [[math:def-finite-cardinality]]

For $d\in D(m)$, the divisor bound gives $|d|\le |m|$ because $m>0$. Since $d,m>0$, the nonnegative clause of the absolute-value definition gives $|d|=d$ and $|m|=m$. Thus $D(m)$ is formed by separation in $\mathbb Z$ and lies in the finite set $I_m$. The subset theorem makes $D(m)$ finite. In the additive commutative monoid of integers, the finite sum over $D(m)$ has the same value in every enumeration. [[math:lem-divisor-bound]] [[math:def-int-abs]] [[math:def-divides-in-z]] [[math:def-subset-and-proper-subset]] [[math:thm-subset-of-a-finite-set]] [[math:def-finite-sum-in-a-commutative-monoid]]

In particular, every positive divisor of $2$ lies between $1$ and $2$. The endpoint property above and $2>1$ show that $2$ is prime. Since $u>0$, the valuation definition therefore gives the greatest exponent $k=v_2(u)$ with $2^k\mid u$. Its existence argument gives $2^k\ge1$. Divisibility supplies an integer $q$ with $2^kq=u$. Since $2^k>0$, multiplication by $2^k$ preserves strict order, so $q$ is positive and unique. This defines $u/2^k$. If $q=2t$ for an integer $t$, the recursion for natural powers gives $u=2^{\operatorname{succ}(k)}t$. Since $\operatorname{succ}(k)>k$, this contradicts the maximality of $k$. Thus the quotient is odd, meaning it is indivisible by $2$. [[math:def-prime]] [[math:def-p-adic-valuation]] [[math:def-group-power]] [[math:def-divides-in-z]] [[math:thm-int-ordered-ring]]

## External input

Apply Ewell’s Theorem 1 to the positive integer $n=u$. Reading each ordered quadruple as its pair of ordered pairs gives a bijection with the quadruples counted by his $r_4(u)$. This preserves every coordinate and the square sum, including tuples with zero or negative entries. His exponent $b(u)$ is $v_2(u)$, so $\operatorname{Od}(u)=u/2^{b(u)}$ is $u_{\mathrm{odd}}$. His $\sigma(\operatorname{Od}(u))$ sums precisely the elements of $D(u_{\mathrm{odd}})$. With these identifications and the natural exponent and cardinality conventions above, his formula gives the displayed count.
