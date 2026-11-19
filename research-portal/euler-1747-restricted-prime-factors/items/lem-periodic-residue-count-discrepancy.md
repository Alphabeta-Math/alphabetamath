---
id: lem-periodic-residue-count-discrepancy
kind: lemma
title: Periodicity and jump bounds for residue counts
status: draft
domain: mathematics
deps:
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:lem-integer-part
  - math:def-finite-cardinality
  - math:lem-nat-embeds-int
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-subset-of-a-finite-set
  - math:thm-sum-rule
  - math:def-ordered-field
  - math:thm-reals-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-abs-value
  - math:def-one-sided-limits
  - math:thm-well-ordering-principle
  - math:def-limit-point-r
  - math:lem-of-abs-value
formulation_deps:
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:lem-integer-part
  - math:def-finite-cardinality
  - math:lem-nat-embeds-int
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-subset-of-a-finite-set
  - math:def-ordered-field
  - math:thm-reals-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-abs-value
  - math:def-one-sided-limits
argument_deps:
  - math:def-congruence-modulo-an-integer
  - math:thm-division-algorithm-in-z
  - math:lem-integer-part
  - math:def-finite-cardinality
  - math:lem-nat-embeds-int
  - math:lem-cardinality-of-finite-natural-initial-segment
  - math:thm-subset-of-a-finite-set
  - math:thm-sum-rule
  - math:def-ordered-field
  - math:thm-reals-ordered-field
  - math:lem-int-embeds-rat
  - math:lem-rat-embeds-dense
  - math:def-abs-value
  - math:def-one-sided-limits
  - math:thm-well-ordering-principle
  - math:def-limit-point-r
  - math:lem-of-abs-value
dependency_roles:
  math:def-congruence-modulo-an-integer: mathematical-premise
  math:thm-division-algorithm-in-z: mathematical-premise
  math:lem-integer-part: mathematical-premise
  math:def-finite-cardinality: mathematical-premise
  math:lem-nat-embeds-int: mathematical-premise
  math:lem-cardinality-of-finite-natural-initial-segment: mathematical-premise
  math:thm-subset-of-a-finite-set: mathematical-premise
  math:thm-sum-rule: mathematical-premise
  math:def-ordered-field: mathematical-premise
  math:thm-reals-ordered-field: mathematical-premise
  math:lem-int-embeds-rat: mathematical-premise
  math:lem-rat-embeds-dense: mathematical-premise
  math:def-abs-value: mathematical-premise
  math:def-one-sided-limits: mathematical-premise
  math:thm-well-ordering-principle: mathematical-premise
  math:def-limit-point-r: mathematical-premise
  math:lem-of-abs-value: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Let $M$ be a positive integer and $D\subseteq\{1,\ldots,M\}$. Identify the integers with their usual copy in the reals, with arithmetic and order preserved. For an integer $k$, write $r_M(k)$ for its residue representative, the unique integer $d$ with $1\le d\le M$ for which $k-d$ is an integer multiple of $M$. Thus $M$ represents residue zero. Write $\#S$ and $|S|$ for the number of elements of a finite set $S$. For real $t\ge0$, define
$$A_D(t)=\#\{k\in\mathbb Z:1\le k\le t,\ r_M(k)\in D\},\qquad E_D(t)=A_D(t)-\frac{|D|}{M}t.$$

Then $M$ is a period of the discrepancy $E_D$, meaning $E_D(t+M)=E_D(t)$ for all $t\ge0$. In $0<t\le M$, its jumps, where the limits from below and above both exist and differ, are exactly the points $d\in D$. For any real $B\ge0$, if the endpoint values $E_D(0)$ and $E_D(M)$ and both one-sided limits at every $d\in D$ have absolute value at most $B$, then $|E_D(t)|\le B$ for all $t\ge0$. Here the absolute value of a real $x$ is $x$ for $x\ge0$ and $-x$ for $x<0$.

## Facts & Assumptions

[F1] Two integers are congruent modulo $M$ when their difference is an integer multiple of $M$ ([[math:def-congruence-modulo-an-integer|Integer congruence]]).

[F2] Division of an integer $a$ by a positive integer $M$ gives unique integers $q,r$ with $a=qM+r$ and $0\le r<M$ ([[math:thm-division-algorithm-in-z|Division with remainder]]).

[F3] The reals are a totally ordered field, so addition preserves inequalities and multiplication by a positive number preserves their direction ([[math:thm-reals-ordered-field|The ordered field of reals]], [[math:def-ordered-field|Ordered field]]). The usual inclusions from integers to rationals and rationals to reals preserve $1$, the arithmetic operations of addition and multiplication, and the order ([[math:lem-int-embeds-rat|Integers in the rationals]], [[math:lem-rat-embeds-dense|Rationals in the reals]]).

