---
id: lem-author-a4a441da4986-stationary-maximal-divergence
title: The stationary maximal vacuum divergence identity with the article sign
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-stationary-lorentzian-data
  - physics:thm-gr-constraint-equations-in-normal-frame
  - math:prop-gradient-hessian-and-divergence-connection-formulas
  - physics:thm-gr-killing-and-on-shell-matter-identities
  - math:def-product-connection-on-tensor-and-hom-bundles
  - math:prop-induced-connections-commute-with-contraction-and-permutation
  - physics:def-gr-curvature-tensor-and-derived-tensors
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  physics:thm-gr-constraint-equations-in-normal-frame: mathematical-premise
  math:prop-gradient-hessian-and-divergence-connection-formulas: mathematical-premise
  physics:thm-gr-killing-and-on-shell-matter-identities: mathematical-premise
  math:def-product-connection-on-tensor-and-hom-bundles: mathematical-premise
  math:prop-induced-connections-commute-with-contraction-and-permutation: mathematical-premise
  physics:def-gr-curvature-tensor-and-derived-tensors: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

On a smooth maximal spacelike hypersurface in a vacuum spacetime (here meaning $\operatorname{Ric}(g)=0$), decompose the stationary Killing field as $T=Nn+X$, use $k(U,V)=-g(\nabla_U n,V)$, and write $D$ for the Levi–Civita connection of the induced Riemannian metric $h$. Spatial indices range from $1$ to $3$, and are raised and lowered with $h$. Then
$$D_iX_j+D_jX_i=2Nk_{ij},\qquad D_i k^{ij}=0,\qquad D_i(k^{ij}X_j)=N|k|_h^2.$$
Here $|k|_h^2=h^{ia}h^{jb}k_{ij}k_{ab}$. These are conditional local identities on an already supplied maximal hypersurface; they do not construct it.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[def-stationary-lorentzian-data]]

[[physics:thm-gr-constraint-equations-in-normal-frame]]

[[math:prop-gradient-hessian-and-divergence-connection-formulas]]

[[physics:thm-gr-killing-and-on-shell-matter-identities]]

[[math:def-product-connection-on-tensor-and-hom-bundles]]

[[math:prop-induced-connections-commute-with-contraction-and-permutation]]

[[physics:def-gr-curvature-tensor-and-derived-tensors]]

## Facts & Assumptions

[F1] The hypersurface data fix $n,h,k,N,X$, maximality $\operatorname{tr}_h k=0$, and the stationary data fix the ambient metric-compatible connection and the local-flow Killing condition. [[def-spacelike-maximal-hypersurface-data]] [[def-stationary-lorentzian-data]]

[F2] For this Lorentzian ambient metric, Proof 1.1 of the constraint supplier proves $D_UV=(\nabla_UV)^\top$, hence $h(D_UV,W)=g(\nabla_UV,W)$ for tangent fields. Its Statement (c) gives $G(n,Y)=(\operatorname{div}_hK)(Y)-D_Y\operatorname{tr}_hK$, where $K(U,V)=g(\nabla_U n,V)=-k(U,V)$ is symmetric. [[physics:thm-gr-constraint-equations-in-normal-frame]]

[F3] Clause (a) characterizes $\mathcal L_Tg=0$ by the covariant Killing equation $g(\nabla_UT,V)+g(\nabla_VT,U)=0$. Its smooth oriented time-oriented Lorentzian four-dimensional hypotheses are supplied by the stationary data. [[physics:thm-gr-killing-and-on-shell-matter-identities]] [[def-stationary-lorentzian-data]]

[F4] On $T\Sigma$ and its dual use the product tensor connection induced by $D$. It differentiates tensor products by the Leibniz rule and commutes with contractions and permutations. Since $D$ is $h$-compatible, $Dh=0$; differentiating $h^{ia}h_{aj}=\delta^i{}_j$ with these rules also gives $Dh^{-1}=0$. [[math:def-product-connection-on-tensor-and-hom-bundles]] [[math:prop-induced-connections-commute-with-contraction-and-permutation]] [[def-spacelike-maximal-hypersurface-data]]

[F5] For the Riemannian metric $h$, the divergence of a smooth vector field $Y$ is the trace $D_iY^i$. [[math:prop-gradient-hessian-and-divergence-connection-formulas]]

[F6] The scalar curvature is $\operatorname{Scal}_g=g^{ab}\operatorname{Ric}_{ab}$ and the Einstein tensor is $G=\operatorname{Ric}-\tfrac12\operatorname{Scal}_g g$. These are geometric tensor definitions, independent of a physical field-equation postulate. [[physics:def-gr-curvature-tensor-and-derived-tensors]]

## Proof

**Given:** The smooth stationary Lorentzian data, the supplied maximal spacelike hypersurface, and the geometric vacuum hypothesis $\operatorname{Ric}(g)=0$, with the conventions and interfaces in [F1]–[F6].

**Goal:** Derive the three local identities with the displayed sign.

1.1 Apply the tangential projection identity in [F2] to the tangent shift $X$. It gives $g(\nabla_UX,V)=h(D_UX,V)$ for tangent $U,V$. Metric compatibility and the dual/product connection in [F4] identify the right side in components with $D_iX_j$. The projection identity is valid for a spacelike hypersurface in a Lorentzian manifold; no Riemannian ambient-metric hypothesis is used. [given, F1, F2, F4]

1.2 The hypothesis $\operatorname{Ric}(g)=0$ implies $\operatorname{Scal}_g=0$ and $G=0$ by [F6]. In [F2], $K=-k$ and maximality give $\operatorname{tr}_hK=0$, so its mixed normal projection yields $\operatorname{div}_hK=0$. Hence $h^{ia}D_i k_{aj}=0$. Raising $j$ and commuting the inverse metric with $D$ using [F4] gives exactly $D_i k^{ij}=0$. [given, F1, F2, F4, F6]

2.1 By [F3], $0=g(\nabla_UT,V)+g(\nabla_VT,U)$. Substitute $T=Nn+X$. The terms $U(N)g(n,V)$ and $V(N)g(n,U)$ vanish by normal orthogonality, and the two normal-derivative terms sum to $-2Nk(U,V)$, using the symmetry in [F2]. Step 1.1 converts the remaining terms to $h(D_UX,V)+h(D_VX,U)$. Thus $D_iX_j+D_jX_i=2Nk_{ij}$. [given, F1, F2, F3, step 1.1]

3.1 Set $Y^i=k^{ij}X_j$. By [F5] its divergence is $D_iY^i$. The tensor product and contraction rules of [F4] give $D_iY^i=(D_i k^{ij})X_j+k^{ij}D_iX_j$. Step 1.2 eliminates the first term. Symmetry of $k$ and step 2.1 give $k^{ij}D_iX_j=\tfrac12k^{ij}(D_iX_j+D_jX_i)=Nk^{ij}k_{ij}=N|k|_h^2$. This proves the final identity. Reversing the second fundamental form convention reverses the displayed divergence sign but leaves its zero-integral implication unchanged. [F2, F4, F5, step 2.1, step 1.2, algebra] ∎
