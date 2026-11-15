---
id: def-author-9f9c6144aed8-ik-sbs
title: Exact bifurcate-sphere package for the IK criterion
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-author-9f9c6144aed8-ik-af
  - def-bifurcate-killing-horizon-data
  - def-stationary-lorentzian-data
  - physics:lem-gr-fx-null-normal-plane-and-screen
  - math:prop-constant-rank-kernels-and-images-of-bundle-maps-over-one-base-are-subbundles
dependency_roles:
  def-author-9f9c6144aed8-ik-af: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  physics:lem-gr-fx-null-normal-plane-and-screen: mathematical-premise
  math:prop-constant-rank-kernels-and-images-of-bundle-maps-over-one-base-are-subbundles: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Ionescu–Klainerman, On the uniqueness of smooth, stationary black holes
        in vacuum
      url: https://arxiv.org/pdf/0711.0040
      locator: §1.2, SBS and footnotes 5–6, printed p. 7
      statement: SBS assumes transverse smooth non-expanding horizon branches and
        nontrivial tangential T on S0.
      hypotheses: The AF end and section are fixed.
      reading_limits: Consulted the arXiv v2 PDF text of section 1.2, SBS and
        footnotes 5–6 on printed/PDF p. 7. No page-image inspection or later
        analytic proof reconstruction is claimed. This citation supplies the SBS
        predicates only; quotient geometry and descent are justified below with
        the declared mathematical suppliers and a local argument.
dependency_level: 3
proof_strategy: direct
---

## Definition

For the end, section and exterior in [[def-author-9f9c6144aed8-ik-af]], set $S_0=\partial I^-(M^{\mathrm{end}})\cap\partial I^+(M^{\mathrm{end}})$. The **IK SBS package** requires $S_0\subset\Sigma_0$ to be an embedded two-sphere equal to $|x|=1$ under the chosen identification of $\Sigma_0$ with $\{|x|>1/2\}$. In a neighborhood $O$ of $S_0$, require $H^+=O\cap\partial I^-(M^{\mathrm{end}})$ and $H^-=O\cap\partial I^+(M^{\mathrm{end}})$ to be smooth embedded null hypersurfaces, each diffeomorphic to $S_0\times(-1,1)$, intersecting transversely in $S_0$. Require both to be non-expanding, meaning their null second fundamental forms have zero trace. Here the null second fundamental form is $\chi_L(X,Y)=g(\nabla_X L,Y)$ on the two-dimensional spacelike quotient of a null hypersurface by its null normal line, for a smooth nonzero null normal $L$; its trace uses the quotient's induced positive metric. Finally $T$ is tangent to both branches and is not identically zero on $S_0$. Nullness and transversality follow the conventions in [[def-bifurcate-killing-horizon-data]]; this package does not require $T$ itself to be a null generator.

## Facts & Assumptions

[F1] The AF package fixes the ambient smooth time-oriented Lorentzian four-manifold, end, section, exterior and stationary field, with the inherited ZFC conventions. [[def-author-9f9c6144aed8-ik-af]]

[F2] A smooth null hypersurface has a tangent metric with nonzero radical; its null normal line is that radical. The embeddedness and transversality conventions are those of [[def-bifurcate-killing-horizon-data]]. No Killing generator is assumed for either branch here.

[F3] The ambient metric has signature $(-,+,+,+)$, and its Levi–Civita connection is torsion-free and metric-compatible: $Xg(U,V)=g(\nabla_XU,V)+g(U,\nabla_XV)$ and $\nabla_XY-\nabla_YX=[X,Y]$. [[def-stationary-lorentzian-data]]

[F4] For a smooth null hypersurface whose tangent metric is positive semidefinite of rank two, the normal-screen supplier gives the smooth positive quotient $L^\perp/\mathbb RL$ and its identification with a transverse spacelike section. Derivatives of fields along the hypersurface use the pullback connection. Its Countable Choice assumption is supplied by the inherited ZFC convention. Only these clauses of [[physics:lem-gr-fx-null-normal-plane-and-screen]] are used; its affine-generator descent clause is replaced by the local argument below.

[F5] A smooth vector bundle map over the identity of a smooth base with constant fibre rank has a smooth kernel subbundle. In particular, a rank-two map from a rank-three bundle has a smooth rank-one kernel, with smooth nonzero local sections. [[math:prop-constant-rank-kernels-and-images-of-bundle-maps-over-one-base-are-subbundles]]