[F4] Every real $x$ has a unique integer part $\lfloor x\rfloor$, the integer $n$ with $n\le x<n+1$ ([[math:lem-integer-part|Integer part]]).

[F5] The naturals identify with the nonnegative integers, with the same arithmetic and order ([[math:lem-nat-embeds-int|Naturals in the integers]]). For a natural $n$, the set $\{j\in\mathbb N:j<n\}$ is finite with $n$ elements ([[math:lem-cardinality-of-finite-natural-initial-segment|Finite initial segment]]). Subsets of a finite set are finite ([[math:thm-subset-of-a-finite-set|Subsets of a finite set]]). A one-to-one correspondence, pairing every element of each set with exactly one in the other, transfers finiteness and cardinality ([[math:def-finite-cardinality|Finite cardinality]]).

[F6] The cardinality of the union of two disjoint finite sets, meaning they have no common element, is the sum of their cardinalities ([[math:thm-sum-rule|Sum rule]], two-block case).

[F7] Let $f$ be a function on $[0,\infty)$ and let $y>0$. The limit on a specified side requires domain points on that side with $0<|x-y|<\rho$ for every $\rho>0$ ([[math:def-limit-point-r|Limit point]]). Under this condition, a real $L$ is the left or right limit if for every $\varepsilon>0$ there is $\delta>0$ such that $|f(x)-L|<\varepsilon$ for all domain points with $y-\delta<x<y$, or with $y<x<y+\delta$, respectively. When a limit on either side exists, it is unique ([[math:def-one-sided-limits|One-sided limits]], [[math:def-abs-value|Absolute value]]).

[F8] Every nonempty set of nonnegative integers has a least element, an element at most every element of that set ([[math:thm-well-ordering-principle|Well-ordering of the naturals]], [[math:lem-nat-embeds-int|Naturals in the integers]]).

[F9] For reals $u,v$, absolute value satisfies $|-u|=|u|$ and $|uv|=|u||v|$ ([[math:lem-of-abs-value|Basic properties of absolute value]]). The definition gives $|u|=u$ for $u\ge0$ and $|u|=-u$ for $u<0$ ([[math:def-abs-value|Absolute value]]).

## Proof

**Given:** A positive integer $M$, a set $D\subseteq\{1,\ldots,M\}$, and the functions of the statement.

**Goal:** Establish the period identity and locate the jumps, then deduce the global absolute bound from the indicated values and limits.

1.1 Divide $k-1$ by $M$ to obtain $k-1=qM+r$ with $0\le r<M$. Then $d=r+1$ is in $\{1,\ldots,M\}$ and $k-d=qM$. Conversely, a candidate $d$ with $k-d=qM$ gives remainder $d-1$ in the division of $k-1$. Its uniqueness proves that $r_M(k)$ is well defined. In particular $r_M(j)=j$ for $1\le j\le M$, and $r_M(k)=M$ exactly when $k$ is a multiple of $M$. [F1, F2, F3]

1.2 There is no integer $j$ strictly between any integer $n$ and $n+1$, since both $n$ and $j$ would then be integer parts of $j$. For $t\ge0$, put $n=\lfloor t\rfloor$. If $n<0$, then $n<0\le t<n+1$, contradicting the absence of an integer strictly between $n$ and $n+1$. The integers $1\le k\le t$ are exactly those with $1\le k\le n$. The finite set $\{j\in\mathbb N:j<n\}$ corresponds to these integers by $j\mapsto j+1$ with inverse $k\mapsto k-1$, using the same absence of intervening integers. Hence the set counted by $A_D(t)$ is finite, and taking $t=M$ also shows that $D$ is finite. Put $c=|D|/M\ge0$, which is defined since $M>0$. [F3, F4, F5]

1.3 For each $y>0$ and $\rho>0$, set $h=\min\{y,\rho\}/2$. Then $0<h<y$ and $h<\rho$. The domain points $y-h$ and $y+h$ lie on opposite sides of $y$ at distance $h<\rho$ from it. Thus the limit-point condition in [F7] holds on both sides at every positive argument. [F3, F7]

