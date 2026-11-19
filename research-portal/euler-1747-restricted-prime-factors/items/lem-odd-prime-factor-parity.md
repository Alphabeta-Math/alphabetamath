---
id: lem-odd-prime-factor-parity
kind: lemma
title: Odd prime multiplicities modulo four
status: draft
domain: mathematics
proof_strategy: direct
deps:
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-monoid-finite-product
  - math:thm-generalised-associativity
  - math:lem-congruence-respects-integer-arithmetic
  - math:thm-induction-principle
  - math:thm-reals-cauchy-complete
  - math:thm-of-square-roots
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-of-square-monotone
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-natural-numbers
  - math:def-nat-order
  - math:def-finite-cardinality
  - math:thm-subset-of-a-finite-set
  - math:def-real-numbers
  - math:def-real-order
  - math:def-semigroup-and-monoid
  - math:def-injection-surjection-bijection
  - math:def-symmetric-group
  - math:lem-nat-order-is-membership
  - math:def-subset-and-proper-subset
  - math:def-complete-ordered-field
  - math:def-ordered-field
  - math:def-function
  - math:def-ring
  - math:def-field
  - math:def-rationals
  - math:def-ordered-pair
  - math:def-unordered-pair-and-singleton
  - math:def-union-of-a-set-and-binary-union
  - math:lem-unions-and-intersections-of-small-families
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-cartesian-product
  - math:def-nat-addition
  - math:def-nat-multiplication
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-divides-in-z
  - math:def-prime
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:def-nat-order
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-monoid-finite-product
  - math:def-congruence-modulo-an-integer
  - math:thm-subset-of-a-finite-set
  - math:def-finite-cardinality
  - math:lem-nat-embeds-int
  - math:def-real-numbers
  - math:def-real-order
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:thm-reals-cauchy-complete
  - math:thm-of-square-roots
  - math:lem-nat-order-is-membership
  - math:def-subset-and-proper-subset
  - math:def-function
argument_deps:
  - math:def-divides-in-z
  - math:def-prime
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
  - math:thm-fundamental-theorem-of-arithmetic
  - math:def-monoid-finite-product
  - math:thm-generalised-associativity
  - math:lem-congruence-respects-integer-arithmetic
  - math:thm-induction-principle
  - math:thm-reals-cauchy-complete
  - math:thm-of-square-roots
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:lem-of-square-monotone
  - math:def-natural-numbers
  - math:def-semigroup-and-monoid
  - math:def-injection-surjection-bijection
  - math:thm-subset-of-a-finite-set
  - math:def-finite-cardinality
  - math:def-symmetric-group
  - math:lem-nat-order-is-membership
  - math:def-nat-order
  - math:def-subset-and-proper-subset
  - math:def-complete-ordered-field
  - math:def-ordered-field
  - math:def-function
  - math:def-ring
  - math:def-field
  - math:def-rationals
  - math:def-ordered-pair
  - math:def-unordered-pair-and-singleton
  - math:def-union-of-a-set-and-binary-union
  - math:lem-unions-and-intersections-of-small-families
  - math:thm-the-characterising-property-of-ordered-pairs
  - math:def-cartesian-product
  - math:def-nat-addition
  - math:def-nat-multiplication
  - math:def-int-operations
dependency_roles:
  math:def-divides-in-z: mathematical-premise
  math:def-prime: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
  math:thm-fundamental-theorem-of-arithmetic: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
  math:thm-generalised-associativity: mathematical-premise
  math:lem-congruence-respects-integer-arithmetic: mathematical-premise
  math:thm-induction-principle: mathematical-premise
  math:thm-reals-cauchy-complete: mathematical-premise
  math:thm-of-square-roots: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:lem-of-square-monotone: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:def-nat-order: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:def-real-numbers: mathematical-premise
  math:def-real-order: mathematical-premise
  math:def-semigroup-and-monoid: mathematical-premise
  math:def-injection-surjection-bijection: mathematical-premise
  math:def-symmetric-group: mathematical-premise
  math:lem-nat-order-is-membership: mathematical-premise
  math:def-subset-and-proper-subset: mathematical-premise
  math:def-complete-ordered-field: mathematical-premise
  math:def-ordered-field: mathematical-premise
  math:def-function: mathematical-premise
  math:def-ring: mathematical-premise
  math:def-field: mathematical-premise
  math:def-rationals: mathematical-premise
  math:def-ordered-pair: mathematical-premise
  math:def-unordered-pair-and-singleton: mathematical-premise
  math:def-union-of-a-set-and-binary-union: mathematical-premise
  math:lem-unions-and-intersections-of-small-families: mathematical-premise
  math:thm-the-characterising-property-of-ordered-pairs: mathematical-premise
  math:def-cartesian-product: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:def-nat-multiplication: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