## Justification

**Given:** Either smooth null branch $H$ in the Definition, with its ambient Lorentzian metric and Levi–Civita connection. Work locally on $H$; the smooth nonzero null normal $L$ used below will be obtained in step 1.1.

1.1 At a point $p$, nondegeneracy of the ambient metric and codimension one give $\dim (T_pH)^\perp=1$. Choose a nonzero vector $L_p$ in the radical. Then $(T_pH)^\perp=\mathbb RL_p$ and $T_pH=L_p^\perp$. In a basis with metric $-(dx^0)^2+|dx|^2$, write $L_p=a(1,u)$ with $a\ne0$ and $|u|=1$. Every vector of $L_p^\perp$ is uniquely $(b,bu+v)$ with $u\cdot v=0$, and its squared norm is $|v|^2$. Thus the tangent metric is positive semidefinite of rank two with radical exactly $\mathbb RL_p$. View the induced metric as the smooth bundle map $b_H:TH\to T^*H$, $b_H(v)=g(v,\cdot)|_{TH}$. Its fibre rank is two by the preceding calculation, and its kernel is the radical. By F5 this kernel is a smooth line subbundle; choose a smooth nowhere-zero local section $L$. The quotient and its positive metric are therefore those in F4, reversing the sign of a local normal if needed for that supplier's future convention. In particular $\bar\gamma([X],[Y])=g(X,Y)$ is independent of representatives and positive definite. [given, F1, F2, F3, F4, F5, algebra]

2.1 For smooth tangent fields $X$ on $H$, the bracket $[L,X]$ is tangent to $H$. Metric compatibility and torsion freedom give $g(\nabla_LL,X)=-g(L,\nabla_LX)=-g(L,\nabla_XL+[L,X])=-\frac12Xg(L,L)=0$. Hence $\nabla_LL$ lies in $(TH)^\perp=\mathbb RL$: there is a smooth local scalar $\kappa$ with $\nabla_LL=\kappa L$. Smoothness follows by dividing a nonvanishing component of $L$ into the corresponding smooth component of $\nabla_LL$. This derives the required pregeodesic property for every such normal; it imposes no affine parametrization or Killing assumption. [given, F2, F3, step 1.1]

3.1 The pullback derivative $\nabla_XL$ depends only on $L$ along $H$: two smooth ambient extensions differ by a field vanishing on $H$, whose derivative in each tangent direction also vanishes there. The expression $\chi_L(X,Y)=g(\nabla_XL,Y)$ is bilinear in the tangent vectors. Metric compatibility gives $\chi_L(X,L)=\frac12Xg(L,L)=0$, while step 2.1 gives $\chi_L(L,Y)=\kappa g(L,Y)=0$. Changing either representative by a multiple of $L$ therefore leaves $\chi_L$ unchanged. It is symmetric because $\chi_L(X,Y)-\chi_L(Y,X)=-g(L,\nabla_XY-\nabla_YX)=-g(L,[X,Y])=0$. Thus it defines a smooth symmetric form on $TH/\mathbb RL$, and its trace uses the inverse of the positive quotient metric established in step 1.1. [given, F2, F3, F4, step 1.1, step 2.1]

4.1 Any other nonzero local normal is $fL$ for a smooth nowhere-zero function $f$. The connection product rule gives $\chi_{fL}(X,Y)=f\chi_L(X,Y)+X(f)g(L,Y)=f\chi_L(X,Y)$. The quotient metric is unchanged, so the trace is multiplied by $f$ and its vanishing is independent of the chosen local normal. This makes the non-expansion predicate well-defined on both branches. The remaining clauses prescribe embedded sets and tangencies without asserting existence of a horizon generator Killing field. [given, F1, F2, F3, step 1.1, step 3.1] ∎

## External input

The independent [Ionescu–Klainerman source](https://arxiv.org/pdf/0711.0040) supplies the SBS predicates in section 1.2, SBS and footnotes 5–6, printed/PDF p. 7. Only this geometric definition package is imported. The quotient well-definedness and normal-rescaling argument above are local; no existence, vacuum field equation or analytic theorem is inferred from recording these predicates.
