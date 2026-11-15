---
id: lem-author-ca4ffba327b3-normalized-boost-from-positive-lapse
title: The coefficient-one horizon generator inherits the positive lapse derivative
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-bifurcate-killing-horizon-data
  - def-circle-action-and-invariant-normal-data
  - physics:def-gr-metric-selected-connection
  - lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action
  - lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost
  - lem-author-9a15bef58785-affine-generator-acceleration
  - lem-author-9a15bef58785-killing-acceleration-covector
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  def-circle-action-and-invariant-normal-data: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action: mathematical-premise
  lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost: mathematical-premise
  lem-author-9a15bef58785-affine-generator-acceleration: mathematical-premise
  lem-author-9a15bef58785-killing-acceleration-covector: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 3
---

## Statement

Work in the smooth time-oriented Lorentzian four-dimensional setting of signature $(-,+,+,+)$ with its Levi–Civita connection $\nabla$. Let $S=\partial\Sigma$ be an embedded spacelike two-sphere bounding a smooth spacelike hypersurface $\Sigma$, smooth up to $S$, with future unit normal $n$ and unit normal $\nu$ to $S$ within $\Sigma$ pointing into the exterior section. Let $T,K,Z$ be smooth Killing fields near $S$, with $K=T+\Omega Z$, constant $\Omega$, and $K|_S=0$. Suppose $Z$ generates a smooth time-orientation-preserving circle action by isometries on an invariant neighborhood of $S$ and that this action preserves $S$. Put $N=-g(T,n)$. There is a circle fixed point $p\in S$ with $Z(p)=T(p)=0$ and $\nabla_vZ=0$ for every $v\in(T_pS)^\perp$. At any such pole the normal boost coefficient of $K$, specified by $\nabla_\nu K=a_p n$ and $\nabla_nK=a_p\nu$ at $p$, is $a_p=\nu(N)|_p$. Thus it is positive if the inward lapse derivative is positive there.

Moreover, suppose two distinct smooth embedded null hypersurfaces $H_+,H_-$ meet along $S$, with $T_qH_+\cap T_qH_-=T_qS$ for $q\in S$. On these respective branches suppose there are smooth nowhere-zero null normal generator fields $L_+,L_-$ and smooth functions $s$ on $H_+$ and $t$ on $H_-$ satisfying $\nabla_{L_+}L_+=\nabla_{L_-}L_-=0$, $L_+(s)=L_-(t)=1$, and $s^{-1}(0)=t^{-1}(0)=S$. Suppose $K=cK_0$ near $S$ for a real constant $c$ and a smooth field $K_0$ with $K_0|_{H_+}=sL_+$, $K_0|_{H_-}=-tL_-$, and $\nabla_\nu K_0=n$ on $S$ in the specified future/exterior normal convention. Then $c=a_p=\nu(N)|_p$. If this derivative is positive, $c>0$, $K$ is nonzero on $H_\pm\setminus S$, and the signed branch equations there are $\nabla_KK=cK$, $d(g(K,K))=-2cK^\flat$ on $H_+\setminus S$ and $\nabla_KK=-cK$, $d(g(K,K))=2cK^\flat$ on $H_-\setminus S$, where $K^\flat=g(K,\cdot)$. These are the signed surface-gravity equations of the resulting bifurcate Killing horizon. They extend as zero equations at $S$ and do not determine a coefficient from the zero equation alone. No existence of the additional branch and profile data is asserted.

## Statement references

[[def-spacelike-maximal-hypersurface-data]]

[[def-bifurcate-killing-horizon-data]]

[[def-circle-action-and-invariant-normal-data]]

[[physics:def-gr-metric-selected-connection]]

[[lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action]]

[[lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost]]

[[lem-author-9a15bef58785-affine-generator-acceleration]]

[[lem-author-9a15bef58785-killing-acceleration-covector]]

## Facts & Assumptions

