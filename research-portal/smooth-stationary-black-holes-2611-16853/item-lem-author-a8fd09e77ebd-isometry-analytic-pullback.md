---
title: An arbitrary metric isometry transports analyticity and Killing fields
status: published
research_item: lem-author-a8fd09e77ebd-isometry-analytic-pullback
dependency_level: 0
sources:
  references:
    - title: Piotr T. Chruściel, Geometry of Black Holes (revised July 2018; August
        15, 2018 PDF)
      url: https://homepage.univie.ac.at/piotr.chrusciel/teaching/Black%20Holes/BlackHolesVienna.pdf
      locator: Appendix A.5, printed p. 233 (PDF p. 241), symmetric/nondegenerate
        two-tensors and signature; Appendix A.21, printed p. 305 (PDF p. 313),
        equation (A.21.1).
      statement: A symmetric covariant two-tensor is nondegenerate when its coordinate
        matrix has nonzero determinant. The pseudo-Riemannian convention fixes
        its signature. An isometry preserves the metric by pullback.
      hypotheses: A smooth manifold with a smooth symmetric nondegenerate covariant
        two-tensor; metric preservation is imposed on the smooth diffeomorphism
        used here.
      reading_limits: Read the cited passages in the web-extracted PDF text. A.21.1,
        printed p. 306, was also consulted for the local Killing convention. No
        general theorem on isometry groups or analyticity of isometries is
        imported; the transport argument below is local work.
---

## Prerequisites

