---
id: lem-author-86990d62062f-closed-component-index
title: Compact extra components contribute index zero
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-exterior-weighted-elliptic-data
  - lem-author-86990d62062f-compact-domain-poisson
  - math:thm-sobolev-compactness-and-elliptic-estimates-give-fredholm-hodge-decomposition
  - math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations
  - math:thm-boundary-schauder-estimate-for-the-dirichlet-problem
  - math:thm-elliptic-differential-operators-on-compact-vector-bundles-have-parametrices-and-regularity
  - math:def-axiom-of-choice
  - math:thm-choice-implies-dependent-implies-countable-choice
  - math:def-riemannian-volume-density
  - math:thm-density-measure-integration-agrees-with-smooth-density-integration
  - math:thm-smooth-partitions-of-unity-exist-on-manifolds
  - math:prop-coordinate-formula-for-riemannian-divergence
  - math:lem-integral-of-a-divergence-of-an-l-one-c-one-field-vanishes
  - def-fredholm-continuation-data
  - math:thm-holder-spaces-on-bounded-domains-are-banach-spaces
  - math:thm-bounded-inverse-theorem
dependency_roles:
  def-exterior-weighted-elliptic-data: mathematical-premise
  lem-author-86990d62062f-compact-domain-poisson: mathematical-premise
  math:thm-sobolev-compactness-and-elliptic-estimates-give-fredholm-hodge-decomposition: mathematical-premise
  math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations: mathematical-premise
  math:thm-boundary-schauder-estimate-for-the-dirichlet-problem: mathematical-premise
  math:thm-elliptic-differential-operators-on-compact-vector-bundles-have-parametrices-and-regularity: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  math:thm-choice-implies-dependent-implies-countable-choice: mathematical-premise
  math:def-riemannian-volume-density: mathematical-premise
  math:thm-density-measure-integration-agrees-with-smooth-density-integration: mathematical-premise
  math:thm-smooth-partitions-of-unity-exist-on-manifolds: mathematical-premise
  math:prop-coordinate-formula-for-riemannian-divergence: mathematical-premise
  math:lem-integral-of-a-divergence-of-an-l-one-c-one-field-vanishes: mathematical-premise
  def-fredholm-continuation-data: mathematical-premise
  math:thm-holder-spaces-on-bounded-domains-are-banach-spaces: mathematical-premise
  math:thm-bounded-inverse-theorem: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Gilbarg and Trudinger, Elliptic Partial Differential Equations of Second
        Order (2001 reprint)
      url: https://djvu.online/file/jxRRleAzbYjsl
      locator: Chapter 6, section 6.4, Theorem 6.17, printed pp.109–110.
      statement: A classical C^2 solution of Lu=f has local C^{k+2,alpha} regularity
        if f and the elliptic operator coefficients have local C^{k,alpha}
        regularity.
      hypotheses: Integer k >= 0; 0 < alpha < 1; ellipticity; a classical solution on
        an open Euclidean set. Here k=2 on precompact smooth metric charts.
      reading_limits: Consulted the theorem statement and surrounding
        difference-quotient discussion in the online transcription. OCR has
        defects. Import only interior regularity; no reconstruction of its proof
        is claimed.
dependency_level: 2
---

## Statement

If the exterior definition permits extra compact components, there are only finitely many. A compact component with nonempty boundary contributes an invertible Dirichlet block. On a connected closed component the scalar Laplacian $C^{4,\alpha}\to C^{2,\alpha}$ has constants as kernel and the mean-zero functions as range, hence index zero. Consequently allowing these components does not change the index-zero conclusion on the full exterior.

## Facts & Assumptions

**Given:** the hypotheses in the Statement, $0<\alpha<1$, and the exterior conventions; work in ZFC.

[A1] Work in ZFC; full Choice supplies the DC and Countable Choice required by the analytic and integration inputs. [[math:def-axiom-of-choice]] [[math:thm-choice-implies-dependent-implies-countable-choice]]

