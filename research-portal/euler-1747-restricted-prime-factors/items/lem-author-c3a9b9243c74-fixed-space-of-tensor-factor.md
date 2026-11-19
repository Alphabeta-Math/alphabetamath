---
id: lem-author-c3a9b9243c74-fixed-space-of-tensor-factor
kind: lemma
title: Fixed vectors for an action on one Hilbert tensor factor
status: draft
domain: mathematics
deps:
  - math:def-balanced-and-bilinear-maps
  - math:def-real-and-complex-inner-product-space
  - math:thm-bounded-linear-operator-equivalences
  - math:def-countable-choice
  - math:def-hilbert-space
  - math:def-strongly-continuous-unitary-representation
  - math:lem-nrqm-composites-hilbert-tensor-construction
  - math:thm-orthogonal-decomposition-by-a-closed-subspace
  - math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces
  - math:def-topological-group
  - math:def-subgroup
  - math:thm-universal-property-of-module-tensor-products
  - math:thm-extension-of-a-bounded-map-from-a-dense-subspace
  - math:thm-complete-subspace-iff-closed
  - math:prop-pythagorean-parallelogram-and-polarisation-identities
  - math:def-linear-subspace
  - math:def-linear-combination-and-span
  - math:def-metric-interior-closure-boundary
  - math:cor-inner-product-induces-a-norm
  - math:def-cauchy-in-metric
  - math:def-continuous-map-top
  - math:def-topological-space
  - math:def-metric-topology
  - math:def-metric-convergence
  - math:def-sum-of-linear-subspaces
  - math:def-vector-space-of-linear-maps
  - math:prop-linear-maps-form-a-vector-space
  - math:def-group-action
  - math:def-group-homomorphism
  - math:lem-group-homomorphism-basic-properties
  - math:def-metric-ball
  - math:def-banach-space
formulation_deps:
  - math:def-real-and-complex-inner-product-space
  - math:def-countable-choice
  - math:def-hilbert-space
  - math:def-strongly-continuous-unitary-representation
  - math:lem-nrqm-composites-hilbert-tensor-construction
  - math:def-topological-group
  - math:def-subgroup
  - math:def-linear-subspace
  - math:def-metric-interior-closure-boundary
  - math:def-linear-combination-and-span
  - math:def-continuous-map-top
  - math:def-topological-space
  - math:def-metric-topology
  - math:def-vector-space-of-linear-maps
  - math:def-group-action
argument_deps:
  - math:def-balanced-and-bilinear-maps
  - math:def-real-and-complex-inner-product-space
  - math:thm-bounded-linear-operator-equivalences
  - math:def-countable-choice
  - math:def-hilbert-space
  - math:def-strongly-continuous-unitary-representation
  - math:lem-nrqm-composites-hilbert-tensor-construction
  - math:thm-orthogonal-decomposition-by-a-closed-subspace
  - math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces
  - math:thm-universal-property-of-module-tensor-products
  - math:thm-extension-of-a-bounded-map-from-a-dense-subspace
  - math:thm-complete-subspace-iff-closed
  - math:prop-pythagorean-parallelogram-and-polarisation-identities
  - math:def-linear-subspace
  - math:def-linear-combination-and-span
  - math:def-metric-interior-closure-boundary
  - math:cor-inner-product-induces-a-norm
  - math:def-cauchy-in-metric
  - math:def-continuous-map-top
  - math:def-topological-space
  - math:def-metric-topology
  - math:def-metric-convergence
  - math:def-sum-of-linear-subspaces
  - math:def-vector-space-of-linear-maps
  - math:prop-linear-maps-form-a-vector-space
  - math:def-group-action
  - math:def-group-homomorphism
  - math:lem-group-homomorphism-basic-properties
  - math:def-metric-ball
  - math:def-banach-space