2.1 Fix $t\ge0$. For each $d\in D$, an integer of the form $k=d+qM$ lies in $t<k\le t+M$ exactly when $q-1\le (t-d)/M<q$. By the integer-part property there is exactly one such $q$, namely $\lfloor (t-d)/M\rfloor+1$. Thus $k\mapsto r_M(k)$ pairs the newly counted integers with $D$ one-to-one. The newly counted set and the set counted by $A_D(t)$ are disjoint and their union is the set counted by $A_D(t+M)$. Hence $A_D(t+M)=A_D(t)+|D|$ and $E_D(t+M)=E_D(t)+|D|-cM=E_D(t)$. [F1, F3, F4, F5, F6, step 1.1, step 1.2]

2.2 For each positive integer $j$, discreteness of the integers from step 1.2 gives $A_D(x)=A_D(j)$ on $j\le x<j+1$. On $j-1<x<j$, the count is constant and equals $A_D(j)-1$ if $r_M(j)\in D$, and $A_D(j)$ otherwise, because only $j$ can be added at $x=j$. In that case the new point forms a set of cardinality one and the disjoint union rule adds one to the count. For either side, let $a$ be its constant count. Then $|E_D(x)-(a-cj)|=|-c(x-j)|=c|x-j|$ on that side. For $\varepsilon>0$, taking $\delta=\varepsilon/(1+c+\varepsilon)$ gives $0<\delta<1$ and $c\delta<\varepsilon$. Step 1.3 supplies the limit-point condition at $j>0$. Hence the right limit is $E_D(j)$ and the left limit is $E_D(j)-1$ if $r_M(j)\in D$, and $E_D(j)$ otherwise. [F3, F5, F6, F7, F9, step 1.2, step 1.3]

3.1 If $y>0$ is nonintegral, it is strictly between $n=\lfloor y\rfloor$ and $n+1$. Discreteness implies that $A_D$ is constant throughout $n<x<n+1$. In a neighborhood of $y$ lying in this interval, $|E_D(x)-E_D(y)|=|-c(x-y)|=c|x-y|$. Given $\varepsilon>0$, use the least of $y-n$, $n+1-y$ and $\varepsilon/(1+c+\varepsilon)$ as $\delta$ in the two one-sided conditions. Step 1.3 supplies the limit-point condition at $y$, so both limits equal $E_D(y)$. Combining this with the integer limits and $r_M(j)=j$ for $1\le j\le M$ gives exactly the claimed jumps in $0<t\le M$. [F3, F4, F7, F9, step 1.1, step 1.2, step 1.3, step 2.2]

3.2 Suppose the test values in the statement have absolute value at most $B$. For any real $z$, the bound $|z|\le B$ is equivalent to $-B\le z\le B$. If $z\ge0$, then $|z|=z$ and $-B\le z$ holds automatically. If $z<0$, then $|z|=-z$ and $z\le B$ holds automatically, while $-z\le B$ is equivalent to $-B\le z$. For $0\le u<M$, take $a$ to be the greatest element of $\{j\in D\cup\{0,M\}:j\le u\}$ and $b$ the least element of $\{j\in D\cup\{0,M\}:u<j\}$. These sets contain $0$ and $M$, respectively. The least element of the second exists by well-ordering. The first has a greatest element because applying well-ordering to the nonnegative integers $M-j$ for $j$ in that set gives a least $M-a$. On $a\le x<b$, the count equals $A_D(a)$, since on $0\le x\le M$ the counted integers are exactly the elements of $D$ at most $x$ and none lies strictly between $a$ and $b$. Since $c\ge0$, we have $A_D(a)-cb\le E_D(u)\le A_D(a)-ca=E_D(a)$. The lower endpoint of this inequality is the left limit at $b$, by applying the formula for the constant count just below the integer $b$ from step 2.2. If $b$ is outside $D$, then $b=M$ and this limit equals $E_D(M)$. The upper endpoint is $E_D(0)$ if $a=0$, and the right limit at $a$ otherwise. Thus $-B\le E_D(u)\le B$, and the same equivalence gives $|E_D(u)|\le B$. The bound at $u=M$ is one of the endpoint tests. [F3, F8, F9, step 1.1, step 1.2, step 2.2]

4.1 For any $t\ge0$, set $q=\lfloor t/M\rfloor$ and $u=t-qM$. As in step 1.2, $q\ge0$, and $0\le u<M$. For this $u$, the period identity gives $E_D(u+jM)=E_D(u)$ for all nonnegative integers $j$. If there were a failure, the least such $j$ would be positive, and translation by $M$ from $u+(j-1)M$ would rule out failure at $j$. In particular $E_D(t)=E_D(u)$, so $|E_D(t)|\le B$. This completes the periodicity and jump-bound claims. [F3, F4, F8, step 1.2, step 2.1, step 3.2] ∎
