---
id: def-author-97780c2fed82-general-spacelike-surface-data
title: General spacelike two-surfaces, null gauges and fluxes
kind: definition
status: draft
origin: pipeline
domain: mathematics
deps:
  - physics:def-gr-smooth-lorentzian-objects
  - physics:def-gr-fx-null-screen-geometry
  - physics:def-gr-metric-selected-connection
  - math:def-riemannian-volume-form-on-an-oriented-manifold
  - math:prop-integration-over-an-oriented-embedded-submanifold
  - physics:lem-emg-lorentz-hodge-calculus
  - math:def-affine-connection-on-a-smooth-manifold
  - math:def-pullback-connection
  - math:thm-pullback-connection-is-well-defined-and-functorial
  - math:def-integral-of-a-compactly-supported-smooth-density
  - math:thm-density-integration-is-defined-without-an-orientation
  - math:def-countable-choice
dependency_roles:
  physics:def-gr-smooth-lorentzian-objects: mathematical-premise
  physics:def-gr-fx-null-screen-geometry: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  math:def-riemannian-volume-form-on-an-oriented-manifold: mathematical-premise
  math:prop-integration-over-an-oriented-embedded-submanifold: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  math:def-affine-connection-on-a-smooth-manifold: mathematical-premise
  math:def-pullback-connection: mathematical-premise
  math:thm-pullback-connection-is-well-defined-and-functorial: mathematical-premise
  math:def-integral-of-a-compactly-supported-smooth-density: mathematical-premise
  math:thm-density-integration-is-defined-without-an-orientation: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 0
---

## Definition

Assume Countable Choice $\mathrm{AC}_\omega$. Let $(M,g,N)$ be a smooth oriented, time-oriented Lorentzian four-manifold with signature $(-,+,+,+)$ and a smooth metric connection $\nabla$, meaning any $g$-compatible affine connection; torsion freedom is not assumed. Let $i:S\hookrightarrow M$ be a nonempty compact oriented smooth embedded two-manifold without boundary with positive-definite induced metric $q=i^*g$. No containing spacelike hypersurface is required. Supply a global ordered pair of future null normal fields $\ell,k$ with $g(\ell,k)=-1$; the choice of $\ell$ labels the outgoing direction. The library convention $g(\ell,k)=-2$ is converted by halving its second normal.

For tangent fields $u,v$ on $S$, identify them with their images under $di$ in metric pairings and interpret $\nabla_u\ell$ as $(i^*\nabla)_u\ell$ in the pullback tangent bundle $i^*TM$. Put $\chi_\ell(u,v)=g(\nabla_u\ell,v)$, $\theta_{(\ell)}=\operatorname{tr}_q\chi_\ell$ and $\Omega(u)=-g(k,\nabla_u\ell)$. A marginal outer trapped surface (MOTS) means $\theta_{(\ell)}=0$ everywhere; no sign for the other null expansion is added. Write $d\mu_q$ for the positive area density and $A=\int_S d\mu_q$. For a smooth real two-form $F$, use the chosen orientations to define $F|_{TS}=b\,dA_q$ and $(\star_gF)|_{TS}=e\,dA_q$, where $dA_q$ is the positive oriented area form. Set $Q_M=(4\pi)^{-1}\int_SF=(4\pi)^{-1}\int_Sb\,d\mu_q$ and $Q_E=(4\pi)^{-1}\int_S\star_gF=(4\pi)^{-1}\int_Se\,d\mu_q$.

## Definition references

[[physics:def-gr-smooth-lorentzian-objects]]

[[physics:def-gr-fx-null-screen-geometry]]

[[physics:def-gr-metric-selected-connection]]

[[math:def-riemannian-volume-form-on-an-oriented-manifold]]

[[math:prop-integration-over-an-oriented-embedded-submanifold]]

[[physics:lem-emg-lorentz-hodge-calculus]]

[[math:def-affine-connection-on-a-smooth-manifold]]

[[math:def-pullback-connection]]

[[math:thm-pullback-connection-is-well-defined-and-functorial]]

[[math:def-integral-of-a-compactly-supported-smooth-density]]

[[math:thm-density-integration-is-defined-without-an-orientation]]

[[math:def-countable-choice]]

## Facts & Assumptions

[A1] Countable Choice is assumed for the smooth tangent-bundle and time-orientation conventions of the Lorentzian and null-screen suppliers, the Hodge supplier's background hypotheses, and the density-integral construction. [[math:def-countable-choice]]

