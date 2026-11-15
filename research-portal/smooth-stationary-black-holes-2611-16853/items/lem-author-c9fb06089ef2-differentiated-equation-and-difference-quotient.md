---
id: lem-author-c9fb06089ef2-differentiated-equation-and-difference-quotient
title: Tangential differentiated equations admit classical difference quotients
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation
  - math:def-holder-spaces-c-k-alpha-and-their-scaled-norms
  - math:def-ck-and-multi-index-notation-in-several-variables
  - math:lem-derivative-algebra-and-chain-rules
  - math:thm-continuous-partial-derivatives-imply-total-differentiability
  - math:thm-chain-rule-for-total-derivatives
  - math:thm-clairaut-schwarz-mixed-partials
  - math:cor-mean-value-theorem
  - math:thm-compactness-under-continuous-maps
  - math:cor-heine-borel-in-the-product-topology
dependency_roles:
  lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation: mathematical-premise
  math:def-holder-spaces-c-k-alpha-and-their-scaled-norms: mathematical-premise
  math:def-ck-and-multi-index-notation-in-several-variables: mathematical-premise
  math:lem-derivative-algebra-and-chain-rules: mathematical-premise
  math:thm-continuous-partial-derivatives-imply-total-differentiability: mathematical-premise
  math:thm-chain-rule-for-total-derivatives: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
  math:cor-heine-borel-in-the-product-topology: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 8
---

## Statement

Fix $0<\alpha<1$ and an integer $m\ge4$. Let $w\in C^{m,\alpha}$ solve the flattened smooth quasilinear equation $A^{ij}(x,w,Dw)w_{ij}+B(x,w,Dw)=0$, with zero height on the flat boundary. Work locally, shrinking the boundary chart to a half-ball $B_R^+=\{x\in\mathbb R^3:|x|<R,\ x_3>0\}$ whose closed graph-jet image lies in the smooth coefficient domain, and use $C^{m,\alpha}(\overline{B_R^+})$ for regularity up to that boundary. Repeated indices are summed. For a tangential multi-index $I$ of length $m-2$, set $v=D^Iw$. Then $v\in C^{2,\alpha}(\overline{B_R^+})$, has zero trace on $x_3=0$, and satisfies the classical linear equation $a^{ij}v_{ij}=f_I$, where $a^{ij}=A^{ij}(x,w,Dw)$ and $f_I\in C^{1,\alpha}(\overline{B_R^+})$.

Fix $0<r<R$ and $h_0=(R-r)/2$. For a tangential coordinate unit vector $e_t$ and every $0<|h|<h_0$, the quotient $\delta_hv(x)=(v(x+he_t)-v(x))/h$ is defined on $\overline{B_r^+}$, belongs to $C^{2,\alpha}(\overline{B_r^+})$, has zero flat-boundary trace, and satisfies
$$a^{ij}(x)(\delta_hv)_{ij}(x)=\delta_hf_I(x)-(\delta_ha^{ij})(x)v_{ij}(x+he_t).$$
Here $\delta_h$ always uses the same direction and shift. The right side, $\delta_hv$, and each first derivative of $\delta_hv$ have uniformly bounded $C^{0,\alpha}(\overline{B_r^+})$ norms for $0<|h|<h_0$. The corresponding equation and uniform bounds hold for arbitrary multi-indices $I$ of length $m-2$ and any fixed unit direction $e$ on nested interior balls $B_r\subset B_R$ in the coordinate domain, again for $0<|h|<(R-r)/2$; no boundary trace is asserted in the interior case.

## Facts & Assumptions

[F1] The flattened equation has smooth finite-dimensional coefficients on the local spacelike-jet domain, with smooth local extensions at the flat boundary, a positive principal matrix on compact admissible graph-jet neighborhoods, and homogeneous flat-boundary height; existing tangential derivatives have zero trace. [[lem-author-c9fb06089ef2-flattened-dirichlet-quasilinear-equation]]

[F2] The Hölder supplier defines the derivative suprema, top-order Hölder seminorm, and continuous up-to-boundary derivative convention. Product, composition, and quotient bounds used below are proved here from these definitions. [[math:def-holder-spaces-c-k-alpha-and-their-scaled-norms]]