- [math:def-real-analytic-germ-in-several-variables](https://alphabetamath.cc/item/def-real-analytic-germ-in-several-variables)
- [math:def-smooth-atlas](https://alphabetamath.cc/item/def-smooth-atlas)
- [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)
- [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)
- [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)
- [math:prop-pullback-of-covariant-tensors-is-smooth-and-functorial](https://alphabetamath.cc/item/prop-pullback-of-covariant-tensors-is-smooth-and-functorial)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows)
- [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)
- [math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism](https://alphabetamath.cc/item/def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism)
- [math:cor-diffeomorphism-pushforward-preserves-lie-brackets](https://alphabetamath.cc/item/cor-diffeomorphism-pushforward-preserves-lie-brackets)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [` Piotr T. Chruściel, Geometry of Black Holes (revised July 2018; August 15, 2018 PDF) · Appendix A.5, printed p. 233 (PDF p. 241), symmetric/nondegenerate two-tensors and signature; Appendix A.21, printed p. 305 (PDF p. 313), equation (A.21.1). `](https://homepage.univie.ac.at/piotr.chrusciel/teaching/Black%20Holes/BlackHolesVienna.pdf)


## Statement

Work in ZFC. Let $U$ and $V$ be smooth $n$-manifolds, $n\geq1$, with smooth pseudo-Riemannian metrics $g_U$ and $g_V$. Here such a metric is a smooth symmetric covariant two-tensor whose matrix in each coordinate chart has nonzero determinant, with a fixed signature on each connected component. Suppose $F:U\to V$ is an isometry onto $V$, meaning a smooth diffeomorphism satisfying $F^*g_V=g_U$.

A real-analytic atlas means a covering family of charts whose transition maps in both directions have components locally represented by convergent real power series. A compatible real-analytic structure is represented by such an atlas which is smoothly compatible with the given smooth atlas: every transition between charts of the two atlases, in either direction, is smooth. A metric is analytic in this structure when its components in the representing analytic charts are real analytic. Suppose $V$ carries such a compatible real-analytic structure and $g_V$ is analytic. Then pulling back its analytic atlas by $F$ gives $U$ a compatible real-analytic structure in which $g_U=F^*g_V$ is analytic.

For either metric, a smooth vector field $Y$ is Killing when $\mathcal L_Yg=\left.\frac{d}{dt}\right|_{t=0}\Phi_t^*g=0$, where $\Phi_t$ is its local flow. Isometries transport these fields in both directions: $Y$ is Killing for $g_U$ if and only if $F_*Y$ is Killing for $g_V$, where $(F_*Y)_{F(p)}=dF_p(Y_p)$. For all smooth vector fields $X,Y$ on $U$, one also has $F_*[X,Y]=[F_*X,F_*Y]$. No orientation, time orientation, prescribed symmetry generator, or completeness of the fields is required.

## Statement references

[math:def-real-analytic-germ-in-several-variables](https://alphabetamath.cc/item/def-real-analytic-germ-in-several-variables)

[math:def-smooth-atlas](https://alphabetamath.cc/item/def-smooth-atlas)

[math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)

[math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism](https://alphabetamath.cc/item/def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism)

[math:cor-diffeomorphism-pushforward-preserves-lie-brackets](https://alphabetamath.cc/item/cor-diffeomorphism-pushforward-preserves-lie-brackets)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Facts & Assumptions

[A1] ZFC supplies the axiom of choice, hence the countable choice assumed by the vector-field pushforward supplier for the canonical smooth tangent bundles. This convention is inherited by the bracket transport used below. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice) [math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism](https://alphabetamath.cc/item/def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism)

[F1] Real-analytic scalar germs have absolutely convergent multivariable power-series representatives; a vector-valued map is analytic componentwise. [math:def-real-analytic-germ-in-several-variables](https://alphabetamath.cc/item/def-real-analytic-germ-in-several-variables)

[F2] Atlas domains cover the manifold; smooth compatibility requires every cross-transition to be smooth. A diffeomorphism is a smooth bijection with smooth inverse and is a homeomorphism. [math:def-smooth-atlas](https://alphabetamath.cc/item/def-smooth-atlas) [math:def-diffeomorphism-and-local-diffeomorphism-of-manifolds](https://alphabetamath.cc/item/def-diffeomorphism-and-local-diffeomorphism-of-manifolds)

[F3] Smooth tensor fields are smooth sections of tensor bundles. The symmetric nondegenerate metric convention and metric preservation by pullback are the conventions recorded in Chruściel, Appendix A.5 and equation (A.21.1), at the locators in the source reference. [math:def-smooth-tensor-field](https://alphabetamath.cc/item/def-smooth-tensor-field)

[F4] Pullback inserts the differential into each covariant slot. For smooth composable maps it is smooth and satisfies $(G\circ H)^*T=H^*(G^*T)$ and $\operatorname{id}^*T=T$. [math:def-pullback-of-a-covariant-tensor-field](https://alphabetamath.cc/item/def-pullback-of-a-covariant-tensor-field) [math:prop-pullback-of-covariant-tensors-is-smooth-and-functorial](https://alphabetamath.cc/item/prop-pullback-of-covariant-tensors-is-smooth-and-functorial)

[F5] Every smooth vector field has a smooth local flow, unique on common local domains; its time slices are diffeomorphisms where defined. The tensor Lie derivative is its pullback derivative at zero. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) [math:thm-fundamental-theorem-on-flows](https://alphabetamath.cc/item/thm-fundamental-theorem-on-flows) [math:def-lie-derivative-of-a-tensor-field](https://alphabetamath.cc/item/def-lie-derivative-of-a-tensor-field)

[F6] Pushforward by a diffeomorphism is the smooth vector field defined by $(F_*Y)_{F(p)}=dF_p(Y_p)$. [math:def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism](https://alphabetamath.cc/item/def-pushforward-and-pullback-of-a-vector-field-by-a-diffeomorphism)

[F7] Diffeomorphism pushforward preserves Lie brackets of smooth vector fields. [math:cor-diffeomorphism-pushforward-preserves-lie-brackets](https://alphabetamath.cc/item/cor-diffeomorphism-pushforward-preserves-lie-brackets)

## Proof

**Given:** The smooth manifolds, metrics, isometry $F$, and compatible analytic atlas on $V$ in the Statement, with the ZFC convention above.

**Goal:** Transfer the analytic structure, metric analyticity, Killing fields, and brackets.

1.1 For each chart $x_i:D_i\to x_i(D_i)$ in the specified analytic atlas of $V$, use $\widetilde x_i=x_i\circ F$ on $F^{-1}(D_i)$. These are charts because $F$ is a homeomorphism; their domains cover $U$ because the $D_i$ cover $V$. On each overlap, $\widetilde x_j\circ\widetilde x_i^{-1}=x_j\circ x_i^{-1}$. Thus the transitions in both directions are the original analytic transitions, and the pulled-back charts form a real-analytic atlas in the stated sense. [given, F1, F2]

1.2 Let $Y$ be any smooth vector field on $U$ with local flow $\Phi_t$ and put $Z=F_*Y$. On the conjugate local domain define $\Psi_t=F\circ\Phi_t\circ F^{-1}$. It is smooth, has $\Psi_0=\operatorname{id}$, and satisfies the local flow composition law. Differentiating its curves gives $\frac{d}{dt}\Psi_t(q)=dF_{\Phi_t(F^{-1}(q))}Y_{\Phi_t(F^{-1}(q))}=Z_{\Psi_t(q)}$. It is therefore the local flow of $Z$ on this domain. [A1, F5, F6]

2.1 If $a$ is any chart in the given smooth atlas of $U$, the cross-transition $a\circ\widetilde x_i^{-1}=a\circ F^{-1}\circ x_i^{-1}$ is smooth on its domain, and so is its inverse $x_i\circ F\circ a^{-1}$. Indeed $x_i$ is a smooth chart for the given structure of $V$ by its assumed compatibility, and both $F$ and $F^{-1}$ are smooth. This proves compatibility with the original smooth structure of $U$. [given, F2, step 1.1]

2.2 Pullback functoriality and $\Psi_t\circ F=F\circ\Phi_t$ give $F^*(\Psi_t^*g_V)=\Phi_t^*(F^*g_V)$. Differentiating at zero gives $F^*(\mathcal L_Zg_V)=\mathcal L_Yg_U$; the fixed pullback commutes with this derivative because at each point it is a fixed linear map on tensor components. Pullback by $F$ is injective, with inverse pullback by $F^{-1}$. Consequently $\mathcal L_Yg_U=0$ if and only if $\mathcal L_Zg_V=0$, which proves Killing transport in both directions without assuming complete flows. [given, F4, F5, step 1.2]

3.1 The metric identity and pullback functoriality give $(\widetilde x_i^{-1})^*g_U=(x_i^{-1})^*g_V$. These are precisely the coordinate tensors of the two metrics, so the components of $g_U$ in $\widetilde x_i$ equal the analytic components of $g_V$ in $x_i$. Hence $g_U$ is analytic in the pulled-back structure. [given, F1, F3, F4, step 1.1, step 2.1]

4.1 For smooth $X,Y$, the bracket supplier gives $F_*[X,Y]=[F_*X,F_*Y]$. Together with the atlas construction and Killing equivalence this proves all the stated transport claims. The argument places no requirement on the image of any preferred generator. [A1, F6, F7, step 3.1, step 2.2] ∎

## External input

Chruściel supplies the metric and metric-preservation conventions at the recorded locators. The general Killing convention is defined above using the declared tensor Lie derivative. The analytic atlas is defined above from the declared atlas and analytic-germ interfaces. The transport proof is local; no analyticity theorem for isometries is imported.