[F1] The exterior has a compact core and exactly one specified noncompact end. [[def-exterior-weighted-elliptic-data]]

[F2] Compact components with nonempty boundary have the Dirichlet inverse. [[lem-author-86990d62062f-compact-domain-poisson]]

[F3] The compact boundaryless scalar Laplace-type Green operator has range orthogonal to its smooth kernel. [[math:thm-sobolev-compactness-and-elliptic-estimates-give-fredholm-hodge-decomposition]]

[F4] The interior Schauder estimate gives $C^{2,\alpha}$ regularity and a smaller-ball estimate for bounded classical $C^2$ solutions with $C^{0,\alpha}$ forcing. Its boundary counterpart supplies the second-order Dirichlet estimate used in the compact-domain construction. [[math:thm-interior-schauder-estimate-for-uniformly-elliptic-equations]] [[math:thm-boundary-schauder-estimate-for-the-dirichlet-problem]]

[F5] For the compact boundaryless operators under consideration, $H^k$ is defined by finite smooth localization, and $H^k\hookrightarrow C^r$ continuously if $k>r+3/2$. In particular $H^4\hookrightarrow C^2$ and $H^2\hookrightarrow C^0$. [[math:thm-elliptic-differential-operators-on-compact-vector-bundles-have-parametrices-and-regularity]]

[F6] The Riemannian density is $d\mu_h=\sqrt{\det h}\,|dx^1dx^2dx^3|$. Its integral is the partition-weighted coordinate integral, without an orientation; smooth subordinate partitions of unity exist. [[math:def-riemannian-volume-density]] [[math:thm-density-measure-integration-agrees-with-smooth-density-integration]] [[math:thm-smooth-partitions-of-unity-exist-on-manifolds]]

[F7] For $m=\sqrt{\det h}$, the coordinate divergence is $m^{-1}\partial_i(mX^i)$, also on nonorientable manifolds. A compactly supported $C^1$ vector field on $\mathbb R^3$ has integrable field and divergence and zero divergence integral. [[math:prop-coordinate-formula-for-riemannian-divergence]] [[math:lem-integral-of-a-divergence-of-an-l-one-c-one-field-vanishes]]

[F8] The finite-norm Euclidean closure Hölder spaces are Banach. A bounded linear bijection between Banach spaces has bounded inverse under DC. Fredholm index is kernel dimension minus cokernel dimension, with closed range required. [[math:thm-holder-spaces-on-bounded-domains-are-banach-spaces]] [[math:thm-bounded-inverse-theorem]] [[def-fredholm-continuation-data]]

[F9] Higher interior regularity for a classical solution is imported in External input.

## External input

Theorem 6.17 in the cited book supplies the higher interior regularity in [F9], with $k=2$. Only precompact Euclidean charts are used; the Hölder inverse estimate below is derived locally.