[F3] Multi-indices and $C^k$ regularity have their coordinate meanings; the scalar product rule applied on coordinate lines can be iterated to differentiate finite products. [[math:def-ck-and-multi-index-notation-in-several-variables]] [[math:lem-derivative-algebra-and-chain-rules]]

[F4] Continuous partial derivatives give total differentiability, and the total chain rule differentiates a smooth finite-dimensional coefficient evaluated on a $C^1$ graph-jet map. [[math:thm-continuous-partial-derivatives-imply-total-differentiability]] [[math:thm-chain-rule-for-total-derivatives]]

[F5] Continuous second partial derivatives commute; applying this to lower derivative fields allows reordering at every derivative order already possessed by $w$. [[math:thm-clairaut-schwarz-mixed-partials]]

[F6] The real mean value theorem applies to a scalar function continuous on a closed segment and differentiable in its interior. We use it on coordinate segments, on segments in a convex coefficient neighborhood, and on differences of two translated scalar functions. [[math:cor-mean-value-theorem]]

[F7] Continuous real-valued functions on a nonempty compact space attain finite maxima and minima. [[math:thm-compactness-under-continuous-maps]]

[F8] Closed bounded subsets of finite-dimensional Euclidean space are compact. [[math:cor-heine-borel-in-the-product-topology]]

## Proof

**Given:** The hypotheses, chart, and nested radii in the Statement.

**Goal:** Prove the differentiated equation and the uniform bounds without assuming any additional derivative of $w$.

1.1 Write $[u]_\alpha=\sup_{x\ne y}|u(x)-u(y)|/|x-y|^\alpha$ and $\|u\|_{0,\alpha}=\|u\|_\infty+[u]_\alpha$ on the domain in question. The identity $p(x)q(x)-p(y)q(y)=p(x)(q(x)-q(y))+q(y)(p(x)-p(y))$ gives $[pq]_\alpha\le\|p\|_\infty[q]_\alpha+\|q\|_\infty[p]_\alpha$ and hence $\|pq\|_{0,\alpha}\le\|p\|_{0,\alpha}\|q\|_{0,\alpha}$. Iterating [F3] and using [F5] expresses every derivative of a product as a finite sum of products of derivative fields. On a bounded convex ball or half-ball, a derivative field with bounded first derivatives is Lipschitz by the chain rule along segments and [F6], and therefore is Hölder with seminorm at most its Lipschitz constant times the diameter to the power $1-\alpha$. The same estimates extend to the closure by continuity from interior points. Thus all lower derivatives as well as the top derivatives of a $C^{k,\alpha}$ field are Hölder, and the displayed product inequality applied to the differentiated products proves closure under finite products in $C^{k,\alpha}$. [F2, F3, F4, F5, F6, given, algebra]

1.2 For $x\in\overline{B_r^+}$ and $0<|h|<h_0$, every $x+she_t$, $0\le s\le1$, has norm at most $r+|h|<R$ and the same normal coordinate as $x$. Thus both endpoints and the connecting segment lie in the original chart, including its flat boundary when $x_3=0$. For any scalar $u\in C^{1,\alpha}(\overline{B_R^+})$ and any interior point $x$, apply [F6] to $t\mapsto u(x+te_t)$ on the interval with endpoints $0,h$ to obtain $|\delta_hu(x)|\le\|\partial_tu\|_\infty$. For two interior points $x,y\in B_r^+$ apply it instead to $t\mapsto u(x+te_t)-u(y+te_t)$ on the same interval. Its derivative is $\partial_tu(x+te_t)-\partial_tu(y+te_t)$, whose absolute value is at most $[\partial_tu]_{\alpha;B_R^+}|x-y|^\alpha$. Consequently $[\delta_hu]_{\alpha;B_r^+}\le[\partial_tu]_{\alpha;B_R^+}$ and $\|\delta_hu\|_{0,\alpha;B_r^+}\le\|\partial_tu\|_{0,\alpha;B_R^+}$. These bounds pass to flat-boundary points by continuous extension. This proves the uniform quotient estimate for both signs of $h$ directly, with no differentiability beyond $C^{1,\alpha}$. [F2, F3, F6, given, algebra]