[F1] The Lorentzian and null-screen suppliers fix the spacelike-surface and future-null-pair conventions. Metric compatibility means clause (a) of the connection supplier. Connection-dependent null-screen assertions are used only in the metric-selected case; no symmetry of $\chi_\ell$ is assumed for a general metric connection. [[physics:def-gr-smooth-lorentzian-objects]] [[physics:def-gr-fx-null-screen-geometry]] [[physics:def-gr-metric-selected-connection]]

[F2] The Riemannian area form obeys $|dA_q|=d\mu_q$. Integration of an ambient two-form over $S$ means integration of its pullback, with compact support required on $S$ itself; the oriented integral has its finite-chart construction. The Lorentzian Hodge star is a smooth bundle map fixed by $g$ and the ambient orientation. [[math:def-riemannian-volume-form-on-an-oriented-manifold]] [[math:prop-integration-over-an-oriented-embedded-submanifold]] [[physics:lem-emg-lorentz-hodge-calculus]]

[F3] An affine connection is a connection on $TM$. For any smooth map $i$ and any connection on a vector bundle, the pullback prescription gives a frame-independent connection on the pullback bundle and satisfies $(i^*\nabla)_u(i^*s)=(\nabla s)(di(u))$ for local ambient sections $s$. No torsion or metric hypothesis is needed. [[math:def-affine-connection-on-a-smooth-manifold]] [[math:def-pullback-connection]] [[math:thm-pullback-connection-is-well-defined-and-functorial]]

[F4] Under Countable Choice, a compactly supported smooth density is integrated by a chart partition and the resulting finite sum of coefficient integrals is independent of charts and partition. This integral is finite, linear and strictly positive for a nonzero nonnegative density. [[math:def-integral-of-a-compactly-supported-smooth-density]] [[math:thm-density-integration-is-defined-without-an-orientation]]

## Justification

**Given:** The objects and hypotheses in the Definition, including Countable Choice.

**Goal:** Establish the assertions and well-definedness stated there.

1.1 Multiplying the library second null normal by $1/2$ changes its pairing with the first from $-2$ to $-1$ and preserves its future null direction. These are the supplied smooth normal fields; no global pair is inferred from local existence. [given, A1, F1]

1.2 The area form $dA_q$ is nowhere zero and smooth. Both pulled-back two-forms are smooth, since $F$, the Hodge star and $i$ are smooth. Thus each is uniquely a smooth scalar multiple of $dA_q$: in a positive surface chart, divide its coefficient by $\sqrt{\det q}>0$. The ratios agree on overlaps by the top-form transformation law, giving global smooth $b,e$. [A1, F2]

2.1 Apply the pullback construction to the connection on $TM$ and the smooth embedding $i$. In any pulled-back frame $e_a$, write $\ell=\ell^ae_a$ and let $\omega^a{}_b$ be the ambient connection matrix. Then $(i^*\nabla)_u\ell$ has coefficients $u(\ell^a)+\omega^a{}_b(di(u))\ell^b$, which are smooth and depend only on the section along $S$. Frame independence is supplied by the pullback theorem. If a local ambient extension of $\ell$ is used, the section identity gives the same formula; two such extensions agree after pullback, so their tangential derivatives agree. The connection's function-linearity in $u$, smooth metric pairing and invertibility of the positive matrix $q$ now make $\chi_\ell$, its $q$-trace and $\Omega$ well-defined smooth tensors or functions. In the metric-selected case, $\chi_\ell$ and $\theta_{(\ell)}$ coincide with the null-screen definitions; $\Omega$ is the independent local definition above. The general argument uses no torsion restriction. [A1, F1, F3, step 1.1]

2.2 Compactness of $S$ makes $d\mu_q$, $b\,d\mu_q$, $e\,d\mu_q$ and the pulled-back top forms compactly supported on $S$. Choose a common chart partition in positive surface charts. The localized coefficients of $b\,dA_q$ and $b\,d\mu_q$ are the same functions $\rho_j b\sqrt{\det q}$; their respective form and density integrals therefore have identical finite chart sums. Replacing $b$ by $e$ gives the second equality. The submanifold integral convention then proves both stated flux identities, with finite integrals. [A1, F2, F4, step 1.2]

3.1 The area density is nonzero and nonnegative because $S$ is nonempty and $q$ is positive definite. Strict positivity of density integration gives $A>0$. With ambient orientation fixed, reversing the surface orientation negates $dA_q$ and both oriented flux integrals, while leaving $d\mu_q$ and $A$ unchanged; equivalently $b,e$ both change sign. Thus both charges change sign and their squares are unchanged. [F2, F4, step 1.2, step 2.2] ∎
