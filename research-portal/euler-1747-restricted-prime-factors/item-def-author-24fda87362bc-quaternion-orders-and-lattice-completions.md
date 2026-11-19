---
title: Quaternion orders and completed lattices
status: draft
research_item: def-author-24fda87362bc-quaternion-orders-and-lattice-completions
dependency_level: 1
---

## Prerequisites

- [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm)
- [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation)
- [math:def-subring](https://alphabetamath.cc/item/def-subring)
- [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis)
- [math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations)
- [math:def-left-and-right-modules](https://alphabetamath.cc/item/def-left-and-right-modules)
- [math:thm-change-of-basis-matrices-are-inverses](https://alphabetamath.cc/item/thm-change-of-basis-matrices-are-inverses)
- [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space)
- [math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary)
- [math:def-matrix-product-and-identity-matrix](https://alphabetamath.cc/item/def-matrix-product-and-identity-matrix)
- [math:thm-universal-property-of-module-tensor-products](https://alphabetamath.cc/item/thm-universal-property-of-module-tensor-products)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball)
- [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology)
- [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence)


## Definition

In the rational Hamilton algebra $B=B(\mathbb Q)$, a full integral lattice $L$ is the set of all integer linear combinations of a rational basis $b_1,\ldots,b_4$ of $B$. A rational basis means every element of $B$ has a unique expression as a rational linear combination of these four elements. An order $O$ in $B$ is a full integral lattice that is a unital subring of $B$, meaning it contains $1$ and is closed under addition, additive inverses and multiplication.

For a prime $\ell$, write $B_\ell=B(\mathbb Q_\ell)$, with $B$ embedded by the coefficient inclusion $\mathbb Q\subseteq\mathbb Q_\ell$. The completion $L_\ell$ of $L$ at $\ell$ is the set of $\mathbb Z_\ell$-linear combinations of $b_1,\ldots,b_4$ in $B_\ell$, or equivalently the image of $L\otimes_{\mathbb Z}\mathbb Z_\ell$ under $b\otimes t\mapsto tb$. In this tensor product, $L$ has the right action $b\cdot r=rb$ by integer scaling, and $\mathbb Z_\ell$ has the left action $r\cdot t=rt$ by multiplication by the embedded integer $r$, for $r\in\mathbb Z$. For the order $O$ write $O_\ell$ for this completion.

## Justification

The quaternion coordinates and multiplication come from [def-author-24fda87362bc-hamilton-algebra-and-reduced-norm](item-def-author-24fda87362bc-hamilton-algebra-and-reduced-norm). Rational basis coordinates restrict to unique integer coordinates on $L$, giving the free module basis of [math:def-free-module-on-a-set-and-standard-basis](https://alphabetamath.cc/item/def-free-module-on-a-set-and-standard-basis). The four standard vectors exhibit a full lattice when spanned over $\mathbb Z$, and their multiplication table makes that lattice an order by [math:def-subring](https://alphabetamath.cc/item/def-subring).

Let $e=(1,i,j,k)$ and $b=(b_1,\ldots,b_4)$. The rational coordinate matrix $P$ from $b$ to $e$ and the reverse matrix $Q$ satisfy $PQ=QP=I$ by [math:thm-change-of-basis-matrices-are-inverses](https://alphabetamath.cc/item/thm-change-of-basis-matrices-are-inverses). By [math:def-matrix-product-and-identity-matrix](https://alphabetamath.cc/item/def-matrix-product-and-identity-matrix), the product entries are $(PQ)_{ab}=\sum_{j=1}^4 P_{aj}Q_{jb}$ and $(QP)_{ab}=\sum_{j=1}^4 Q_{aj}P_{jb}$, and $I$ has diagonal entries $1$ and off-diagonal entries $0$. The field inclusion $\mathbb Q\subseteq\mathbb Q_\ell$ from [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation) preserves these sums, products, $0$ and $1$, so $PQ=QP=I$ also holds over $\mathbb Q_\ell$. The columns of $P$ are the standard coordinates of the $b_i$, so $P$ sends a column of local coefficients to the standard coordinates of the corresponding linear combination of the $b_i$. Its inverse $Q$ shows that the $b_i$ form a basis over $\mathbb Q_\ell$. A second integer basis of $L$ lies in the integer span of the first and conversely, giving the same local span because $\mathbb Z\subseteq\mathbb Z_\ell$.

The two integer actions satisfy the right and left module axioms of [math:def-left-and-right-modules](https://alphabetamath.cc/item/def-left-and-right-modules) by distributivity, scalar associativity and the action of $1$. The rule $(b',t)\mapsto tb'$ is additive in both variables by distributivity and integer-balanced since $t(b'\cdot r)=(r\cdot t)b'$. Applied to these $\mathbb Z$-modules and the additive group of $B_\ell$, [math:thm-universal-property-of-module-tensor-products](https://alphabetamath.cc/item/thm-universal-property-of-module-tensor-products) gives a unique additive map sending $b'\otimes t$ to $tb'$. The defining relations in [math:def-tensor-product-of-modules-by-generators-and-relations](https://alphabetamath.cc/item/def-tensor-product-of-modules-by-generators-and-relations) describe the inverse on its image. If $b'=\sum_i n_i b_i$ with $n_i\in\mathbb Z$, the same relations give $b'\otimes t=\sum_i b_i\otimes(n_i t)$. Combining terms with the same $b_i$ expresses every tensor as $\sum_i b_i\otimes t_i$. Thus the image is the local span, and uniqueness of the $b$-coordinates makes $\sum_i t_i b_i\mapsto\sum_i b_i\otimes t_i$ the inverse on that span.

For $u=e$ or $u=b$, write $[x]_{u,j}$ for the $j$th coordinate of $x$ in that basis and set $d_u(x,y)=\max_{1\le j\le4}|[x]_{u,j}-[y]_{u,j}|_\ell$. The extended absolute value on $\mathbb Q_\ell$ is multiplicative and satisfies the strong triangle inequality by [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field). Thus $d_u$ is a metric in the sense of [math:def-metric-space](https://alphabetamath.cc/item/def-metric-space). Separation and symmetry follow coordinatewise, and taking the maximum of the coordinate triangle inequalities gives $d_u(x,z)\le d_u(x,y)+d_u(y,z)$. For either coordinate matrix $A=P$ or $A=Q$, take $C_A=1+\max_{i,j}|a_{ij}|_\ell$. Applying multiplicativity and the strong triangle inequality to each entry $(Aw)_i=\sum_{j=1}^4 a_{ij}w_j$ gives
$$\max_i |(Aw)_i|_\ell\le C_A\max_j|w_j|_\ell.$$
Applying this to coordinate differences gives $d_e\le C_P d_b$ and $d_b\le C_Q d_e$. The open ball $B_{d_u}(x,r)$ consists of the points $y$ with $d_u(x,y)<r$, for $r>0$, by [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball). The comparisons give $B_{d_b}(x,r/C_P)\subseteq B_{d_e}(x,r)$ and $B_{d_e}(x,r/C_Q)\subseteq B_{d_b}(x,r)$. Thus the criteria for an open set in [math:def-metric-topology](https://alphabetamath.cc/item/def-metric-topology) agree for the two metrics. The standard quaternion coordinate topology is the metric topology of $d_e$.

By [math:def-metric-interior-closure-boundary](https://alphabetamath.cc/item/def-metric-interior-closure-boundary), a point is in the closure of $L$ exactly when every open ball around it meets $L$. For $x\in L_\ell$, set $t_j=[x]_{b,j}\in\mathbb Z_\ell$. Let $a_{j,n}$ be the representative in $\{0,\ldots,\ell^n-1\}$ of the residue of $t_j$ modulo $\ell^n$. For $m\ge n$, the lifts $a_{j,m}$ and $a_{j,n}$ differ by a multiple of $\ell^n$, so their distance is at most $\ell^{-n}$ by the rational absolute value formula. Step 1.2 of [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp) constructs the canonical embedding by taking the limit of these lifts in $\mathbb Q_\ell$. For any $r>0$, metric convergence in [math:def-metric-convergence](https://alphabetamath.cc/item/def-metric-convergence) gives an index $N_j$ for each $j$ such that $|a_{j,n}-t_j|_\ell<r$ for all $n\ge N_j$. Taking $n\ge\max_{1\le j\le 4}N_j$ gives $\sum_{j=1}^4 a_{j,n}b_j\in L$ at $d_b$-distance less than $r$ from $x$. Conversely, if $x\notin L_\ell$, some coordinate $[x]_{b,j}$ lies outside $\mathbb Z_\ell$, the closed unit ball of [def-author-24fda87362bc-local-adic-valuation](item-def-author-24fda87362bc-local-adic-valuation). For $d_b(x,y)<1$, if $[y]_{b,j}$ were in the unit ball, the strong triangle inequality would give $|[x]_{b,j}|_\ell\le\max(|[y]_{b,j}|_\ell,|[x]_{b,j}-[y]_{b,j}|_\ell)\le1$. Thus the open $d_b$-ball of radius $1$ around $x$ is disjoint from $L_\ell$, hence also from $L$. This establishes that $L_\ell$ is the closure of $L$ for the standard quaternion coordinate topology.

The products of basis vectors of $O$ belong to $O$. Expanding products over $\mathbb Z_\ell$ therefore gives $O_\ell O_\ell\subseteq O_\ell$, and $1\in O\subseteq O_\ell$. The local span is closed under addition and additive inverses as well, so $O_\ell$ is a unital subring.
