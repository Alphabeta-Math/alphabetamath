---
id: def-complex-self-dual-two-form-data
title: Complex self-dual forms and metric-dependent contraction
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - physics:def-emg-lorentzian-forms
  - physics:lem-emg-lorentz-hodge-calculus
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - math:def-direct-sum-model-of-complexification
  - math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle
  - math:def-smooth-section-local-section-and-support
  - math:def-vector-bundle-map-over-a-smooth-base-map
  - math:thm-sylvesters-law-of-inertia
  - math:def-countable-choice
dependency_roles:
  physics:def-emg-lorentzian-forms: mathematical-premise
  physics:lem-emg-lorentz-hodge-calculus: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  math:def-direct-sum-model-of-complexification: mathematical-premise
  math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle: mathematical-premise
  math:def-smooth-section-local-section-and-support: mathematical-premise
  math:def-vector-bundle-map-over-a-smooth-base-map: mathematical-premise
  math:thm-sylvesters-law-of-inertia: mathematical-premise
  math:def-countable-choice: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
sources:
  references:
    - title: Lecture Notes on General Relativity
      url: https://arxiv.org/pdf/gr-qc/9712019
      locator: §1, equations (1.87)–(1.88), PDF p. 30
      statement: The Hodge star maps p-forms to (n-p)-forms and its square is given by
        the metric-signature formula.
      hypotheses: An oriented nondegenerate metric and the stated form degree and
        dimension.
      reading_limits: Consulted only §1, equations (1.87)–(1.88) and the accompanying
        signature explanation on PDF p. 30. This is background for the Hodge
        convention; the bundle construction, complex extension and applications
        below are local arguments using the declared mathematical suppliers.
dependency_level: 0
---

## Definition

Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$: every countable family of nonempty sets has a choice function.

Let $(M,g,N,o)$ be a smooth, oriented and time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$. A real two-form is a smooth section of $\bigwedge^2T^*M$; a complex two-form is a section of its complexification and can be written uniquely as $U+iV$ with real two-forms $U,V$. Extend the metric Hodge star $\star_g$ complex linearly by $\star_g(U+iV)=\star_gU+i\star_gV$. In this convention a complex two-form $Z$ is called self-dual when $\star_gZ=-iZ$.

For a real two-form $F$, define its complex self-dual form by $\mathcal F=F+i\star_gF$. Raise both indices using the inverse metric and define the complex bilinear contraction $\mathcal F^2=\mathcal F_{ab}\mathcal F^{ab}$, with summation over both indices and without complex conjugation or a factor of one half.

Let $A:TM\to TM$ be a smooth fiberwise invertible real-linear bundle map over the identity. Its algebraic pullbacks are the covariant two-tensors $(A^*g)_p(u,v)=g_p(A_pu,A_pv)$ and $(A^*F)_p(u,v)=F_p(A_pu,A_pv)$ for $u,v\in T_pM$. The latter is again a real two-form. This pullback is defined fiberwise and $A$ need not be the differential of a diffeomorphism.

## Definition references

[[physics:def-emg-lorentzian-forms]]

[[physics:lem-emg-lorentz-hodge-calculus]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[math:def-direct-sum-model-of-complexification]]

[[math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle]]

[[math:def-smooth-section-local-section-and-support]]

[[math:def-vector-bundle-map-over-a-smooth-base-map]]

[[math:thm-sylvesters-law-of-inertia]]

[[math:def-countable-choice]]

## Facts & Assumptions

[A1] Assume the Axiom of Countable Choice $\mathrm{AC}_\omega$: every countable family of nonempty sets has a choice function, as defined in [[math:def-countable-choice]]. This is the background assumption of the geometric suppliers used in [F1] and [F2].

[F1] The oriented, time-oriented Lorentzian data and real differential forms are as in [[physics:def-emg-lorentzian-forms]].

[F2] The metric Hodge star is a smooth real-linear bundle map and satisfies $\star_g^2=-\operatorname{id}$ on real two-forms. [[physics:lem-emg-lorentz-hodge-calculus]]