[F1] The lapse is $N=-g(T,n)$, $g(n,n)=-1$, and the connection is metric compatible. Since $\nu$ is tangent to the spacelike hypersurface and normal to its boundary, $(n,\nu)$ is an orthonormal basis of the normal plane to $S$. [[def-spacelike-maximal-hypersurface-data]] [[physics:def-gr-metric-selected-connection]]

[F2] The circle-action definition supplies the generator and invariant-submanifold conventions. Its choice of least period $2\pi$ for a normalized action is not needed here: the circle-pole lemma requires a smooth time-oriented circle action by isometries on the embedded spacelike two-sphere. That lemma supplies a pole with $T=Z=0$ and trivial normal derivative of $Z$; the vanishing Killing field lemma supplies the normal boost form for $K$. [[def-circle-action-and-invariant-normal-data]] [[lem-author-ca4ffba327b3-sphere-pole-and-trivial-normal-action]] [[lem-author-ca4ffba327b3-vanishing-killing-field-normal-boost]]

[F3] The additional branch, nowhere-zero generator, affine geodesic, parameter, zero-set and $K_0$-normalization conditions are hypotheses of the second conclusion, not consequences of the horizon definition. For nonzero constant $c$, the affine-profile supplier gives opposite branch accelerations. For the ambient Killing field $K$, the covector supplier converts those accelerations into ambient covector equations. The bifurcate-horizon definition supplies the signed surface-gravity terminology on the nonzero-generator parts. [[def-bifurcate-killing-horizon-data]] [[lem-author-9a15bef58785-affine-generator-acceleration]] [[lem-author-9a15bef58785-killing-acceleration-covector]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the lapse/boost identity and its conditional signed horizon consequences.

1.1 The action is smooth, time-orientation preserving and isometric, and preserves the embedded spacelike two-sphere $S$, so the circle-pole lemma applies. It gives a pole $p$ with $T(p)=Z(p)=0$ and $\nabla_\nu Z=0$. The vanishing Killing field lemma applies to $K|_S=0$ and the orthonormal normal basis $(n,\nu)$ from [F1], giving $\nabla_\nu K=a_pn$ and $\nabla_nK=a_p\nu$ at $p$. [given, F1, F2]

2.1 Differentiate the lapse in the inward tangent direction at the boundary: $\nu(N)=-g(\nabla_\nu T,n)-g(T,\nabla_\nu n)=-g(\nabla_\nu T,n)$ at $p$ since $T(p)=0$. Also $\nabla_\nu K=\nabla_\nu T$ because $\Omega$ is constant and $\nabla_\nu Z=0$. Thus $\nu(N)|_p=-g(a_pn,n)=a_p$. This also proves the sign assertion. [F1, step 1.1]

3.1 Under the additional branch and profile hypotheses, the constant relation $K=cK_0$ gives $\nabla_\nu K=c\nabla_\nu K_0=cn$ at $p$. Comparing with step 1.1 yields $c=a_p=\nu(N)|_p$ for any real $c$. In the positive-derivative case this proves $c>0$, so in particular $c\ne0$ as required by the affine-profile supplier. [given, F1, step 1.1, step 2.1]

4.1 In that positive case the profiles $K=csL_+$ and $K=-ctL_-$, the nowhere-zero generators and the stipulated zero sets make $K$ nonzero on $H_\pm\setminus S$ and tangent and normal to each null branch. These complements are dense because the transverse intersection $S$ is a two-surface in each three-dimensional branch. The branches are therefore Killing horizons for the same ambient Killing field $K$, with bifurcation surface $S$. All affine-profile hypotheses in [F3] now hold, so $\nabla_KK=cK$ on $H_+$ and $\nabla_KK=-cK$ on $H_-$. The ambient covector identity in [F3] gives $d(g(K,K))=-2cK^\flat$ and $d(g(K,K))=2cK^\flat$, respectively. On their nonzero parts these specify the stated signed coefficients; at $S$, smoothness and $K=0$ give only the zero equations, which alone select no coefficient. [given, F3, step 3.1] ∎