dependency_roles:
  math:def-balanced-and-bilinear-maps: mathematical-premise
  math:def-real-and-complex-inner-product-space: mathematical-premise
  math:thm-bounded-linear-operator-equivalences: mathematical-premise
  math:def-countable-choice: mathematical-premise
  math:def-hilbert-space: mathematical-premise
  math:def-strongly-continuous-unitary-representation: mathematical-premise
  math:lem-nrqm-composites-hilbert-tensor-construction: mathematical-premise
  math:thm-orthogonal-decomposition-by-a-closed-subspace: mathematical-premise
  math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces: mathematical-premise
  math:def-topological-group: mathematical-premise
  math:def-subgroup: mathematical-premise
  math:thm-universal-property-of-module-tensor-products: mathematical-premise
  math:thm-extension-of-a-bounded-map-from-a-dense-subspace: mathematical-premise
  math:thm-complete-subspace-iff-closed: mathematical-premise
  math:prop-pythagorean-parallelogram-and-polarisation-identities: mathematical-premise
  math:def-linear-subspace: mathematical-premise
  math:def-linear-combination-and-span: mathematical-premise
  math:def-metric-interior-closure-boundary: mathematical-premise
  math:cor-inner-product-induces-a-norm: mathematical-premise
  math:def-cauchy-in-metric: mathematical-premise
  math:def-continuous-map-top: mathematical-premise
  math:def-topological-space: mathematical-premise
  math:def-metric-topology: mathematical-premise
  math:def-metric-convergence: mathematical-premise
  math:def-sum-of-linear-subspaces: mathematical-premise
  math:def-vector-space-of-linear-maps: mathematical-premise
  math:prop-linear-maps-form-a-vector-space: mathematical-premise
  math:def-group-action: mathematical-premise
  math:def-group-homomorphism: mathematical-premise
  math:lem-group-homomorphism-basic-properties: mathematical-premise
  math:def-metric-ball: mathematical-premise
  math:def-banach-space: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Statement

Assume Countable Choice. Let $V,W$ be complex Hilbert spaces, complete spaces for the norms from their inner products, and let $\rho$ be a strongly continuous unitary representation of a topological group $L$ on $V$. Thus $\rho$ acts by bijective complex-linear isometries with continuous vector orbit maps. The Hilbert tensor product $V\widehat\otimes W$ is the completion of the finite sums of elementary tensors with pairing $\langle v\otimes w,v'\otimes w'\rangle=\langle v,v'\rangle\langle w,w'\rangle$. Let $L$ act by $\rho(a)\otimes I_W$ for $a\in L$, where $I_W$ is the identity. For any subgroup $J\le L$, let $V^J$ be the vectors fixed by every element of $J$. Then
$$(V\widehat\otimes W)^J=V^J\widehat\otimes W$$
as closed subspaces of $V\widehat\otimes W$. If $W\ne0$, the left side is nonzero exactly when $V^J\ne0$. If a finite linear combination of operators $\rho(a)$ preserves $V^J$ and acts there by a scalar, the same combination of $\rho(a)\otimes I_W$ acts by that scalar on $(V\widehat\otimes W)^J$.

## Statement references

[[math:def-countable-choice|Countable Choice]]

[[math:def-hilbert-space|Hilbert spaces]]

[[math:def-real-and-complex-inner-product-space|Complex inner products]]

[[math:def-strongly-continuous-unitary-representation|Strongly continuous unitary representations]]

[[math:def-topological-group|Topological groups]]

[[math:def-group-action|Group actions]]

[[math:def-subgroup|Subgroups]]

[[math:lem-nrqm-composites-hilbert-tensor-construction|Hilbert tensor construction]]

[[math:def-linear-subspace|Linear subspaces]]

[[math:def-metric-interior-closure-boundary|Closed sets in the norm metric]]

[[math:def-linear-combination-and-span|Finite linear combinations]]

[[math:def-vector-space-of-linear-maps|Pointwise operations on linear maps]]

[[math:def-continuous-map-top|Continuity at a point]]

[[math:def-topological-space|Topologies and open sets]]

[[math:def-metric-topology|Norm topology]]

## Facts & Assumptions

[A1] Countable Choice supplies a choice function for any sequence of nonempty sets. It is assumed for the tensor construction, bounded extension, the passage from completeness to closedness, and orthogonal decomposition ([[math:def-countable-choice]]).

[F1] A Hilbert space is complete for the norm from its inner product. A strongly continuous unitary representation is a group homomorphism into the group of surjective complex-linear isometries with norm-continuous vector orbit maps ([[math:def-hilbert-space]], [[math:def-strongly-continuous-unitary-representation]]).

[F2] Under [A1], the Hilbert tensor product is the completion of the algebraic tensor product, which consists of finite sums of elementary tensors. The elementary tensor map is complex-bilinear, the product pairing is positive definite, and the elementary tensor norm is $\|v\|\,\|w\|$. Take all pairings linear in the first argument ([[math:lem-nrqm-composites-hilbert-tensor-construction]]).

