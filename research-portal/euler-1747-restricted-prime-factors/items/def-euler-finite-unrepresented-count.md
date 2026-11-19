---
id: def-euler-finite-unrepresented-count
kind: definition
title: The finite product-sum certificate
status: draft
domain: mathematics
deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:def-nat-addition
  - math:def-nat-multiplication
  - math:def-sum-over-a-finite-index-set
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - math:lem-nat-mult-identity
  - lem-binary-products-and-avoidance
  - math:def-nat-finite-sum-and-product
  - math:def-monoid-finite-product
formulation_deps:
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:def-congruence-modulo-an-integer
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:def-nat-addition
  - math:def-nat-multiplication
  - math:def-sum-over-a-finite-index-set
argument_deps:
  - math:thm-division-algorithm-in-z
  - math:thm-int-ordered-ring
  - def-euler-finite-certificate-indices
  - def-author-c74aeff6099d-bounded-integer-indices
  - math:lem-nat-embeds-int
  - math:def-nat-multiplication
  - math:lem-nat-mult-identity
  - math:def-sum-over-a-finite-index-set
  - lem-binary-products-and-avoidance
  - math:def-int-operations
  - math:def-nat-finite-sum-and-product
  - math:def-monoid-finite-product
dependency_roles:
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:def-congruence-modulo-an-integer: mathematical-premise
  def-euler-finite-certificate-indices: mathematical-premise
  def-author-c74aeff6099d-bounded-integer-indices: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:def-nat-addition: mathematical-premise
  math:def-nat-multiplication: mathematical-premise
  math:def-sum-over-a-finite-index-set: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:lem-nat-mult-identity: mathematical-premise
  lem-binary-products-and-avoidance: mathematical-premise
  math:def-nat-finite-sum-and-product: mathematical-premise
  math:def-monoid-finite-product: mathematical-premise
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 7, §7, equation (7.2) and its preceding sentence
dependency_level: 3
---

## Definition

Let $a$ be an integer with $1\le a\le313$ and $a\equiv1\pmod4$, meaning that $a-1=4m$ for an integer $m$. Write $m=(a-1)/4$ for this integer quotient. Use $H=2^{22}-1=4{,}194{,}303$ and the finite-range indicators $\varepsilon_j$. Each indicator is binary, meaning it is $0$ or $1$, for $0\le j\le H$, and $\varepsilon_j=0$ for every integer $j<0$.

For a nonnegative integer $B$, write $I_B$ for the finite set of integers from $0$ through $B$, including both endpoints. In the formula below the product ranges over $I_m$ and the sum ranges over $I_H$. A finite sum adds one value per index, and a finite product multiplies one value per index, with empty sum $0$ and empty product $1$. The sum and product are computed in the natural numbers $0,1,2,\ldots$, identified with their integer copies. For a binary value $b$, the difference $1-b$ is $1$ when $b=0$ and $0$ when $b=1$.

Define the integer
$$U(a)=\sum_{k=0}^{H}\prod_{i=0}^{(a-1)/4}(1-\varepsilon_i\varepsilon_{k-i}).$$

## Definition references

[[math:def-integers|Integers]]

[[math:def-int-order|Integer order]]

[[math:def-int-operations|Integer arithmetic]]

[[math:def-congruence-modulo-an-integer|Congruence modulo an integer]]

[[def-euler-finite-certificate-indices|Finite-range indicators and their zero extension]]

[[def-author-c74aeff6099d-bounded-integer-indices|Bounded integer index sets]]

[[math:def-natural-numbers|Natural numbers]]

[[math:lem-nat-embeds-int|Natural numbers as integers]]

[[math:def-nat-addition|Natural addition]]

[[math:def-nat-multiplication|Natural multiplication]]

[[math:def-sum-over-a-finite-index-set|Finite sums and products over index sets]]

## Justification

The congruence gives a quotient with remainder $0$, and division with remainder by the positive integer $4$ makes that quotient unique ([[math:thm-division-algorithm-in-z]]). Subtracting $1$ from the bounds on $a$ gives $0\le4m\le312=4\cdot78$. If integers satisfy $x<y$, then $4(y-x)>0$, so $4x<4y$. Totality of integer order now gives $0\le m\le78$ ([[math:thm-int-ordered-ring]]). Thus both $I_m$ and $I_H$ are finite bounded index sets ([[def-author-c74aeff6099d-bounded-integer-indices]]).

For $i\in I_m$ and $k\in I_H$, we have $0\le i\le78\le H$ and $k-i\le k\le H$ by integer order and its compatibility with addition ([[math:thm-int-ordered-ring]]). If $k-i$ is negative its indicator is $0$, and if $k-i$ is nonnegative its indicator lies in the defining range through $H$. Thus both indicators in each factor have uniquely specified binary values ([[def-euler-finite-certificate-indices]]).

Put $b=\varepsilon_i\varepsilon_{k-i}$ for a fixed pair of indices. If the right indicator is $0$, the product is $0$. If it is $1$, the product equals the left indicator. These are the natural multiplication rules for a right factor of $0$ or $1$ ([[math:def-nat-multiplication]], [[math:lem-nat-mult-identity]]). Thus $b$ is binary, and the two cases defining $1-b$ agree with integer subtraction by the additive identity and inverse laws ([[math:thm-int-ordered-ring]]). The binary product rule makes the product for each fixed $k$ either $0$ or $1$ because all tests $b$ are binary and $I_m$ is finite ([[lem-binary-products-and-avoidance]]). The finite product and finite sum each have a unique natural value, independent of the listing of their finite index sets ([[math:def-sum-over-a-finite-index-set]]). Taking the integer copy of the final sum gives one integer $U(a)$ for each admissible $a$.

Integer addition and multiplication are associative with identities $0$ and $1$, respectively ([[math:thm-int-ordered-ring]]). Thus the finite monoid recursion applies with integer addition for a sum and integer multiplication for a product ([[math:def-monoid-finite-product]]). For either operation, use the same index listing in both evaluations and extend the list of natural entries by the natural identity $e$ of the operation. Write $x_n$ for the entries of this extension and $T_n$ for the running natural value after $n$ entries. With $\ast$ denoting the operation, the recursion is $T_0=e$ and $T_{n+1}=T_n\ast x_n$ ([[math:def-nat-finite-sum-and-product]]).

The embedding $\iota(n)=[(n,0)]$ sends the natural $0$ and $1$ to the integer $0$ and $1$ by the definitions of those integer constants ([[math:def-int-operations]], [[math:lem-nat-embeds-int]]). It also preserves addition and multiplication ([[math:lem-nat-embeds-int]]). Hence $\iota(T_0)$ is the integer identity and $\iota(T_{n+1})=\iota(T_n)\ast\iota(x_n)$, with the operation on the right taken in the integers. By uniqueness of the monoid recursion, $\iota(T_n)$ is the integer running value for the list of embedded entries. At the original list length, the value depends only on the entries of that finite list ([[math:def-monoid-finite-product]]).

Preservation of binary multiplication and the two cases for $1-b$ above show that each integer factor is the image of its natural counterpart. The recursion comparison then identifies each integer inner product with the image of the natural inner product. Applying it again to the outer list of inner products gives $U(a)$ when the whole expression is evaluated directly in the integers. This holds for any listings because the natural finite-index values are independent of the listings ([[math:def-sum-over-a-finite-index-set]]).