dependency_level: 0
---

## Statement

Let $u$ be a positive odd integer, meaning $u>0$ and $2$ does not divide $u$. Write $u=\prod_{i<m}p_i$ as a product of primes, allowing repetitions and using the empty product $1$ when $u=1$. Index the list by the natural number $m$ viewed as the set of its predecessors, which is empty for $m=0$. Let $S=\{i\in m:p_i\equiv3\pmod4\}$ and let $k=|S|$, the finite cardinality of $S$. This counts each such prime with its multiplicity, the number of times it occurs. Write $(-1)^k$ for the product of $k$ copies of $-1$. Then $u\equiv(-1)^k\pmod4$.

If $u\equiv1\pmod4$, the count $k$, viewed as a nonnegative integer, is even, meaning divisible by $2$. If in addition $u$ has a prime divisor congruent to $3$ modulo $4$, it has one at most $\sqrt{u}$, the unique nonnegative real number whose square is $u$, using the usual embedding of the integers in the reals.

## Statement references

[[math:def-integers]]

[[math:def-int-order]]

[[math:def-int-operations]]

[[math:def-divides-in-z]]

[[math:def-prime]]

[[math:thm-int-ordered-ring]]

[[math:def-natural-numbers]]

[[math:def-nat-order]]

[[math:lem-nat-order-is-membership]]

[[math:thm-fundamental-theorem-of-arithmetic]]

[[math:def-function]]

[[math:def-monoid-finite-product]]

[[math:def-congruence-modulo-an-integer]]

[[math:def-subset-and-proper-subset]]

[[math:thm-subset-of-a-finite-set]]

[[math:def-finite-cardinality]]

[[math:lem-nat-embeds-int]]

[[math:def-real-numbers]]

[[math:def-real-order]]

[[math:lem-int-embeds-rat]]

[[math:lem-rat-embeds-dense]]

[[math:thm-reals-cauchy-complete]]

[[math:thm-of-square-roots]]

## Facts & Assumptions

[F1] An integer $d$ divides $a$ when $a=dq$ for some integer $q$ ([[math:def-divides-in-z]]). A prime is an integer greater than $1$ whose only positive divisors are $1$ and itself ([[math:def-prime]]).

[F2] Congruence $a\equiv b\pmod n$ means $a-b=nq$ for some integer $q$ ([[math:def-congruence-modulo-an-integer]]). For an integer $a$ and a positive integer $b$, the quotient $q$ and remainder $r$ satisfying $a=bq+r$ and $0\le r<b$ are unique and exist ([[math:thm-division-algorithm-in-z]]).

[F3] The integers form a commutative ring ([[math:def-ring]]) with a total order preserved by addition and with positive elements closed under multiplication ([[math:thm-int-ordered-ring]]). The natural-number embedding $\iota(n)=[(n,0)]$ is injective, preserves addition and multiplication, preserves and reflects order, and has image exactly the nonnegative integers ([[math:lem-nat-embeds-int]]). No natural number lies strictly between a natural number and its successor ([[math:lem-nat-discrete]]).

[F4] Every integer at least $1$ is a finite product of primes, and any two such lists for that integer differ only by a permutation ([[math:thm-fundamental-theorem-of-arithmetic]]). A permutation of the index set $m$ is a bijection $m\to m$ ([[math:def-symmetric-group]], [[math:def-injection-surjection-bijection]]).

[F5] A finite product in a monoid starts at its identity and multiplies by the next factor at each extension of the list ([[math:def-monoid-finite-product]]). Finite products in a monoid can be split at a given length or regrouped using nondecreasing natural-number endpoints starting at $0$. In a commutative monoid they can also be reordered without changing their value ([[math:thm-generalised-associativity]]). Integer multiplication is associative and commutative with identity $1$ by [F3], so it defines a commutative monoid ([[math:def-semigroup-and-monoid]]).