[F3] Regard a complex vector space $E$ as a right $\mathbb C$-module by $x\cdot c=cx$. For complex vector spaces $E,F,P$, a complex-bilinear map $b:E\times F\to P$ is additive in each variable and satisfies $b(cx,y)=c\,b(x,y)=b(x,cy)$. These are the additivity and scalar-transfer conditions for balance ([[math:def-balanced-and-bilinear-maps]]). A balanced map to an abelian group induces a unique additive map on the algebraic tensor product with the prescribed values on elementary tensors ([[math:thm-universal-property-of-module-tensor-products]]).

[F4] Under [A1], a bounded linear map on a dense linear subspace extends uniquely to a bounded linear map on the whole normed space when its target is Banach. The extension has the same operator norm as the original map ([[math:thm-extension-of-a-bounded-map-from-a-dense-subspace]]). Any two such maps with a common dense restriction are both bounded extensions of that restriction and are therefore equal.

[F5] A closed subspace of a complete metric space is complete in the inherited metric. Under [A1], a complete subspace of any metric space is closed ([[math:thm-complete-subspace-iff-closed]]).

[F6] Every closed subspace $M$ in a Hilbert space gives the orthogonal decomposition $V=M\oplus M^\perp$ under [A1], where $M^\perp=\{u:\langle u,m\rangle=0\text{ for all }m\in M\}$ ([[math:thm-orthogonal-decomposition-by-a-closed-subspace]]).

[F7] The Cauchy–Schwarz inequality is $|\langle x,y\rangle|\le\|x\|\|y\|$ ([[math:thm-cauchy-schwarz-for-real-and-complex-inner-product-spaces]]).

[F8] Complex polarization recovers the inner product from the norm and complex scalar operations. For orthogonal vectors $x,y$, $\|x+y\|^2=\|x\|^2+\|y\|^2$ ([[math:prop-pythagorean-parallelogram-and-polarisation-identities]]).

[F9] The complex inner products are linear in the first argument and satisfy conjugate symmetry $\langle x,y\rangle=\overline{\langle y,x\rangle}$. In particular they are conjugate-linear in the second argument ([[math:def-real-and-complex-inner-product-space]]).

[F10] A bounded linear operator between normed spaces is continuous. If $C$ is a bound for $T$, then $\|Tx-Ty\|\le C\|x-y\|$ by linearity ([[math:thm-bounded-linear-operator-equivalences]], implication from boundedness to Lipschitz continuity).

[F11] A complex linear subspace contains zero and is closed under addition and complex scalar multiplication ([[math:def-linear-subspace]]).

[F12] A finite complex linear combination is a sum of a finite list of scalar multiples, including the empty sum, which is zero ([[math:def-linear-combination-and-span]]).

[F13] The norm closure of a set consists of the points whose every open norm ball meets that set. A set is closed for the norm metric if each point outside it has an open norm ball disjoint from the set ([[math:def-metric-interior-closure-boundary]], [[math:def-metric-topology]], [F22]).

[F14] The inner-product norm satisfies the triangle inequality and absolute homogeneity $\|c x\|=|c|\|x\|$ ([[math:cor-inner-product-induces-a-norm]]).

[F15] In a metric space a sequence is Cauchy if for every positive rational $\varepsilon$ all pairwise distances on some tail are less than $\varepsilon$ ([[math:def-cauchy-in-metric]]).

[F16] For a map from a topological space into a Hilbert space, continuity at a point is equivalent to the following condition. For each norm ball about the image, some open set containing the point maps into that ball. The open-set criterion gives this condition because norm balls are open. At a point $y$ with $\|y-c\|<r$, the triangle inequality puts the ball of radius $r-\|y-c\|$ about $y$ in the ball of radius $r$ about $c$. Conversely every open target set containing the image contains such a norm ball ([[math:def-continuous-map-top]], [[math:def-metric-topology]], [F14], [F22]).

[F17] A finite intersection of open sets is open, with the empty intersection taken to be the whole space ([[math:def-topological-space]]).

[F18] In the norm metric, a sequence $(x_n)$ converges to $x$ if for every positive rational $\varepsilon$ one has $\|x_n-x\|<\varepsilon$ for all sufficiently large $n$, and convergence implies these same bounds ([[math:def-metric-convergence]]).

[F19] For linear subspaces $A$ and $B$ of the same vector space, their sum is the linear subspace $A+B=\{x+y:x\in A,\ y\in B\}$ ([[math:def-sum-of-linear-subspaces]]).