[Gilbarg–Trudinger, Theorem 6.17](https://djvu.online/file/jxRRleAzbYjsl).

## Proof

**Given:** the hypotheses in the Statement, $0<\alpha<1$, and the exterior conventions; work in ZFC.

**Goal:** prove the Statement.

**Proof technique:** direct.

1.1 Manifold components are open, since each point has a connected ball or half-ball neighborhood. Their intersections with the compact core $K$ form an open cover of $K$, so only finitely many components meet $K$. The connected tail $\{r>2r_0\}$ lies in one component. Every other component lies in $K$, is closed in the manifold, and hence is compact. Thus there are finitely many extra components. [F1]

1.2 Let $M$ be a connected closed component. For a $C^1$ vector field $X$, choose a finite smooth partition $(\chi_a)$ supported compactly inside precompact coordinate charts. In chart $a$ put $m_a=\sqrt{\det h}$ and extend the vector field with coefficients $m_a\chi_a X^i$ by zero to $\mathbb R^3$. This is $C^1$ and compactly supported, so [F7] gives zero integral of its Euclidean divergence. By [F6] and the coordinate formula, this is $\int_M\operatorname{div}_h(\chi_aX)\,d\mu_h=0$. Summing over $a$, the product rule and $\sum_a\chi_a=1$ give $\int_M\operatorname{div}_hX\,d\mu_h=0$. For real $C^2$ functions $u,v$, take $X=u\operatorname{grad}_h v$; expanding the same coordinate formula gives $\int_M u\Delta_hv\,d\mu_h=-\int_M h^{ij}(\partial_i u)(\partial_jv)\,d\mu_h$. Taking $u=1$ gives $\int_M\Delta_hv\,d\mu_h=0$. This proof uses densities throughout and needs no orientation. [A1, F1, F6, F7]

2.1 On any fixed compact component, use finitely many precompact coordinate balls or boundary half-balls and the usual closure Hölder norms, for $k=2,4$. A Cauchy sequence converges in each chart by [F8]; its local function and derivative limits agree on overlaps by their uniform convergence and the coordinate chain rule. They therefore define a global $C^{k,\alpha}$ limit, with convergence in the finite chart norm. This proves the needed Banach property. The zero-boundary subspace is closed because the norm controls the continuous boundary values. The coordinate formula for $\Delta_h$ has smooth coefficients on these compact patches, so it is a bounded linear map from that Dirichlet $C^{4,\alpha}$ space to $C^{2,\alpha}$. For a component with nonempty boundary, [F2] gives bijectivity; [F8] then gives a bounded inverse. The boundary estimate in [F4] is used only in that supplied compact-domain construction, not as an estimate on a closed component. [A1, F1, F2, F4, F8, step 1.1]

2.2 Use $P=-\Delta_h$ on the trivial real line bundle over $M$ with the positive density $d\mu_h$. Its smooth principal symbol is $h^{ij}\xi_i\xi_j>0$ for $\xi\ne0$, and step 1.2 makes it formally symmetric. These are precisely the compact, boundaryless, positive scalar-symbol hypotheses of [F3] and [F5]. The Green theorem makes the $H^2$ kernel smooth. For a member $v$ of that kernel, step 1.2 with $u=v$ gives $\int_M|dv|_h^2\,d\mu_h=0$. The integrand is continuous and nonnegative, and the density is positive in every chart, so $dv=0$ everywhere. A connected manifold is path connected, because its path components are open in connected coordinate neighborhoods; thus $v$ is constant. Conversely constants are in the kernel. Consequently [F3] gives a bounded Green map $G:H^k\to H^{k+2}$ on mean-zero data, for every integer $k\ge0$. [A1, F3, F5, F6, step 1.2]

3.1 If $f\in C^{2,\alpha}(M)$ and $\int_M f\,d\mu_h=0$, set $u=-Gf$. Finite smooth localization on compact charts puts $f$ in $H^2$, with $\|f\|_{H^2}\le C\|f\|_{C^{2,\alpha}}$: each localized derivative through order two is bounded on a bounded chart support. The Green bounds give $u\in H^4$, $\Delta_hu=f$, and $\int_Mu\,d\mu_h=0$. By [F5], $H^4\hookrightarrow C^2$ in dimension three, so this distributional equation is classical: its two sides are continuous and agree as distributions. Moreover $\|u\|_{C^0}\le C\|u\|_{H^2}\le C\|f\|_{L^2}\le C\|f\|_{C^0}$, by the $H^2\hookrightarrow C^0$ embedding and the $k=0$ Green bound. The hypotheses of [F9] now hold in each precompact chart: $L=\Delta_h=h^{ij}\partial_i\partial_j+b^j\partial_j$ is uniformly elliptic there with smooth coefficients, $f\in C^{2,\alpha}$, and $u\in C^2$. Theorem 6.17 with $k=2$ gives $u\in C^{4,\alpha}$ locally. A finite smaller-chart cover gives this regularity on $M$. [A1, F1, F3, F5, F6, F9, step 2.2]

4.1 To prove the Hölder inverse bound, fix nested coordinate balls $B_R\supset B_{R/2}\supset B_{R/4}\supset B_{R/8}$ with the closure of $B_R$ inside a chart. Write $a^{ij}=h^{ij}$ and $Lu=a^{ij}u_{ij}+b^ju_j=f$. By [F4], $\|u\|_{C^{2,\alpha}(B_{R/2})}\le C(\|f\|_{C^{0,\alpha}(B_R)}+\|u\|_{C^0(B_R)})$. All subsequent differentiations are legitimate by step 3.1. For a coordinate index $\ell$, $L(\partial_\ell u)=\partial_\ell f-(\partial_\ell a^{ij})u_{ij}-(\partial_\ell b^j)u_j$. Apply [F4] to this classical solution on $B_{R/2}$ and estimate products by $[pq]_\alpha\le\|p\|_\infty[q]_\alpha+[p]_\alpha\|q\|_\infty$. This gives $\|u\|_{C^{3,\alpha}(B_{R/4})}\le C(\|f\|_{C^{1,\alpha}(B_R)}+\|u\|_{C^0(B_R)})$. For $|\gamma|=2$, $L(D^\gamma u)=D^\gamma f-[D^\gamma,L]u$, where the commutator $[D^\gamma,L]=D^\gamma L-LD^\gamma$ has coefficients involving derivatives of $a,b$ through order two and applies derivatives of order at most three to $u$. Its $C^{0,\alpha}$ norm is bounded by $C\|u\|_{C^{3,\alpha}(B_{R/4})}$. One more application of [F4] on $B_{R/4}$ yields $\|u\|_{C^{4,\alpha}(B_{R/8})}\le C(\|f\|_{C^{2,\alpha}(B_R)}+\|u\|_{C^0(B_R)})$. Choose finitely many such inner balls covering $M$. Smooth coordinate transitions on their compact overlaps compare the finite chart norms by the chain rule and the same product inequality. Summation and the $C^0$ bound of step 3.1 give $\|u\|_{C^{4,\alpha}(M)}\le C_M\|f\|_{C^{2,\alpha}(M)}$. [F1, F4, F5, step 3.1]

5.1 The integral functional $f\mapsto\int_M f\,d\mu_h$ is continuous on $C^{2,\alpha}(M)$, since its absolute value is at most $\mu_h(M)\|f\|_{C^0}$. It is nonzero on constants because $0<\mu_h(M)<\infty$. Its kernel is therefore a closed codimension-one subspace: explicitly, every $f$ decomposes as its mean constant plus a mean-zero function. Step 1.2 shows the Laplacian range is contained in this kernel; step 3.1 proves equality. The $C^{4,\alpha}$ kernel is exactly the constants by step 1.2, and step 4.1 supplies the bounded inverse between the mean-zero subspaces. Thus the closed block is Fredholm with one-dimensional kernel and cokernel, hence index zero. [F1, F6, F8, step 2.1, step 1.2, step 3.1, step 4.1]

6.1 Only finitely many compact blocks occur by step 1.1. Their finite direct sum has closed range, kernel the direct sum of their kernels, and cokernel the direct sum of their cokernels. Indeed, in finitely many coordinates convergence is coordinatewise, so a product of closed ranges is closed, and quotienting the product range is the product of the coordinate quotients. Each nonempty-boundary block has index zero by step 2.1; each closed connected block has index zero by step 5.1. Hence their kernel and cokernel dimensions are equal and finite. Adding these blocks to the end-component operator adds equal amounts to the kernel and cokernel dimensions and preserves closedness of the range. Consequently, whenever the end-component operator has index zero, so does the full operator. This proves every assertion of the Statement. [F1, F8, step 1.1, step 2.1, step 5.1] ∎