[F6] If two pairs of integers are congruent modulo the same modulus, their respective products are also congruent ([[math:lem-congruence-respects-integer-arithmetic]]). Induction establishes a property on the natural numbers by proving it at $0$ and showing that it passes from $j$ to $j+1$ ([[math:thm-induction-principle]]).

[F7] The real numbers form a complete ordered field ([[math:thm-reals-cauchy-complete]]), meaning a field ([[math:def-field]]) with an order as in [[math:def-ordered-field]] in which every nonempty bounded-above subset has a least upper bound ([[math:def-complete-ordered-field]]). In such a field every nonnegative number has a unique nonnegative square root ([[math:thm-of-square-roots]]).

[F8] The embeddings of the integers into the rationals ([[math:def-rationals]]) and of the rationals into the reals preserve order and multiplication ([[math:lem-int-embeds-rat]], [[math:lem-rat-embeds-dense]]). In an ordered field ([[math:def-ordered-field]]), if $a,b$ are nonnegative and $a^2\le b^2$, then $a\le b$ ([[math:lem-of-square-monotone]]).

[F9] Separating a membership condition from a given set defines a subset of that set ([[math:def-subset-and-proper-subset]]). Every natural number $m$ viewed as its set of predecessors is finite with cardinality $m$ ([[math:def-finite-cardinality]]). A subset of a finite set is finite ([[math:thm-subset-of-a-finite-set]]). A finite set has cardinality zero exactly when it is empty. If $|S|=k$, there is a bijection from $k$ to $S$, and a bijection between finite sets preserves their cardinality ([[math:def-finite-cardinality]]). A bijection is an injective and surjective function ([[math:def-injection-surjection-bijection]]).

[F10] For natural numbers $i,n$ in the von Neumann model, $i<n$ is equivalent to $i\in n$, and $i\le n$ is equivalent to $i\subseteq n$ ([[math:def-natural-numbers]], [[math:def-nat-order]], [[math:lem-nat-order-is-membership]]). The successor is $\sigma(n)=n\cup\{n\}$, with $n\notin n$ and $n<\sigma(n)$. In particular, the natural number $2$ is $\{0,1\}$ ([[math:def-natural-numbers]]).

[F11] A function $f:A\to B$ assigns each input in its domain $A$ exactly one value in its codomain $B$ ([[math:def-function]]).

[F12] An ordered pair $(a,b)$ is the set $\{\{a\},\{a,b\}\}$ ([[math:def-ordered-pair]]), and equality of ordered pairs is coordinatewise ([[math:thm-the-characterising-property-of-ordered-pairs]]). The singleton $\{x\}$ has just the member $x$ ([[math:def-unordered-pair-and-singleton]]). The binary union $A\cup B$ is the union of $\{A,B\}$ ([[math:def-union-of-a-set-and-binary-union]]) and its members are exactly the elements belonging to $A$ or to $B$ ([[math:lem-unions-and-intersections-of-small-families]]). The Cartesian product $A\times B$ is the set of ordered pairs with first entry in $A$ and second entry in $B$ ([[math:def-cartesian-product]]).

[F13] For natural $a,b$, addition satisfies $a+0=a$ and $a+\sigma(b)=\sigma(a+b)$ ([[math:def-nat-addition]]). Multiplication satisfies $a\cdot0=0$ and $a\cdot\sigma(b)=a\cdot b+a$ ([[math:def-nat-multiplication]]). The numerals $1$ and $2$ are $\sigma(0)$ and $\sigma(1)$ ([[math:def-natural-numbers]]). The embedding $\iota$ sends the natural $0$ and $1$ to the integer $0=[(0,0)]$ and $1=[(1,0)]$ ([[math:def-int-operations]], [F3]). Since $1+1=2$ in the naturals by the addition recursion, it also sends $2$ to the integer $2$ by preservation of addition.

## Proof

**Given:** A positive integer $u$ with $2\nmid u$.

**Goal:** Prove the product congruence, the evenness of $k$ when $u\equiv1\pmod4$, and the square-root bound when a prime divisor congruent to $3$ modulo $4$ exists.