2.1 Put $G(x)=(x,w(x),Dw(x))$, which is $C^{m-1,\alpha}$ by [F2] and [F5]. Use the smooth local extensions from [F1] at a boundary jet, and choose a closed coefficient-space ball $K$ centered at that jet, contained in an open ball on which those extensions are smooth. By continuity of $G$, shrink the chart so that $G(\overline{B_R^+})\subset K$. The ball $K$ is convex and compact by [F8]. For any smooth scalar coefficient $F$ among these extensions, every derivative of $F$ needed here and its next derivative are bounded on $K$ by [F7]. Applying [F4] and [F6] on coefficient-space segments makes each such derivative of $F$ Lipschitz on that ball. Thus its composite with $G$ is Hölder, since $G$ is Hölder. Repeatedly applying [F3] and [F4] expresses a derivative of order $j\le m-1$ of $F\circ G$ as a finite sum of a derivative of $F$ evaluated at $G$ times derivative fields of $G$ of orders at most $j$. The estimates in step 1.1 show that all these terms are Hölder and bounded; their continuous boundary extensions are given by the same expressions. In particular $a^{ij}$ and $b(x)=B(x,w,Dw)$ are $C^{m-1,\alpha}$ locally up to the flat boundary. [F1, F2, F3, F4, F5, F6, F7, F8, step 1.1, choose]

3.1 Differentiate $a^{ij}w_{ij}+b=0$ by $D^I$, using the iterated product rule and commuting only derivatives already supplied by $w\in C^{m,\alpha}$. With $J\le I$ denoting componentwise order and $\binom{I}{J}$ the product of the ordinary binomial coefficients, the result is $a^{ij}v_{ij}=f_I$, where $f_I=-D^Ib-\sum_{0<J\le I}\binom{I}{J}(D^Ja^{ij})D^{I-J}w_{ij}$. In every summand $1\le|J|\le m-2$, so $D^Ja^{ij}$ is at least $C^{1,\alpha}$ by step 2.1, while $D^{I-J}w_{ij}$ has order $m-|J|\le m-1$ and is at least $C^{1,\alpha}$. Also $D^Ib\in C^{1,\alpha}$. Step 1.1 therefore gives $f_I\in C^{1,\alpha}$. All $m$ derivatives needed for the left side already exist, so the equation is classical; continuity extends it to the flat boundary. Finally $v\in C^{2,\alpha}$ follows from the definition and [F5], and its zero trace follows from [F1] because $I$ is tangential. [F1, F2, F3, F5, step 1.1, step 2.1, algebra]

4.1 For each permitted fixed nonzero $h$, translation and subtraction preserve $C^{2,\alpha}$ regularity, and $D^\beta\delta_hv=\delta_hD^\beta v$ for $|\beta|\le2$ by differentiation of the two translates. Tangential shifts preserve the zero trace. Subtracting $a^{ij}(x)v_{ij}(x)=f_I(x)$ from the equation at $x+he_t$, and dividing by $h$, gives exactly the displayed equation after writing the shifted product difference as $a^{ij}(x)\delta_hv_{ij}+\delta_ha^{ij}(x)v_{ij}(x+he_t)$. Step 1.2 applied to $f_I$, to each $a^{ij}$, to $v$, and to each $v_j$ bounds $\delta_hf_I$, $\delta_ha^{ij}$, $\delta_hv$, and $D\delta_hv$ uniformly in $C^{0,\alpha}$. Translation does not enlarge the Hölder norm of $v_{ij}$ restricted from the larger chart, so step 1.1 bounds each product on the right uniformly. This uses $v_j\in C^{1,\alpha}$ and $v_{ij}\in C^{0,\alpha}$, never a third derivative of $v$. [F2, F3, step 1.1, step 2.1, step 3.1, step 1.2, algebra]

5.1 On nested interior balls the norm bound $|x+she|\le r+|h|<R$ holds for any fixed unit direction $e$, with no restriction on $I$. The composition, product, and differentiated-equation arguments are unchanged. For the quotient estimate replace $\partial_tu$ by $D_eu$, a fixed finite linear combination of first coordinate derivatives; it has the required $C^{0,\alpha}$ bound. Thus the same mean value calculation and product bound prove the interior assertion. Together these steps establish every claimed equation, trace, and uniform bound on the stated small-shift domains. [F2, F3, F4, F6, step 1.1, step 2.1, step 3.1, step 1.2, step 4.1, algebra] ∎
