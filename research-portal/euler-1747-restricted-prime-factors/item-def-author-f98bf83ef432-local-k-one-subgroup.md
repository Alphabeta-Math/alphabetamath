---
title: Local congruence subgroup for the conductor
status: draft
research_item: def-author-f98bf83ef432-local-k-one-subgroup
dependency_level: 0
sources:
  references:
    - title: Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms
        at cusps
      url: https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf
      locator: §2.1.1 (PDF page 6), §2.1.4 equation (8) and §2.1.5 (PDF page 8), §3.1
        up to equation (22) (PDF pages 16–17)
      statement: Section 2.1.1 defines a uniformizer as a generator of the maximal
        ideal of $\mathfrak o$. For $K=\mathrm{GL}_2(\mathfrak o)$ and $n\ge 0$,
        equation (8) defines $K_1(n)$ by $c\in\varpi^n\mathfrak o$ and $a\in
        U_n$, and $K'_1(n)$ by $c\in\varpi^n\mathfrak o$ and $d\in U_n$. Here
        $U_n=1+\varpi^n\mathfrak o$ for $n>0$ and $U_0=\mathfrak o^\times$.
        Section 2.1.1 normalizes $|\varpi|=1/\#(\mathfrak o/\varpi\mathfrak o)$.
        Section 2.1.5 defines the conductor exponent using the unprimed group.
        Section 3.1 uses these unprimed local factors for the adelic newform and
        uses $\mathrm{GL}_2(\mathbb Z_p)$ at each prime $p$ of exponent zero.
      hypotheses: For the local subgroup definitions, $F$ is a nonarchimedean local
        field of characteristic zero with ring of integers $\mathfrak o$ and
        uniformizer $\varpi$. Section 2.1.5 defines the conductor for
        irreducible admissible generic representations of $\mathrm{GL}_2(F)$.
        The adelic setting of §3.1 is over $\mathbb Q$, with an irreducible
        unitary cuspidal representation, central character trivial on the
        positive reals, and a holomorphic discrete series of lowest weight
        $k\ge2$ at infinity.
      reading_limits: Checked the PDF text for the uniformizer definition, absolute
        value normalization, unit filtration, two matrix groups, choice of fixed
        subgroup for the conductor, and the local factors used in the adelic
        newform construction. The conjugation and transport of fixed points are
        proved here. This citation is used for the conventions.
    - title: J. S. Milne, Algebraic Number Theory (v3.08)
      url: https://www.jmilne.org/math/CourseNotes/ANTc.pdf#page=128
      locator: §7, Proposition 7.46 and Definition 7.48, printed page 126 (PDF page 128)
      statement: For a field complete for a discrete absolute value, the ring of
        integers is compact if and only if the residue field is finite.
        Definition 7.48 calls a field with a nontrivial absolute value a local
        field when it is locally compact for that absolute value.
      hypotheses: The compactness criterion assumes completeness for a discrete
        absolute value and takes the residue field of the corresponding ring of
        integers. The application uses the nonarchimedean $q$-adic absolute
        value on $\mathbb Q_q$.
      reading_limits: Checked the proposition and definition in the PDF. Only the
        finite-residue-field direction of the proposition is used. The local
        argument verifies its hypotheses and deduces local compactness.
    - title: J. S. Milne, Algebraic Number Theory (v3.08)
      url: https://www.jmilne.org/math/CourseNotes/ANTc.pdf#page=109
      locator: §7, paragraph immediately before Proposition 7.6, printed page 107 (PDF
        page 109)
      statement: An absolute value $|\cdot|$ on a field $K$ is discrete when
        $|K^\times|$ is a discrete subgroup of the positive reals under
        multiplication.
      hypotheses: The passage concerns an absolute value on a field in the
        nonarchimedean setting. The set being tested for discreteness consists
        of the values of the nonzero field elements.
      reading_limits: Checked the definition in the PDF text. Only the definition is
        used here. The isolation of the nonzero $q$-adic values is shown
        locally.
    - title: J. S. Milne, Algebraic Number Theory (v3.08)
      url: https://www.jmilne.org/math/CourseNotes/ANTc.pdf#page=117
      locator: §7, last paragraph before “Completions in the nonarchimedean case” and
        the opening discussion of that subsection, printed pages 115–116 (PDF
        pages 117–118)
      statement: The ring of integers of the completion $\mathbb Q_p$ of $\mathbb Q$
        for $|\cdot|_p$ is denoted by $\mathbb Z_p$. For a discrete
        nonarchimedean absolute value, the associated ring in the completion
        $\widehat K$ is $\{x\in\widehat K:|x|\le1\}$.
      hypotheses: The notation concerns the completion of $\mathbb Q$ for the $p$-adic
        absolute value. The ring description concerns a completion for a
        discrete nonarchimedean absolute value.
      reading_limits: Read the p-adic ring-of-integers notation and the description of
        the associated ring in the completion on the cited pages. The
        identification with compatible residue tuples uses the canonical
        embedding theorem cited in the inventory.