1.1 By prime factorization, take $u=\prod_{i<m}p_i$. The set $S$ is a subset of the finite index set $m$, so it is finite and its cardinality $k$ is a natural number. For another prime list $p'_i$ for $u$, uniqueness gives the same length and a permutation $\pi$ of $m$ with $p'_i=p_{\pi(i)}$. Let $S'=\{i\in m:p'_i\equiv3\pmod4\}$, a finite subset of $m$. Then $i\in S'$ exactly when $i\in m$ and $\pi(i)\in S$. Separate from the graph of $\pi$ exactly the pairs with first entry in $S'$. This gives a function from $S'$ to $S$ because each $i\in S'$ has exactly one value $\pi(i)$ and that value belongs to $S$. The restriction is injective because $\pi$ is injective. It is onto $S$ because the preimage of each element of $S$ under $\pi$ belongs to $S'$. The two counts therefore agree. Each entry divides $u$ by moving it to the front and taking the product of the remaining entries. Conversely, if a prime $p$ divides $u$, write $u=pv$ with $v$ an integer. Since $p>1$ and $u>0$, $v$ must be positive: $v=0$ would give $u=0$ and $v<0$ would give $-u=p(-v)>0$. As a positive integer, $v\ge1$. Factoring $v$ and adjoining $p$ gives a prime list for $u$, so uniqueness forces $p$ to occur in the chosen list. [given, F1, F2, F3, F4, F5, F9, F11, F12]

2.1 Divide each $p_i$ by $4$ to get $p_i=4a_i+r_i$ with $r_i\in\{0,1,2,3\}$. If $r_i=0$ or $2$, write $r_i=2e$ with $e=0$ or $1$. Then $p_i=2(2a_i+e)$, and step 1.1 gives $u=p_i v$ for some integer $v$. Thus $u=2((2a_i+e)v)$, contradicting $2\nmid u$. Hence $r_i=1$ or $3$. Form the sign list by separating from $m\times\{-1,1\}$ the pairs $(i,1)$ for $r_i=1$ and $(i,-1)$ for $r_i=3$. The unique remainder at each $i\in m$ supplies exactly one value $s_i$. In both cases $p_i\equiv s_i\pmod4$, using $p_i+1=4(a_i+1)$ in the second case. By uniqueness of the remainder, the positions with $r_i=3$ are exactly those with $p_i\equiv3\pmod4$. [given, F1, F2, F3, F9, F11, F12, step 1.1]

3.1 Compare the products of the first $j$ terms of the prime list and the sign list by induction, asserting congruence modulo $4$ whenever $j\le m$. For $j=0$ both products equal $1$. If $\sigma(j)\le m$, then $j<m$ and $j\in m$ by [F10], so the induction hypothesis applies and the entries $p_j$ and $s_j$ are defined. Multiply the two products by those respective entries. The next products are congruent by the multiplication rule and the congruence of the next factors. At $j=m$ this gives $u\equiv\prod_{i<m}s_i\pmod4$. [F2, F3, F5, F6, F10, step 1.1, step 2.1]

4.1 For $j\le m$ let $S_j=\{i\in S:i\in j\}$ and $k_j=|S_j|$, which exists because $S_j$ is a subset of the finite set $S$. We show by induction that the product of the first $j$ signs is $(-1)^{k_j}$ whenever $j\le m$. At $j=0$, the count is zero and the product is $1$. If $\sigma(j)\le m$, then $j<m$ and the induction hypothesis applies at $j$. Since $\sigma(j)=j\cup\{j\}$ and $j\notin j$, the only possible new qualifying position is $j$. If $j\notin S$, then $S_{\sigma(j)}=S_j$ and the next sign is $1$, so both the count and product stay the same. If $j\in S$, then $S_{\sigma(j)}=S_j\cup\{j\}$. Choose a bijection $f:k_j\to S_j$ and take the graph $g=f\cup\{(k_j,j)\}$. The old graph supplies the unique pair at each input in $k_j$. The new pair has first coordinate $k_j\notin k_j$, so it supplies exactly one value at the new input. Thus $g$ is a function from $\sigma(k_j)=k_j\cup\{k_j\}$ to $S_{\sigma(j)}$. The old inputs map bijectively to $S_j$, and the new input maps to $j\notin S_j$, so $g$ is a bijection. Thus $k_{\sigma(j)}=\sigma(k_j)$ by uniqueness of finite cardinality. The next sign is $-1$, so the sign product appends one copy of $-1$ and is $(-1)^{k_{\sigma(j)}}$ by the product recursion. At $j=m$ we have $S_m=S$, so the full sign product is $(-1)^k$ and the congruence is $u\equiv(-1)^k\pmod4$. [F3, F5, F6, F9, F10, F11, F12, step 1.1, step 2.1, step 3.1]