[F20] For linear maps between the same two complex vector spaces, addition and scalar multiplication are pointwise ([[math:def-vector-space-of-linear-maps]]). In particular, $(\sum_i c_i U_i)(x)=\sum_i c_i U_i(x)$ and $(U-I)(x)=Ux-x$ for an endomorphism $U$. These operations yield linear maps ([[math:prop-linear-maps-form-a-vector-space]]).

[F21] A group homomorphism preserves products ([[math:def-group-homomorphism]]) and carries the identity to the identity ([[math:lem-group-homomorphism-basic-properties]]). For a left action, the identity acts trivially and the product acts by composition in the same order ([[math:def-group-action]]).

[F22] On a Hilbert space and its subspaces, the norm gives the metric $d(x,y)=\|x-y\|$ ([[math:def-banach-space]]). Thus the open norm ball centered at $x$ of radius $r>0$ is $B(x,r)=\{y:\|y-x\|<r\}$ by the open-ball definition and symmetry of the metric ([[math:def-metric-ball]]).

## Proof

**Given:** $L,\rho,V,W,J$ and [A1].

**Goal:** Identify the fixed vectors and the induced scalar action.

1.1 For $a\in L$, the prescription $(v,w)\mapsto\rho(a)v\otimes w$ is complex-bilinear by linearity of $\rho(a)$ and bilinearity of the elementary tensor map. By [F3] the prescription is balanced for the right action $v\cdot c=cv$, so it induces an additive map $T_{a,0}$ on $V\odot W$, the algebraic tensor product. For $c\in\mathbb C$, the relation $c(v\otimes w)=(cv)\otimes w$ and bilinearity give $T_{a,0}(c(v\otimes w))=cT_{a,0}(v\otimes w)$, and additivity gives homogeneity on finite sums. Since $\rho(a)$ is a complex-linear norm isometry, complex polarization gives $\langle\rho(a)v,\rho(a)v'\rangle=\langle v,v'\rangle$. Thus $T_{a,0}$ preserves the product pairing on elementary tensors and, by sesquilinearity, on finite sums. It extends by bounded linear extension from the dense algebraic tensor product into the complete space $V\widehat\otimes W$. Write this extension as $T_a=\rho(a)\otimes I_W$. Norm preservation extends by continuity. [A1, F1, F2, F3, F4, F8, F9, F10]

2.1 By [F1] and [F21], $\rho(a)\rho(b)=\rho(ab)$ and $\rho(e)=I_V$ for the identity $e\in L$. Thus $T_aT_b=T_{ab}$ and $T_e=I$ on elementary tensors by step 1.1 and on their span by linearity. In each equality the two maps are bounded linear maps into the completed tensor product with the same restriction to the dense algebraic tensor product. By [F4] the equalities hold on the whole tensor product. These are the left-action laws of [F21], and $T_aT_{a^{-1}}=T_e=T_{a^{-1}}T_a$ makes $T_{a^{-1}}$ the inverse of $T_a$. Fix $b\in L$, $z\in V\widehat\otimes W$, and $\varepsilon>0$. By density choose $z_0=\sum_i v_i\otimes w_i$ with $\|z-z_0\|<\varepsilon/4$ and set $s=\sum_i\|w_i\|$. For each term the orbit continuity in [F1], the criterion in [F16], and the ball formula in [F22] give an open set $U_i$ containing $b$ on which $\|\rho(a)v_i-\rho(b)v_i\|<\varepsilon/(2(1+s))$. The intersection of these finitely many open sets is an open set $U$ containing $b$ by [F17]. For $a\in U$, the norm of $T_a z_0-T_b z_0$ is bounded by $\sum_i\|\rho(a)v_i-\rho(b)v_i\|\,\|w_i\|$, which is at most $\varepsilon s/(2(1+s))<\varepsilon/2$. Since $T_a$ and $T_b$ are isometries, $\|T_a z-T_b z\|\le 2\|z-z_0\|+\|T_a z_0-T_b z_0\|<\varepsilon$. By [F16] the orbit map is continuous at $b$, proving strong continuity. [A1, F1, F2, F4, F14, F16, F17, F21, F22, step 1.1]

