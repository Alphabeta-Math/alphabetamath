---
title: Reciprocal-square tail from a counting function
status: draft
research_item: lem-reciprocal-square-tail-from-counting
dependency_level: 0
---

## Prerequisites

- [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)
- [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)
- [math:def-series](https://alphabetamath.cc/item/def-series)
- [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)
- [math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)
- [math:def-interval](https://alphabetamath.cc/item/def-interval)
- [math:def-darboux-integral](https://alphabetamath.cc/item/def-darboux-integral)
- [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set)
- [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)
- [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part)
- [math:lem-abel-summation-by-parts](https://alphabetamath.cc/item/lem-abel-summation-by-parts)
- [math:def-derivative](https://alphabetamath.cc/item/def-derivative)
- [math:lem-derivative-of-a-power](https://alphabetamath.cc/item/lem-derivative-of-a-power)
- [math:cor-differentiable-implies-continuous](https://alphabetamath.cc/item/cor-differentiable-implies-continuous)
- [math:def-continuity-real](https://alphabetamath.cc/item/def-continuity-real)
- [math:thm-finitely-many-discontinuities-integrable](https://alphabetamath.cc/item/thm-finitely-many-discontinuities-integrable)
- [math:thm-ftc-second-part](https://alphabetamath.cc/item/thm-ftc-second-part)
- [math:thm-linearity-of-the-integral](https://alphabetamath.cc/item/thm-linearity-of-the-integral)
- [math:thm-additivity-over-subintervals](https://alphabetamath.cc/item/thm-additivity-over-subintervals)
- [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)
- [math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity)
- [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)
- [math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)
- [math:def-darboux-sums](https://alphabetamath.cc/item/def-darboux-sums)
- [math:def-integers](https://alphabetamath.cc/item/def-integers)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:def-partition-and-refinement](https://alphabetamath.cc/item/def-partition-and-refinement)
- [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws)
- [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)
- [math:def-infimum](https://alphabetamath.cc/item/def-infimum)
- [math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value)
- [math:lem-of-triangle-inequality](https://alphabetamath.cc/item/lem-of-triangle-inequality)
- [math:def-rationals](https://alphabetamath.cc/item/def-rationals)
- [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)
- [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)
- [math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set)
- [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection)
- [math:def-function-limit](https://alphabetamath.cc/item/def-function-limit)
- [math:def-limit-point-r](https://alphabetamath.cc/item/def-limit-point-r)


## Statement

Let $D\subseteq\mathbb Z_{>0}$, where $\mathbb Z_{>0}$ denotes the integers greater than zero in their usual embedded copy in the complete ordered field $\mathbb R$ of real numbers, and let $P>0$ be real. For comparisons and arithmetic in $\mathbb R$, send integers to rationals by $k\mapsto k/1$ and then use the ordered-field embedding of the rationals into the reals. Send natural numbers, including finite cardinalities, first to their corresponding nonnegative integers. For real $t\ge P$ put $C(t)=\#\{k\in D:P<k\le t\}$, where $\#$ denotes finite cardinality, the number of elements of a finite set. Assume that real $a,b\ge0$ satisfy $C(t)\le a(t-P)+b$ for every real $t\ge P$. Then the series and the integral below both converge and
$$\sum_{\substack{k\in D\\k>P}}\frac1{k^2}=2\int_P^\infty C(t)t^{-3}\,dt\le\frac aP+\frac b{P^2}.$$

The series means the sequence limit of the finite sums over positive integers through $n$, taking the term to be zero unless $k\in D$ and $k>P$. The sequence limit uses positive rational tolerances, interpreted in $\mathbb R$ under the rational embedding. A finite sum begins at zero for the empty sum and adds one term at each index. The integral to infinity means the finite limit of the integrals over $[P,R]=\{t:P\le t\le R\}$ as real $R\to+\infty$. For $R>P$ and a bounded function on $[P,R]$, the finite Darboux integral is the common value of the supremum of the lower sums and the infimum of the upper sums when they agree. A function on this interval is bounded when its values have a common real lower bound and a common real upper bound. Both extrema are taken over all finite partitions of $[P,R]$, where a partition is a strictly increasing finite list of points from $P$ to $R$, including both endpoints. On the closed subinterval between each pair of consecutive points, the lower sum weights the infimum by the subinterval length and the upper sum weights the supremum by that length. For $x>0$ and a positive integer $r$, $x^{-r}$ is the reciprocal of the product of $r$ copies of $x$.

## Statement references

[math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

[math:def-integers](https://alphabetamath.cc/item/def-integers)

[math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)

[math:def-rationals](https://alphabetamath.cc/item/def-rationals)

[math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat)

[math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality)

[math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)

[math:def-series](https://alphabetamath.cc/item/def-series)

[math:def-real-limit](https://alphabetamath.cc/item/def-real-limit)

[math:def-interval](https://alphabetamath.cc/item/def-interval)

[math:def-darboux-integral](https://alphabetamath.cc/item/def-darboux-integral)

[math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set)

[math:def-darboux-sums](https://alphabetamath.cc/item/def-darboux-sums)

[math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field)

[math:def-infimum](https://alphabetamath.cc/item/def-infimum)

[math:def-partition-and-refinement](https://alphabetamath.cc/item/def-partition-and-refinement)

[math:def-improper-integral-at-infinity](https://alphabetamath.cc/item/def-improper-integral-at-infinity)

[math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity)

[math:def-integer-power](https://alphabetamath.cc/item/def-integer-power)

## Facts & Assumptions

[F1] A finite set of cardinality $q$ is in bijection with the first $q$ nonnegative integers, and every subset of a finite set is finite. A bijection is a one-to-one map onto its target. Induction propagates a property from $0$ to all nonnegative integers when the property at $n$ implies it at $n+1$. [math:def-finite-cardinality](https://alphabetamath.cc/item/def-finite-cardinality) [math:def-injection-surjection-bijection](https://alphabetamath.cc/item/def-injection-surjection-bijection) [math:thm-subset-of-a-finite-set](https://alphabetamath.cc/item/thm-subset-of-a-finite-set) [math:thm-induction-principle](https://alphabetamath.cc/item/thm-induction-principle)

[F2] The integer part $\lfloor x\rfloor$ of a real $x$ is the unique integer $d$ with $d\le x<d+1$. No integer lies strictly between $d$ and $d+1$, since such an integer would have both itself and $d$ as its integer part. Hence $k\le x$ is equivalent to $k\le\lfloor x\rfloor$ for integer $k$, and $\lfloor x\rfloor\ge0$ for $x\ge0$. Every nonnegative integer is the image of a unique natural number under the order- and arithmetic-preserving embedding. We use this identification for indices. The integer-to-rational and rational-to-real embeddings preserve order, addition, multiplication and the unit, so their composition preserves those operations and order. [math:lem-integer-part](https://alphabetamath.cc/item/lem-integer-part) [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int) [math:lem-int-embeds-rat](https://alphabetamath.cc/item/lem-int-embeds-rat) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F3] For real sequences $(e_j)$ and $(w_j)$ indexed by nonnegative integers, put $A_n=\sum_{j<n}e_j$. Abel summation by parts is the finite identity $\sum_{j<n}e_jw_j=A_nw_{n-1}+\sum_{j<n-1}A_{j+1}(w_j-w_{j+1})$ for every natural number $n\ge1$, using finite-sum scaling to move the minus sign into the remainder in the cited identity. [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum) [math:lem-abel-summation-by-parts](https://alphabetamath.cc/item/lem-abel-summation-by-parts) [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws)

[F4] The derivative at a domain point that is also a limit point of the domain is the punctured limit of the difference quotient, taken from within the domain. On the nonzero reals, $(t^{-r})'=-rt^{-r-1}$ for positive integers $r$. Differentiability implies continuity, meaning that $\lvert f(t)-f(c)\rvert$ can be made arbitrarily small by taking $t$ sufficiently close to $c$ in the domain. A bounded function on a closed finite interval with distinct endpoints is Darboux integrable if it is continuous except possibly at finitely many points. [math:def-derivative](https://alphabetamath.cc/item/def-derivative) [math:def-function-limit](https://alphabetamath.cc/item/def-function-limit) [math:def-limit-point-r](https://alphabetamath.cc/item/def-limit-point-r) [math:lem-derivative-of-a-power](https://alphabetamath.cc/item/lem-derivative-of-a-power) [math:cor-differentiable-implies-continuous](https://alphabetamath.cc/item/cor-differentiable-implies-continuous) [math:def-continuity-real](https://alphabetamath.cc/item/def-continuity-real) [math:def-bounded-set](https://alphabetamath.cc/item/def-bounded-set) [math:thm-finitely-many-discontinuities-integrable](https://alphabetamath.cc/item/thm-finitely-many-discontinuities-integrable)

[F5] If $u<v$, $G$ is differentiable on $[u,v]$ and $G'$ is integrable there, then $\int_u^v G'=G(v)-G(u)$. Finite integrals are linear in integrable functions and additive when an interval is split. They preserve pointwise order and satisfy $0\le\int_u^v f\le K(v-u)$ if $0\le f\le K$ and $u<v$. [math:thm-ftc-second-part](https://alphabetamath.cc/item/thm-ftc-second-part) [math:thm-linearity-of-the-integral](https://alphabetamath.cc/item/thm-linearity-of-the-integral) [math:thm-additivity-over-subintervals](https://alphabetamath.cc/item/thm-additivity-over-subintervals) [math:thm-monotonicity-of-the-integral](https://alphabetamath.cc/item/thm-monotonicity-of-the-integral)

[F6] Every nonempty set of real numbers bounded above has a least upper bound. For a real-parameter limit at $+\infty$, the error must be less than any prescribed positive real tolerance beyond some real cutoff. For a sequence limit, the error must be less than any prescribed positive rational tolerance, interpreted as a real, at all sufficiently large natural indices. A least upper bound is an upper bound that is at most every upper bound of the same set. [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field) [math:def-complete-ordered-field](https://alphabetamath.cc/item/def-complete-ordered-field) [math:def-limits-at-infinity](https://alphabetamath.cc/item/def-limits-at-infinity) [math:def-real-limit](https://alphabetamath.cc/item/def-real-limit) [math:def-rationals](https://alphabetamath.cc/item/def-rationals) [math:lem-rat-embeds-dense](https://alphabetamath.cc/item/lem-rat-embeds-dense)

[F7] For a real sequence $(B_j)$ and natural numbers $0\le h\le n$, finite-sum splitting gives $\sum_{j<n} B_j=\sum_{j<h}B_j+\sum_{h\le j<n}B_j$. The last sum is $\sum_{\ell<n-h}B_{h+\ell}$ by the shifted-index definition, including the empty sum when $h=n$. [math:lem-finite-sum-laws](https://alphabetamath.cc/item/lem-finite-sum-laws) [math:def-finite-sum](https://alphabetamath.cc/item/def-finite-sum)

[F8] For real $x,y$, $|xy|=|x|\,|y|$ and $|x+y|\le |x|+|y|$. [math:lem-of-abs-value](https://alphabetamath.cc/item/lem-of-abs-value) [math:lem-of-triangle-inequality](https://alphabetamath.cc/item/lem-of-triangle-inequality)

[F9] The real field is totally ordered with $1>0$. Adding a fixed real preserves order, and the product of positive reals is positive. [math:def-complete-ordered-real-field](https://alphabetamath.cc/item/def-complete-ordered-real-field)

## Proof

**Given:** $D,P,a,b$ and the counting function $C$ satisfy the hypotheses in the Statement.

**Goal:** Establish convergence of the series and improper integral, their equality with the factor $2$, and the stated upper bound.

1.1 For a natural number $n$, let $E_n=\{k\in D:P<k\le n\}$. It is a subset of $\{1,\ldots,n\}$, which is finite because $j\mapsto j+1$ from the first $n$ nonnegative integers is injective by cancellation and onto by taking $j=k-1$ for each $1\le k\le n$. For $j\ge0$ set $e_j=1$ if $j+1\in D$ and $j+1>P$, and $e_j=0$ otherwise. The equality $\#E_n=\sum_{j<n}e_j$ holds at $n=0$ since both sides are zero. Passing from $n$ to $n+1$ leaves $E_n$ unchanged when $e_n=0$ and adjoins exactly one element when $e_n=1$. In the latter case a bijection from the first $\#E_n$ nonnegative integers onto $E_n$ extends by sending the next integer to $n+1$. The extension stays injective because $n+1\notin E_n$ and is onto $E_{n+1}$ because the old images and the new image exhaust that set. Thus both sides obey the same recursion, so they agree by induction, using the real images of the cardinalities in the sum identity. For every $t\ge P$, the integer $\lfloor t\rfloor$ is nonnegative, so it is a natural index by [F2]. The set counted by $C(t)$ is $E_{\lfloor t\rfloor}$, which proves finiteness and gives $C(t)=A_{\lfloor t\rfloor}$, with $A_n=\sum_{j<n}e_j$. [F1, F2, F3]

1.2 If $z>0$, then $z^{-1}$ exists and is nonzero because $zz^{-1}=1$. If $z^{-1}<0$, then $z(-z^{-1})=-1$ would be positive by [F9]. Thus $z^{-1}>0$ by totality. For $0<x\le y$, multiplying by positive factors gives $0<x^2\le xy\le y^2$ and $0<x^3\le x^2y\le y^3$. For $r=2,3$, the identity $x^{-r}-y^{-r}=(y^r-x^r)(x^r)^{-1}(y^r)^{-1}$ has a nonnegative right-hand side because $y^r-x^r\ge0$ and both inverses are positive. Thus $0<y^{-r}\le x^{-r}$. [F9, algebra]

2.1 Let $f(t)=C(t)t^{-3}$ for $t\ge P$ and fix $P\le u<v$. For $t\in[u,v]$, step 1.2 gives $0<t^{-3}\le P^{-3}$ since $t\ge P>0$. Its range on $[u,v]$ has lower bound $0$ and upper bound $[a(v-P)+b]P^{-3}$, so $f$ is bounded. The integers in $[u,v]$ form a subset of the finite list $1,\ldots,\lfloor v\rfloor$, which is empty if $\lfloor v\rfloor=0$. For a noninteger $x\in[u,v]$ we have $\lfloor x\rfloor<x<\lfloor x\rfloor+1$, so for $t$ sufficiently close to $x$ we have $C(t)=C(x)$ by step 1.1. Since $t^{-3}$ is continuous on the nonzero reals by [F4], for every $\varepsilon>0$ we can further restrict $t$ so that $|t^{-3}-x^{-3}|<\varepsilon/(1+C(x))$. Then $|f(t)-f(x)|=C(x)|t^{-3}-x^{-3}|<\varepsilon$. Thus [F4] gives integrability of $f$ on $[u,v]$, and in particular $I(R)=\int_P^R f(t)\,dt$ exists for every $R>P$. [given, step 1.1, step 1.2, F1, F2, F4, F8]

3.1 By step 1.2, for $P\le u<v$ and $r=2,3$, we have $0<t^{-r}\le u^{-r}$ on $[u,v]$. Thus $0$ and $u^{-r}$ bound the range, so each power is bounded. The powers are continuous on the nonzero reals by [F4], and the continuity inequalities still hold on $[u,v]$. Thus the integrability criterion in [F4] applies with zero exceptions. Write $\min\{p,q\}$ for the lesser of $p$ and $q$ in the real total order, with their common value when $p=q$. For $c\in[u,v]$ and any real $\delta>0$, if $c<v$, take $t=c+\min\{\delta,v-c\}/2$, and if $c=v$, take $t=c-\min\{\delta,c-u\}/2$. In either case $t\in[u,v]$ and $0<|t-c|<\delta$, so every $c\in[u,v]$ is a limit point of the interval. For either $G(t)=t^{-1}$ or $G(t)=t^{-2}$, the difference quotient on $[u,v]\setminus\{c\}$ is the restriction of the quotient on the nonzero reals. For every positive real tolerance, the same punctured-limit radius from the larger domain works on $[u,v]$. The derivatives on $[u,v]$ are therefore $-t^{-2}$ and $-2t^{-3}$, respectively, including at the endpoints. These derivatives are integrable by linearity. Applying [F5] to the two derivatives and dividing by their respective scalar factors gives $\int_u^v t^{-2}\,dt=u^{-1}-v^{-1}$ and $\int_u^v t^{-3}\,dt=(u^{-2}-v^{-2})/2$. On $[P,R]$ we have $0\le f(t)\le a t^{-2}+(b-aP)t^{-3}$. The upper function is integrable by linearity. Comparison and the two evaluations give $0\le 2I(R)\le 2a(P^{-1}-R^{-1})+(b-aP)(P^{-2}-R^{-2})$. The last expression equals $a/P+b/P^2-[aR+a(R-P)+b]/R^2$. The subtracted numerator is nonnegative since $a,b\ge0$ and $R>P$, so $2I(R)\le a/P+b/P^2$. [given, step 1.2, step 2.1, F4, F5, F9]

4.1 For $P<R_1<R_2$, additivity and $f\ge0$ give $I(R_2)-I(R_1)=\int_{R_1}^{R_2}f\ge0$. The nonempty set of values $I(R)$ for real $R>P$ has a least upper bound $L$ by step 3.1. For every $\varepsilon>0$ there is $R_0>P$ with $I(R_0)>L-\varepsilon$, as otherwise $L-\varepsilon$ would be an upper bound smaller than $L$. For $R\ge R_0$, therefore, $L-\varepsilon<I(R)\le L$. This proves $\int_P^\infty f=L$ and $2L\le a/P+b/P^2$. [step 2.1, step 3.1, F5, F6]

4.2 Suppose $P\le u<v$ and $C(t)=c$ on $[u,v)=\{t:u\le t<v\}$. The functions $f$ and $ct^{-3}$ are integrable on $[u,v]$ and on every nondegenerate closed subinterval by step 2.1, step 3.1 and linearity. To show the two integrals over $[u,v]$ agree, split the interval at $v-\delta$ with $0<\delta<v-u$. The integrands agree on $[u,v-\delta]$. On the remaining interval both are between $0$ and $K=[a(v-P)+b]P^{-3}$, using step 1.2 and $0\le c=C(u)\le a(u-P)+b\le a(v-P)+b$. Their integrals over that interval are each between $0$ and $K\delta$, so the absolute difference over $[u,v]$ is at most $K\delta$ for every such $\delta$ and must be zero. Consequently $2\int_u^v f(t)\,dt=c(u^{-2}-v^{-2})$. [given, step 1.2, step 2.1, step 3.1, F5]

5.1 Let $m=\lfloor P\rfloor+1$, so $m>P$ and $m\ge1$. Interpret $m$ and each integer $N\ge m$ as natural indices by [F2]. Split $[P,N]$ at $m,m+1,\ldots,N$, using each endpoint once. On $[P,m)$ the count is zero, and on $[j,j+1)$ for integer $j\ge m$ it is $A_j$. By induction on the number of subintervals, repeated additivity from [F5] adds the values given by step 4.2. This gives $2I(N)=\sum_{j=m}^{N-1} A_j(j^{-2}-(j+1)^{-2})$, with an empty sum when $N=m$. With $w_j=(j+1)^{-2}$, Abel summation applies at $n=N\ge1$. In its remainder write $B_j=A_{j+1}((j+1)^{-2}-(j+2)^{-2})$. The sum is over $j<N-1$. By [F7] split it at $h=m-1$, which lies between $0$ and $N-1$. For $j<m-1$ we have $A_{j+1}=0$ by step 1.1 because $E_{j+1}$ is empty, so the initial sum is zero by the finite-sum recursion. In the remaining sum $j=m-1+\ell$ with $0\le\ell<N-m$, so $i=j+1=m+\ell$ gives the terms of the integral sum. If $m=1$ the initial sum is empty, and if $m=N$ the remaining sum is empty. Thus the Abel remainder equals $2I(N)$. Since $A_N=C(N)$, the finite partial sum $S_N=\sum_{j<N}e_j(j+1)^{-2}$ satisfies $S_N=C(N)/N^2+2I(N)$. [F1, F2, F3, F5, F7, step 1.1, step 4.2]

6.1 For integers $N\ge m$ the first term of the finite identity is bounded by $0\le C(N)/N^2\le a/N+b/N^2\le (a+b)/N$. Given a positive rational $\varepsilon$, use its positive real image in the following estimates and choose a real cutoff $M\ge P$ beyond which $|I(R)-L|<\varepsilon/4$ and with $M\ge2(a+b)/\varepsilon$. Every natural $N\ge\lfloor M\rfloor+1$ has $N>M$ by [F2] and $N\ge m$, so the finite identity and [F8] give $|S_N-2L|\le C(N)/N^2+2|I(N)-L|<\varepsilon$. The sum of the series is the limit of these partial sums, so it equals $2L=2\int_P^\infty C(t)t^{-3}\,dt\le a/P+b/P^2$, as required. [given, step 4.1, step 5.1, F2, F6, F8] ∎