[F3] The nondegenerate metric has an inverse, which raises tensor indices. [[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[F4] For a real vector space $V$, the direct-sum complexification has underlying pairs $(u,v)$, written $u+iv$, with $(a+bi)(u+iv)=(au-bv)+i(bu+av)$. [[math:def-direct-sum-model-of-complexification]]

[F5] Smooth real vector bundles are described by fibrewise linear local trivializations; a smooth section is a smooth right inverse to the bundle projection. A bundle map over the identity is a smooth map preserving the projection and linear on each fibre. [[math:def-smooth-vector-bundle-rank-fibre-and-trivial-bundle]], [[math:def-smooth-section-local-section-and-support]], [[math:def-vector-bundle-map-over-a-smooth-base-map]]

[F6] The intrinsic exterior pairing on real two-forms has component expression $\langle P,Q\rangle_g=\tfrac12P_{ab}Q^{ab}$. [[physics:lem-emg-lorentz-hodge-calculus]]

[F7] The inertia of a finite-dimensional real symmetric bilinear form is independent of its diagonalizing basis, so invertible real congruence preserves the numbers of positive, negative and zero entries. [[math:thm-sylvesters-law-of-inertia]]

## Justification

Here is the smooth complexification construction used in the Definition. Put $E=\bigwedge^2T^*M$. As a set over $M$, take $E_{\mathbb C}=\{(u,v)\in E\times E:\pi(u)=\pi(v)\}$ with projection $(u,v)\mapsto\pi(u)$, and equip each fibre with the scalar operations of [F4]. Each real local trivialization of $E$ gives coordinates $(p,u,v)\in U\times\mathbb R^6\times\mathbb R^6$ on this set. If the real transition matrix is $h(p)$, the pair transition is $(p,u,v)\mapsto(p,h(p)u,h(p)v)$. It is smooth with smooth inverse given by the inverse transition matrix; the identity and cocycle relations are inherited from those of $E$. Identifying $(u,v)$ with $u+iv\in\mathbb C^6$, this transition is complex-linear by [F4]. Thus these coordinates give the smooth complex vector bundle meant here, with underlying real bundle of rank twelve in the sense of [F5]. A section is smooth exactly when its two component sections are smooth, since both projection to the pair components and formation of the pair are smooth in these coordinates. Consequently every smooth complex two-form has unique globally defined real and imaginary smooth two-forms $U,V$.

For any smooth real-linear bundle map $S:E\to E$, define $S_{\mathbb C}(u+iv)=S(u)+iS(v)$. Uniqueness of the pair makes this well defined. Real linearity gives $S_{\mathbb C}((a+bi)(u+iv))=(aS(u)-bS(v))+i(bS(u)+aS(v))=(a+bi)S_{\mathbb C}(u+iv)$, so it is complex-linear. In the pair coordinates its matrix is the same smooth matrix of $S$ on both components, so it is smooth. Apply this construction to the map $\star_g$ of [F2]. By [F2], $\star_g\mathcal F=\star_gF-iF=-i\mathcal F$, so the stated name agrees with the chosen eigenvalue convention.

For real two-forms $P,Q$, use the inverse metric of [F3] in each covector slot to form $Q^{cd}=g^{ce}g^{df}Q_{ef}$. By [F6], the full contraction $C(P,Q)=P_{ab}Q^{ab}$ equals $2\langle P,Q\rangle_g$, so it is intrinsically defined and independent of the frame. Extend this real bilinear pairing complex bilinearly, using the unique real and imaginary parts just constructed. In particular $C(U+iV,U+iV)=C(U,U)-C(V,V)+i(C(U,V)+C(V,U))$. Its component expression is exactly the full sum in the Definition, with no conjugation and no factor of one half, so that expression is well defined in every frame.

The bundle map $A$ has the meaning in [F5], with base map $\operatorname{id}_M$. In any local frame its matrix entries $A^i{}_a$ are smooth, since they are components of the smooth map applied to the local basis sections. The pullback components are $(A^*g)_{ab}=g_{ij}A^i{}_aA^j{}_b$ and $(A^*F)_{ab}=F_{ij}A^i{}_aA^j{}_b$, hence smooth. The defining fibrewise evaluations are intrinsically bilinear, symmetric for $g$ and alternating for $F$, so these local expressions agree on overlaps and the latter defines a real two-form. If $(A^*g)_p(u,v)=0$ for every $v$, surjectivity of $A_p$ implies $g_p(A_pu,w)=0$ for every $w$, whence $A_pu=0$ and then $u=0$. Thus $A^*g$ is nondegenerate. Its matrix is $A_p^{\mathsf T}g_pA_p$, an invertible congruence, so [F7] gives the same signature $(-,+,+,+)$ as $g$. This reasoning uses only the fibrewise bundle map, with no assumption that it is a differential.

## External input

The Hodge definition and square formula in Carroll's Lecture Notes on General Relativity, §1, equations (1.87)–(1.88), PDF p. 30, provide independent background for the chosen convention. Only those equations and the accompanying signature explanation were consulted. The smooth Hodge map and its square used above are supplied by [F2]; the complex bundle, extension, contraction application and pullback justification are local constructions from [F1]–[F7].