2.2 The space $M=V^J$ contains zero since each $\rho(a)$ is linear. If $x,y\in M$ and $\alpha,\beta\in\mathbb C$, then for each $a\in J$, $\rho(a)(\alpha x+\beta y)=\alpha\rho(a)x+\beta\rho(a)y=\alpha x+\beta y$. Thus $M$ is a complex linear subspace by [F11]. If $x\notin M$, some $a\in J$ gives $\delta=\|\rho(a)x-x\|>0$. By [F20], the pointwise difference $\rho(a)-I_V$ is linear. It has bound $2$ by the triangle inequality and the isometry property. For $\|y-x\|<\delta/2$, [F10] gives $\|\rho(a)y-y\|\ge\delta-2\|y-x\|>0$. By [F22] the ball of radius $\delta/2$ around $x$ misses $M$, so $M$ is closed by [F13]. It is complete in its inherited norm and hence is a Hilbert space for the restricted pairing. The complex-bilinear inclusion prescription $(m,w)\mapsto m\otimes w$ in $V\odot W$ is balanced by [F3] with the right action $m\cdot c=cm$. Its additive descent to $M\odot W$ is complex-linear by the scalar calculation in step 1.1. The restricted pairing gives equality of norms of all finite sums, so this inclusion extends isometrically to $M\widehat\otimes W$ by bounded extension into $V\widehat\otimes W$. Its image is complete by isometry and closed by [F5]. Denote this image by $A$. For $a\in J$, $T_a$ fixes each elementary tensor from $M\odot W$ and thus their span. The restriction of $T_a$ to $A$ and the inclusion of $A$ into the ambient Hilbert space are bounded linear maps that agree on the dense span of the elementary tensors in $A$. By [F4] they agree throughout $A$. [A1, F1, F2, F3, F4, F5, F10, F11, F13, F14, F20, F22, step 1.1]

