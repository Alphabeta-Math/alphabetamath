---
id: rem-euler-1747-formulation
kind: remark
title: Euler’s historical formulation
status: published
domain: mathematics
deps:
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
dependency_roles:
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:def-divides-in-z: mathematical-premise
  math:def-integers: mathematical-premise
  math:def-int-order: mathematical-premise
  math:def-int-operations: mathematical-premise
  math:thm-int-ordered-ring: mathematical-premise
  math:def-natural-numbers: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-nat-discrete: mathematical-premise
formulation_deps:
  - math:def-congruence-modulo-an-integer
  - math:def-divides-in-z
  - math:def-integers
  - math:def-int-order
  - math:def-int-operations
argument_deps:
  - math:def-congruence-modulo-an-integer
  - math:thm-int-ordered-ring
  - math:def-natural-numbers
  - math:lem-nat-embeds-int
  - math:lem-nat-discrete
provenance:
  statement: ai-altered
  proof: not-applicable
sources:
  references:
    - title: Euler’s 1747 conjecture on sums of integers with restricted prime factors
      url: https://hexagonmath.org/pdf/2611.00370v1
      locator: p. 1, §1, historical paragraph and Theorem 1.1, and p. 8, reference [4]
      statement: Section 1 identifies Euler’s proposal with Theorem 1.1 and cites it
        as appearing in Letter 115 with discussion in editorial note 10.
        Reference [4] identifies the 2016 edition.
      hypotheses: Applies to the attribution and cross-reference in the supplied
        article version.
      reading_limits: Checked the historical paragraph and Theorem 1.1 on PDF p. 1 and
        reference [4] on PDF p. 8. This citation records the article’s
        identification and bibliographic pointer.
    - title: Lettre CV. Euler à Goldbach
      url: https://www.e-rara.ch/download/pdf/15664108.pdf
      locator: Fuss edition, tome I, p. 413 (date) and pp. 419–420 (proposal)
      statement: Euler proposes splitting every number of the form 4m+2 into two parts
        4x+1 and 4y+1, neither with a divisor of the form 4p−1.
      hypotheses: The remark uses the positive-integer setting of the proposal. In
        modern notation m, x and y are nonnegative integers and p is a positive
        integer.
      reading_limits: Checked the date and the proposal in the digitized Fuss edition
        text at the indicated printed pages. The explicit ranges for m, x, y and
        p are the modern positive-integer interpretation.
    - title: Correspondence of Leonhard Euler with Christian Goldbach
      url: https://eterna.unibas.ch/publbez/article/view/1192
      locator: 2016 online edition, Letter 115, pp. 935–936 and editorial note 10, as
        cited by the article
      reading_limits: Checked the Basel catalogue entry. The page and note locators
        are reported in the supplied article.
dependency_level: 0
---

## Remarks

In his letter to Christian Goldbach dated May 6, 1747, Leonhard Euler proposed that for every nonnegative integer $m$ there are nonnegative integers $x$ and $y$ with
$$4m+2=(4x+1)+(4y+1),$$
such that neither of the two summands has a positive divisor of the form $4p-1$ for any positive integer $p$. A summand is one of the numbers being added. For an integer $a$, a positive integer $d$ is a divisor of $a$ if $a=dq$ for some integer $q$.

For integers $u$ and $v$, the notation $u\equiv v\pmod 4$ means $u=v+4k$ for some integer $k$. Since $m,x,y\ge 0$, we have $4m+2\ge 2$, $4x+1\ge 1$, and $4y+1\ge 1$. The three forms give residue $2$ modulo $4$ for the input and residue $1$ modulo $4$ for each summand.

The forbidden divisor forms are exactly the positive integers congruent to $3$ modulo $4$. Every positive integer is at least $1$ because the naturals embed in the integers in order, with image the nonnegative integers, and $1$ immediately succeeds $0$ in the naturals. For $p>0$, we have $p\ge 1$, so $4p-1=4(p-1)+3\ge 3$ and $4p-1\equiv 3\pmod 4$. Conversely, a positive integer $d\equiv 3\pmod 4$ has the form $d=4k+3$ for an integer $k$. If $k<0$, then $-k\ge 1$, which would give $d\le -1$. Thus $k\ge 0$, and $p=k+1>0$ gives $d=4p-1$.

The article identifies Euler’s proposal with its Theorem 1.1 and points to Letter 115 and editorial note 10 in the 2016 edition of the correspondence.

## Remarks references

[[math:def-divides-in-z|Integer divisibility]]

[[math:def-congruence-modulo-an-integer|Congruence modulo an integer]]

[[math:def-integers|Integers]]

[[math:def-int-order|Order on the integers]]

[[math:def-int-operations|Arithmetic on the integers]]

[[math:thm-int-ordered-ring|The integers as an ordered ring]]

[[math:def-natural-numbers|Zero and successor in the natural numbers]]

[[math:lem-nat-embeds-int|Embedding the naturals into the integers]]

[[math:lem-nat-discrete|Discreteness of the natural-number order]]