---

## Prerequisites

- [math:def-commutative-ring](https://alphabetamath.cc/item/def-commutative-ring)
- [math:def-matrices-over-a-commutative-ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)
- [math:def-semigroup-and-monoid](https://alphabetamath.cc/item/def-semigroup-and-monoid)
- [math:def-ring-homomorphism](https://alphabetamath.cc/item/def-ring-homomorphism)
- [math:def-field-of-p-adic-numbers](https://alphabetamath.cc/item/def-field-of-p-adic-numbers)
- [math:def-invertible-element](https://alphabetamath.cc/item/def-invertible-element)
- [math:def-prime-and-maximal-ideals](https://alphabetamath.cc/item/def-prime-and-maximal-ideals)
- [math:cor-maximal-ideal-and-residue-field-of-zp](https://alphabetamath.cc/item/cor-maximal-ideal-and-residue-field-of-zp)
- [math:def-locally-compact-metric-space](https://alphabetamath.cc/item/def-locally-compact-metric-space)
- [math:def-fixed-point-sets-of-a-group-action](https://alphabetamath.cc/item/def-fixed-point-sets-of-a-group-action)
- [math:def-g-module-over-a-commutative-ring](https://alphabetamath.cc/item/def-g-module-over-a-commutative-ring)
- [math:def-linear-subspace](https://alphabetamath.cc/item/def-linear-subspace)
- [math:def-linear-isomorphism-and-invertible-linear-map](https://alphabetamath.cc/item/def-linear-isomorphism-and-invertible-linear-map)
- [math:def-prime](https://alphabetamath.cc/item/def-prime)
- [math:def-p-adic-integers-as-compatible-residue-classes](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)
- [math:prop-integers-modulo-n-as-a-quotient-ring](https://alphabetamath.cc/item/prop-integers-modulo-n-as-a-quotient-ring)
- [math:def-group-power](https://alphabetamath.cc/item/def-group-power)
- [math:thm-generated-ideal-description-in-a-commutative-ring](https://alphabetamath.cc/item/thm-generated-ideal-description-in-a-commutative-ring)
- [math:def-invertible-matrix-and-similarity-over-a-commutative-ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)
- [math:def-ring-matrix-product-identity-and-transpose](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)
- [math:thm-ring-matrix-arithmetic-laws](https://alphabetamath.cc/item/thm-ring-matrix-arithmetic-laws)
- [math:prop-canonical-quotient-ring-map](https://alphabetamath.cc/item/prop-canonical-quotient-ring-map)
- [math:def-subgroup](https://alphabetamath.cc/item/def-subgroup)
- [math:thm-p-adic-completion-agrees-with-the-fraction-field-of-zp](https://alphabetamath.cc/item/thm-p-adic-completion-agrees-with-the-fraction-field-of-zp)
- [math:thm-p-adic-completion-is-a-field](https://alphabetamath.cc/item/thm-p-adic-completion-is-a-field)
- [math:def-p-adic-absolute-value-on-the-rationals](https://alphabetamath.cc/item/def-p-adic-absolute-value-on-the-rationals)
- [math:def-group-action](https://alphabetamath.cc/item/def-group-action)
- [math:def-ring-characteristic](https://alphabetamath.cc/item/def-ring-characteristic)
- [math:lem-metric-reverse-triangle](https://alphabetamath.cc/item/lem-metric-reverse-triangle)
- [math:def-metric-continuity](https://alphabetamath.cc/item/def-metric-continuity)
- [math:thm-continuous-image-of-a-compact-space-is-compact](https://alphabetamath.cc/item/thm-continuous-image-of-a-compact-space-is-compact)
- [math:def-vector-space](https://alphabetamath.cc/item/def-vector-space)
- [math:thm-standard-representatives-modulo-n](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)
- [math:def-integers-modulo-n](https://alphabetamath.cc/item/def-integers-modulo-n)
- [math:lem-monoid-units-form-a-group](https://alphabetamath.cc/item/lem-monoid-units-form-a-group)
- [math:def-left-right-and-two-sided-ideal](https://alphabetamath.cc/item/def-left-right-and-two-sided-ideal)
- [math:def-quotient-ring](https://alphabetamath.cc/item/def-quotient-ring)
- [math:def-multiplicative-absolute-value-on-a-field](https://alphabetamath.cc/item/def-multiplicative-absolute-value-on-a-field)
- [math:def-metric-ball](https://alphabetamath.cc/item/def-metric-ball)
- [math:def-metric-compactness](https://alphabetamath.cc/item/def-metric-compactness)
- [math:lem-p-adic-valuation-on-q](https://alphabetamath.cc/item/lem-p-adic-valuation-on-q)
- [math:lem-nat-embeds-int](https://alphabetamath.cc/item/lem-nat-embeds-int)
- [math:thm-well-ordering-principle](https://alphabetamath.cc/item/thm-well-ordering-principle)
- [` Andrew Corbett and Abhishek Saha, On the order of vanishing of newforms at cusps · §2.1.1 (PDF page 6), §2.1.4 equation (8) and §2.1.5 (PDF page 8), §3.1 up to equation (22) (PDF pages 16–17) `](https://webspace.maths.qmul.ac.uk/abhishek.saha/research/ramification-cusps.pdf)
- [` J. S. Milne, Algebraic Number Theory (v3.08) · §7, Proposition 7.46 and Definition 7.48, printed page 126 (PDF page 128) `](https://www.jmilne.org/math/CourseNotes/ANTc.pdf#page=128)
- [` J. S. Milne, Algebraic Number Theory (v3.08) · §7, paragraph immediately before Proposition 7.6, printed page 107 (PDF page 109) `](https://www.jmilne.org/math/CourseNotes/ANTc.pdf#page=109)
- [` J. S. Milne, Algebraic Number Theory (v3.08) · §7, last paragraph before “Completions in the nonarchimedean case” and the opening discussion of that subsection, printed pages 115–116 (PDF pages 117–118) `](https://www.jmilne.org/math/CourseNotes/ANTc.pdf#page=117)


## Definition

For a prime $q$, let $\mathbb Z_q$ be the ring of compatible residue tuples with coordinates in $\mathbb Z/q^j\mathbb Z$ for $j\ge1$, with componentwise ring operations. Write $[m]_{q^j}$ for the residue class of an integer $m$. When used in $\mathbb Z_q$, an integer $m$ denotes the tuple $([m]_{q^j})_{j\ge1}$.

For a commutative ring $R$, $\mathrm{GL}_2(R)$ is the group under matrix multiplication of two-by-two matrices $A$ over $R$ with a two-sided inverse $B$, so $AB=BA=I_2$. For each integer $n\ge0$, write $q^n$ for the natural power in the multiplicative monoid of $\mathbb Z_q$, with $q^0=1$, and $J_n=q^n\mathbb Z_q$ for the ideal of its multiples. Define
$$K_{1,q}(n)=\left\{\begin{pmatrix}a&b\\c&d\end{pmatrix}\in\mathrm{GL}_2(\mathbb Z_q): c\in J_n,\ d-1\in J_n\right\}.$$
For comparison, write $K^{\mathrm{top}}_{1,q}(n)$ for the group defined by the same conditions with $a-1\in J_n$ in place of $d-1\in J_n$.

## Definition references

[Commutative rings](https://alphabetamath.cc/item/def-commutative-ring)

[Matrices over a commutative ring](https://alphabetamath.cc/item/def-matrices-over-a-commutative-ring)

[Multiplicative monoids](https://alphabetamath.cc/item/def-semigroup-and-monoid)

[Prime integers](https://alphabetamath.cc/item/def-prime)

[Compatible residue tuples](https://alphabetamath.cc/item/def-p-adic-integers-as-compatible-residue-classes)

[Integer residue rings](https://alphabetamath.cc/item/prop-integers-modulo-n-as-a-quotient-ring)

[Invertible matrices over a commutative ring](https://alphabetamath.cc/item/def-invertible-matrix-and-similarity-over-a-commutative-ring)

[Matrix product and identity](https://alphabetamath.cc/item/def-ring-matrix-product-identity-and-transpose)

[Natural powers](https://alphabetamath.cc/item/def-group-power)

[Principal ideals](https://alphabetamath.cc/item/thm-generated-ideal-description-in-a-commutative-ring)

[Congruence classes of integers](https://alphabetamath.cc/item/def-integers-modulo-n)

[Quotient rings](https://alphabetamath.cc/item/def-quotient-ring)

[Two-sided ideals](https://alphabetamath.cc/item/def-left-right-and-two-sided-ideal)

[Associativity and identity for matrix multiplication](https://alphabetamath.cc/item/thm-ring-matrix-arithmetic-laws)

[The group of units of a monoid](https://alphabetamath.cc/item/lem-monoid-units-form-a-group)

[Subgroups](https://alphabetamath.cc/item/def-subgroup)

## Justification

Reduction from modulus $q^{j+1}$ to modulus $q^j$ is well defined since $q^{j+1}\mathbb Z\subseteq q^j\mathbb Z$. It preserves sums, products, additive inverses, zero and one because those operations and constants are computed on integer representatives. Thus the compatible tuples are closed under the componentwise operations, contain the constant residue tuples for zero and one, and inherit the commutative ring laws coordinate by coordinate. The tuple for an integer $m$ is compatible by reduction, and the representative formulas make the map from integers to tuples a unital ring homomorphism. The multiples of a single element of a commutative ring form its principal ideal, so $J_n$ is a two-sided ideal.

The two-by-two matrices over $R$ form a monoid under matrix multiplication, by associativity and the identity law. Its units are the matrices with two-sided inverses, so $\mathrm{GL}_2(R)$ is a group.

For $n\ge1$, the canonical projection $x\mapsto x+J_n$ is a unital ring homomorphism to the commutative ring $\mathbb Z_q/J_n$ with kernel $J_n$. Applying it to each entry preserves matrix products and the identity matrix by the entry formulas. It takes invertible matrices to invertible matrices since the reduced inverse is an inverse. The two defining congruences for $K_{1,q}(n)$ say exactly that the reduced matrix $M$ satisfies $(0,1)M=(0,1)$. For $K^{\mathrm{top}}_{1,q}(n)$ they say that $M$ fixes the column $\begin{pmatrix}1\\0\end{pmatrix}$ by left multiplication. Compatible matrix products are associative and the identity fixes the row and the column. A product of matrices fixing the given row or column also fixes it, and multiplying the fixed row or column equation by the inverse shows that the inverse fixes it too. Since entrywise reduction preserves the identity, products and inverses, both preimages are subgroups. For $n=0$, $J_0=\mathbb Z_q$ because $q^0=1$, so both groups are $\mathrm{GL}_2(\mathbb Z_q)$.

The field $\mathbb Q_q$ is the metric completion of $\mathbb Q$ for the $q$-adic metric, with the rationals embedded densely by constant sequences. The extended field operations agree with the rational operations on that embedding, and $\mathbb Q_q$ is a complete nonarchimedean valued field. For every positive integer $m$, the additive multiple $m\cdot1_{\mathbb Q_q}$ is the image of the nonzero rational integer $m$ under the unital embedding. Thus no positive multiple of the identity vanishes and $\mathbb Q_q$ has characteristic zero. Under the canonical embedding into the $q$-adic field $\mathbb Q_q$, $\mathbb Z_q$ is the closed unit ball, and the integer tuple for $q$ maps to the rational integer $q$ since the constant sequence $q$ has those residues. The $q$-adic absolute value extends the rational absolute value $|r|_q=q^{-v_q(r)}$ for $r\ne0$, with $|q|_q=q^{-1}$. The rational valuation $v_q$ is integer-valued, so the absolute value of each nonzero rational belongs to $q^{\mathbb Z}$. For $x\ne0$, let $(r_j)$ be a rational sequence representing $x$ in the completion. The reverse triangle inequality with third point $0$ gives $\bigl||r_j|_q-|x|_q\bigr|\le |r_j-x|_q$, so $|r_j|_q\to |x|_q$. Eventually these values are positive and lie in $[|x|_q/2,2|x|_q]$. They therefore lie in the finite set of integer powers of $q$ in that interval. Their limit is in that finite set, giving $|x|_q\in q^{\mathbb Z}$. Conversely, for each integer $k$, the rational power $q^k$ has $|q^k|_q=q^{-k}$. For nonnegative $k$ this follows from the power recursion and multiplicativity starting with $|1|_q=1$. For negative $k$ it follows by applying multiplicativity to $q^k q^{-k}=1$. The absolute value is nontrivial since $|q|_q=q^{-1}<1$.

In Milne's definition, the absolute value is discrete if the nonzero value group is a discrete subgroup of $\mathbb R_{>0}$ under multiplication. Since $q>1$, the interval $(q^{k-1},q^{k+1})$ meets $q^{\mathbb Z}$ only at $q^k$ for every integer $k$. Thus $|\cdot|_q$ is discrete.

In the closed unit ball, an element of absolute value one is a unit because its inverse has absolute value one. An element of absolute value less than one cannot have an inverse in the ball, since a product of such an element and any element of the ball has absolute value less than one. The values below one are at most $q^{-1}$, so dividing an element of absolute value below one by $q$ gives an element of the ball. Conversely multiplication by $q$ sends the ball to elements of absolute value below one. Every proper ideal contains only nonunits, because an ideal containing a unit contains one. Hence the proper ideal $q\mathbb Z_q$ of all nonunits is the unique maximal ideal. Its generator $q$ is a uniformizer. The residue field $\mathbb Z_q/q\mathbb Z_q$ is canonically $\mathbb F_q=\mathbb Z/q\mathbb Z$. Since $q$ is positive, each class modulo $q$ has exactly one representative in $0,\ldots,q-1$, so the residue field has order $q$. [Standard representatives modulo a positive integer](https://alphabetamath.cc/item/thm-standard-representatives-modulo-n)

Milne denotes the ring of integers of the $q$-adic completion by $\mathbb Z_q$ and identifies the associated ring in a completion for a discrete nonarchimedean absolute value with the closed unit ball. The absolute value on $\mathbb Q$ is discrete since its nonzero values are also exactly $q^{\mathbb Z}$. Under the canonical embedding above, our compatible residue ring is therefore the ring of integers in Proposition 7.46. Milne's Proposition 7.46 applies to this complete discretely valued field with finite residue field and gives compactness of the unit ball $\mathbb Z_q$. For fixed $x\in\mathbb Q_q$, translation by $x$ is continuous because $|(x+y)-(x+z)|_q=|y-z|_q$ for all $y,z\in\mathbb Q_q$, so one can take $\delta=\varepsilon$ in the metric continuity condition. By the continuous-image theorem, the translate $x+\mathbb Z_q$ of the compact unit ball is compact. It contains the open ball of radius one about $x$. Thus $\mathbb Q_q$ is locally compact and satisfies the characteristic-zero nonarchimedean local-field hypothesis of Corbett and Saha with ring of integers $\mathbb Z_q$, uniformizer $q$, and normalization $|q|_q=q^{-1}$.

For positive $n$, Corbett and Saha's equation (8) specialized to $\mathbb Q_q$ calls our bottom-row group $K'_1(n)$ and calls $K^{\mathrm{top}}_{1,q}(n)$ by the name $K_1(n)$, using $U_n=1+J_n$. They use the unprimed convention for the conductor and the adelic newform. Section 3.1 explicitly uses the full integral group at exponent zero.

For $n\ge1$, set $t=q^n$ and $W_n=\begin{pmatrix}0&1\\-t&0\end{pmatrix}\in\mathrm{GL}_2(\mathbb Q_q)$. Its inverse is $-t^{-1}W_n$ since $W_n^2=-tI_2$ and $t$ is nonzero in the field. Matrix multiplication gives
$$W_n\begin{pmatrix}a&b\\c&d\end{pmatrix}W_n^{-1}=\begin{pmatrix}d&-c/t\\-tb&a\end{pmatrix}.$$
If $A$ belongs to either subgroup, its entry $c$ is a multiple of $t$, so $-c/t$ is integral. All other entries of the conjugate are integral by the displayed formula. Since the subgroup contains $A^{-1}$, the same calculation shows that $W_nA^{-1}W_n^{-1}$ is integral. Multiplying the two conjugates shows that it is the inverse of $W_nAW_n^{-1}$. The lower left entry $-tb$ lies in $J_n$, and the two diagonal entries are exchanged, so the conjugate satisfies the other subgroup's congruences. The entry formulas over the commutative field $\mathbb Q_q$ give $(-tI_2)A=A(-tI_2)$ for every two-by-two matrix $A$, since both products multiply each entry of $A$ by $-t$. As $W_n^2=-tI_2$, conjugating twice is the identity. Thus conjugation carries $K^{\mathrm{top}}_{1,q}(n)$ onto $K_{1,q}(n)$.

The canonical embedding of rings sends an integral matrix and its integral inverse to mutually inverse matrices over $\mathbb Q_q$, so the two integral subgroups act by restriction of an action of $\mathrm{GL}_2(\mathbb Q_q)$.

For any left action of $\mathrm{GL}_2(\mathbb Q_q)$, the action of $W_n$ carries the points fixed by $K^{\mathrm{top}}_{1,q}(n)$ bijectively onto the points fixed by $K_{1,q}(n)$, with inverse given by $W_n^{-1}$. Indeed, if $h$ fixes $x$, then $(W_nhW_n^{-1})\cdot(W_n\cdot x)=W_n\cdot x$ by the action law. Let $V$ be a vector space over a field $F$ and let $\mathrm{GL}_2(\mathbb Q_q)$ act on $V$ by $F$-linear maps. The common fixed points of either subgroup form a linear subspace. The zero vector is fixed, and if every $h$ in the subgroup fixes $v$ and $w$, then $h\cdot(\alpha v+\beta w)=\alpha v+\beta w$ for all scalars $\alpha,\beta$. The actions of $W_n$ and $W_n^{-1}$ are linear on the ambient space, so their restrictions to the respective fixed subspaces are mutually inverse linear maps. This gives a linear isomorphism of the fixed spaces.

At exponent zero the fixed spaces for our groups and the full integral factor of §3.1 are identical. The unit conditions in equation (8) with $U_0=\mathbb Z_q^\times$ also give the full integral fixed space if imposed literally on the matrices at exponent zero. If $a$ is a nonunit in an invertible integral matrix $A$, the reduction of $A$ modulo $q\mathbb Z_q$ has nonzero first column and hence $c$ is a unit. For $U=\begin{pmatrix}1&1\\0&1\end{pmatrix}$, both $UA$ and $U^{-1}$ have unit upper-left entry, since $a+c$ is a unit. Thus $A=U^{-1}(UA)$ is a product of two matrices with unit upper-left entry. For a nonunit $d$, the same argument uses the nonzero second column and $L=\begin{pmatrix}1&0\\1&1\end{pmatrix}$, so that both $LA$ and $L^{-1}$ have unit lower-right entry. In each case, the factorization expresses $A$ as a product of two matrices satisfying the chosen unit condition. Any vector fixed by all matrices satisfying that condition is fixed by both factors. By the action law their product fixes the vector, so the full integral group fixes it. The two conventions therefore give the same set $S$ of nonnegative integer exponents admitting a nonzero fixed vector. The order-preserving embedding $\iota:\mathbb N\to\mathbb Z$ has image the nonnegative integers. If $S$ is nonempty, $\iota^{-1}(S)$ has a least element by well-ordering, and its image under $\iota$ is the least exponent for both conventions.