5.1 Suppose $u\equiv1\pmod4$. The congruence in step 4.1 makes it enough to evaluate $(-1)^k$. Divide the nonnegative integer image of $k$ by $2$ to write $\iota(k)=2t+r$ with $r=0$ or $1$. If $t<0$, then $-t$ is a positive integer and hence at least $1$ by natural-number discreteness at $0$ and the order embedding. Thus $2t+r\le-1$, contrary to $\iota(k)\ge0$. Take natural numbers $T$ and $R$ with $\iota(T)=t$ and $\iota(R)=r$. Here $R$ is the natural $0$ or $1$. The embedding preserves addition and multiplication and sends the natural $2$ to the integer $2$, so injectivity transports the length identity to $k=2T+R$ in the naturals. [F2, F3, F10, F13, step 4.1]

6.1 The graph $\mathbb{N}\times\{-1\}$ defines the constant sequence of signs. Take the block endpoints $b_j=2j$ in the naturals. Multiplication recursion gives $b_0=0$ and $b_{\sigma(j)}=b_j+2$, hence the endpoints are nondecreasing by the definition of natural-number order. Each block has length $2$ and its two factors multiply to $1$. Regrouping through endpoint $b_T$ therefore gives a product of $T$ copies of $1$, which equals $1$ by induction using the product recursion. Split the full product at $b_T=2T$. Its remaining length is $R$, so its remaining product is $1$ if $R=0$ and $-1$ if $R=1$. Consequently $(-1)^k=1$ or $-1$, respectively. [F3, F5, F6, F10, F11, F12, F13, step 5.1]

7.1 If $R=1$, the congruence from step 4.1 gives $u\equiv-1\pmod4$. Together with $u\equiv1\pmod4$ this yields $u=4a+1=4b-1$ for integers $a,b$, so $2=4(b-a)$. This contradicts uniqueness of the remainder on division of $2$ by $4$: the quotient $0$ gives remainder $2$, whereas $b-a$ would give remainder $0$. Thus $R=0$ and $\iota(k)=2t$, so $k$ is even in the stated sense. [F1, F2, F3, step 4.1, step 5.1, step 6.1]

8.1 Continue to assume $u\equiv1\pmod4$ and suppose a prime divisor of $u$ is congruent to $3$ modulo $4$. It appears in the list, so $k>0$. By step 7.1, $\iota(k)=2t$. Since $\iota(k)>0$, the integer $t$ is positive, so $t\ge1$ and $\iota(k)\ge2$. By the definition of $k=|S|$, there is a bijection from the natural ordinal $k$ to $S$. By [F3], the integer inequality $\iota(k)\ge2$ gives $2\le k$ in the natural-number order. By [F10], $2=\{0,1\}\subseteq k$, so $0$ and $1$ belong to the domain and their images are distinct positions in $S$. Let $p$ and $q$ be their prime values, labeled so that $p\le q$. The values can coincide. Reorder the factors to write $u=pqc$, where $c$ is the product of the remaining primes. Starting with $1$, each multiplication by a prime preserves positivity, so induction gives $c>0$. Since $c$ is an integer, $c\ge1$. The differences $pq-p^2=p(q-p)$ and $pqc-pq=pq(c-1)$ are nonnegative. Thus $p^2\le pq\le u$. [F1, F2, F3, F5, F6, F9, F10, F13, step 1.1, step 7.1]

9.1 The integer-to-real embeddings preserve products and order, so the images of $p$ and $u$ are positive and still satisfy $p^2\le u$. By completeness of the real ordered field, $u$ has a nonnegative real square root and $(\sqrt{u})^2=u$. Both $p$ and $\sqrt{u}$ are nonnegative in the real ordered field, so $p^2\le(\sqrt{u})^2$ gives $p\le\sqrt{u}$. The selected $p$ is a prime divisor congruent to $3$ modulo $4$, which completes the bound and the proof. [F7, F8, step 1.1, step 8.1] ∎