2.3 Fix $w\in W$. The slice prescription $(v,w')\mapsto\langle w',w\rangle v$ is complex-bilinear since the pairing is linear in $w'$. By [F3] the prescription is balanced for $v\cdot c=cv$. Its additive descent is complex-linear by the scalar calculation in step 1.1, giving $S_{w,0}:V\odot W\to V$. On elementary tensors and then on finite sums $z$, the product pairing gives $\langle S_{w,0}z,u\rangle=\langle z,u\otimes w\rangle$ for $u\in V$. Taking $u=S_{w,0}z$ and using Cauchy–Schwarz gives $\|S_{w,0}z\|^2\le\|z\|\,\|S_{w,0}z\|\,\|w\|$, so $\|S_{w,0}z\|\le\|z\|\,\|w\|$, including when $S_{w,0}z=0$. The domain is dense and $V$ is complete, so bounded linear extension gives $S_w:V\widehat\otimes W\to V$. [A1, F1, F2, F3, F4, F7, F9, step 1.1]

3.1 For fixed $u$, the two sides of $\langle S_wz,u\rangle=\langle z,u\otimes w\rangle$ are linear functionals in $z$. By [F7] their bounds are $\|w\|\|u\|$ and $\|u\otimes w\|$ respectively, using the bound on $S_w$ from step 2.3 and the operator norm equality in [F4]. They agree on the dense algebraic tensor product by step 2.3. For $z_0$ in that subspace, the absolute value of their difference at $z$ is at most $(\|w\|\|u\|+\|u\otimes w\|)\|z-z_0\|$, by linearity, the bounds, and the triangle inequality. Density makes this upper bound arbitrarily small, so the functionals agree at $z$. The maps $S_wT_a$ and $\rho(a)S_w$ are bounded linear maps into $V$, with bound $\|w\|$ since the action operators are isometries. They agree on elementary tensors by the slice prescription and hence on the dense algebraic tensor product. By [F4] they agree everywhere. If $z$ is fixed by $J$, then $\rho(a)S_wz=S_wz$ for every $a\in J$, so $S_wz\in M$. For $u\in M^\perp$, conjugate symmetry gives $\langle S_wz,u\rangle=\overline{\langle u,S_wz\rangle}=0$, so the pairing identity gives $\langle z,u\otimes w\rangle=0$. [A1, F1, F2, F4, F6, F7, F9, F14, step 1.1, step 2.2, step 2.3]

3.2 Let $D$ be the set of finite complex linear combinations of the tensors $u\otimes w$ with $u\in M^\perp$ and $w\in W$, and let $B$ be the norm closure of $D$. The empty sum belongs to $D$, concatenating two finite sums gives their sum in $D$, and multiplying all coefficients by a scalar keeps the result in $D$. Thus $D$ is a linear subspace. Every ball centered at a point of $B$ meets $D$, so $D$ is dense in $B$. If $x\notin B$, there is an open ball of radius $r>0$ about $x$ disjoint from $D$. For every $y$ at distance less than $r/2$ from $x$, the ball of radius $r/2$ about $y$ lies in that ball by [F22] and the triangle inequality and is disjoint from $D$. Hence $y\notin B$, proving that $B$ is closed. Also $0\in D\subseteq B$. For $x,y\in B$, $\alpha,\beta\in\mathbb C$, and $\varepsilon>0$, choose $x',y'\in D$ with $\|x-x'\|,\|y-y'\|<\varepsilon/(1+|\alpha|+|\beta|)$. Then $\alpha x'+\beta y'\in D$, and the norm of its difference from $\alpha x+\beta y$ is at most $|\alpha|\|x-x'\|+|\beta|\|y-y'\|<\varepsilon$. By [F13], $\alpha x+\beta y\in B$, so $B$ is a closed linear subspace. [F1, F2, F6, F11, F12, F13, F14, F22, step 2.2]

4.1 The tensor pairing and sesquilinearity make the finite spans of the elementary tensors generating $A$ and $B$ orthogonal. Cauchy–Schwarz extends the orthogonality from these dense spans to $A$ and $B$. Thus $A\cap B=\{0\}$. By [F19] each term of a Cauchy sequence in $A+B$ has a decomposition $x_n+y_n$ with $x_n\in A$ and $y_n\in B$. Two decompositions differ by a vector in $A\cap B$, so these components are unique. Pythagoras applied to the differences gives $\|(x_n+y_n)-(x_m+y_m)\|^2=\|x_n-x_m\|^2+\|y_n-y_m\|^2$. Each component distance is at most $\|(x_n+y_n)-(x_m+y_m)\|$. For any positive rational $\varepsilon$, the tail on which this last distance is less than $\varepsilon$ also works for both components. By [F15] both component sequences are Cauchy. Since $A$ and $B$ are closed in a Hilbert space and hence complete, $x_n$ converges to some $x\in A$ and $y_n$ to some $y\in B$. For each positive rational $\varepsilon$, both component distances to their limits are less than $\varepsilon/2$ on a common tail by [F18]. The triangle inequality gives $\|(x_n+y_n)-(x+y)\|\le\|x_n-x\|+\|y_n-y\|<\varepsilon$ there. Since $x+y\in A+B$ by [F19], the sequence converges in $A+B$ by [F18]. Thus $A+B$ is complete and therefore closed under [A1]. [A1, F1, F2, F5, F7, F8, F9, F14, F15, F18, F19, step 2.2, step 3.2]

5.1 Decomposing the first factor by [F6] puts every elementary tensor in $A+B$. This sum is linear by [F19] and closed by step 4.1, so density gives $V\widehat\otimes W=A+B$. By step 3.1 and sesquilinearity, a fixed vector $z$ is orthogonal to $D$, and Cauchy–Schwarz extends this orthogonality to $B$. Writing it as $x+y$ with $x\in A$ and $y\in B$ gives $\langle z,y\rangle=\|y\|^2=0$, so $z\in A$. Together with step 2.2 this proves the fixed-space identity. [F2, F6, F7, F9, F19, step 2.2, step 3.1, step 3.2, step 4.1]

6.1 If $M=\{0\}$, all its elementary tensors vanish by bilinearity, and $A=\{0\}$. When $M$ and $W$ are both nonzero, $m\otimes w$ for nonzero $m,w$ has nonzero norm, proving the asserted equivalence for $W\ne0$. If $\sum_i c_i\rho(a_i)$ acts on $M$ by a scalar $\lambda$, then by [F20] and tensor bilinearity, $\sum_i c_i T_{a_i}(m\otimes w)=(\sum_i c_i\rho(a_i)m)\otimes w=\lambda(m\otimes w)$. Since each $T_{a_i}$ is an isometry, the norm laws give $\|\sum_i c_iT_{a_i}z\|\le(\sum_i |c_i|)\|z\|$. On $A$ the finite combination and $\lambda$ times the inclusion are bounded linear maps into the ambient Hilbert space. The combination agrees with $\lambda I$ on the dense span of these tensors in $A$, hence everywhere in $A$ by [F4]. [A1, F2, F4, F12, F14, F20, step 1.1, step 2.2, step 5.1] ∎
