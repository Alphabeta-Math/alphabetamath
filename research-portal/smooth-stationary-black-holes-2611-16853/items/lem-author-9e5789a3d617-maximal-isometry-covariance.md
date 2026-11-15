---
id: lem-author-9e5789a3d617-maximal-isometry-covariance
title: Isometries preserve maximality and transported boundary
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-spacelike-maximal-hypersurface-data
  - math:cor-diffeomorphism-pushforward-preserves-lie-brackets
  - math:cor-diffeomorphisms-preserve-interior-and-boundary
  - math:thm-fundamental-theorem-on-flows
  - math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global
  - math:cor-mean-value-theorem
  - physics:lem-timelike-cone-has-two-convex-components
  - math:def-pullback-of-a-covariant-tensor-field
  - math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary
  - math:def-embedded-smooth-submanifold-with-boundary
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:cor-diffeomorphism-pushforward-preserves-lie-brackets: mathematical-premise
  math:cor-diffeomorphisms-preserve-interior-and-boundary: mathematical-premise
  math:thm-fundamental-theorem-on-flows: mathematical-premise
  math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global: mathematical-premise
  math:cor-mean-value-theorem: mathematical-premise
  physics:lem-timelike-cone-has-two-convex-components: mathematical-premise
  math:def-pullback-of-a-covariant-tensor-field: mathematical-premise
  math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary: mathematical-premise
  math:def-embedded-smooth-submanifold-with-boundary: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 1
---

## Statement

Let $\phi:M\to M$ be a time-orientation-preserving isometry of $(M,g)$, meaning a diffeomorphism satisfying $\phi^*g=g$ whose differential maps future timelike vectors to future timelike vectors, and let $\widehat\Sigma$ be a smooth embedded spacelike hypersurface with boundary $S$. With the future unit normal and convention $k(U,V)=-g(\nabla_U n,V)$, the induced metric and second fundamental form on $\phi(\widehat\Sigma)$ pull back to those of $\widehat\Sigma$. Consequently maximality $\operatorname{tr}_h k=0$ is preserved, and the transported boundary is $\phi(S)$. In particular a complete stationary flow preserving $S$ preserves the boundary and maximality of every translate.

## Facts & Assumptions

[F1] Stationary Lorentzian data supply the smooth metric $g$, time-orientation field $N$, Killing condition $\mathcal L_Tg=0$, and the unique torsion-free metric-compatible Levi–Civita connection. [[def-stationary-lorentzian-data]]

[F2] The future unit normal, induced metric, second fundamental form and maximality use the stated hypersurface convention. [[def-spacelike-maximal-hypersurface-data]] An embedded smooth hypersurface with boundary is supplied with a manifold-with-boundary smooth structure for which its inclusion into the ambient manifold is a smooth embedding. [[math:def-embedded-smooth-submanifold-with-boundary]]

[F3] Diffeomorphism pushforward preserves Lie brackets of smooth vector fields. [[math:cor-diffeomorphism-pushforward-preserves-lie-brackets]]

[F4] A diffeomorphism between smooth manifolds with boundary maps their intrinsic boundaries onto one another. [[math:cor-diffeomorphisms-preserve-interior-and-boundary]]

[F5] A smooth vector field has a unique smooth maximal flow satisfying the flow composition law; completeness makes its domain all of $\mathbb R\times M$. [[math:thm-fundamental-theorem-on-flows]] [[math:prop-a-vector-field-is-complete-if-and-only-if-its-flow-is-global]]

[F6] The mean value theorem implies that a smooth real function with zero derivative on an interval is constant. [[math:cor-mean-value-theorem]]

[F7] In each Lorentzian tangent space the timelike vectors have exactly two connected components, both convex, with the orthonormal-coordinate descriptions independent of basis up to interchange. Thus a linear Lorentzian isometry permutes these components, and a continuous timelike path stays in one component. [[physics:lem-timelike-cone-has-two-convex-components]]

[F8] For a smooth map $F:P\to Q$ and a covariant two-tensor $A$ on $Q$, the pullback is defined by $(F^*A)_p(u,v)=A_{F(p)}(dF_pu,dF_pv)$. [[math:def-pullback-of-a-covariant-tensor-field]]

[F9] A smooth map between manifolds with boundary is an immersion when its differential on each full tangent space is injective, and an embedding when it is also a homeomorphism onto its image. No neatness, properness, closed-image or boundary-preservation condition is included. [[math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary]]

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish covariance of the induced data, boundary transport and the stationary-flow specialization.

1.1 Write $\phi_*U=d\phi\circ U\circ\phi^{-1}$ and define the pulled-back connection by $D_UV=\phi_*^{-1}(\nabla_{\phi_*U}\phi_*V)$. The connection rules and metric compatibility pull back through the isometry, so $D$ is a metric-compatible connection for $g$. By bracket preservation its torsion is $D_UV-D_VU-[U,V]=\phi_*^{-1}(\nabla_{\phi_*U}\phi_*V-\nabla_{\phi_*V}\phi_*U-[\phi_*U,\phi_*V])=0$. Uniqueness therefore gives $D=\nabla$. [given, F1, F3, F8]

1.2 Give $\phi(\widehat\Sigma)$ the transported smooth structure: if $x$ is a boundary or interior chart on $\widehat\Sigma$, its image chart is $x\circ\phi^{-1}$. Its inclusion into $M$ is the original embedding followed by the ambient diffeomorphism $\phi$, so it is a smooth embedding, and the restriction $\phi:\widehat\Sigma\to\phi(\widehat\Sigma)$ is a diffeomorphism of manifolds with boundary. Intrinsic boundary preservation now gives $\partial(\phi(\widehat\Sigma))=\phi(\partial\widehat\Sigma)=\phi(S)$. [given, F2, F4, F9]

1.3 For the specialization let $\Phi_t$ be the flow of the complete stationary field $T$. It is global and smooth, and $\Phi_{t+h}=\Phi_h\circ\Phi_t$ with $\Phi_t^{-1}=\Phi_{-t}$, so each $\Phi_t$ is a diffeomorphism. Differentiating $\Phi_{t+h}^*g=\Phi_t^*(\Phi_h^*g)$ at $h=0$ gives $\frac{d}{dt}\Phi_t^*g=\Phi_t^*(\mathcal L_Tg)=0$. For fixed $p,U,V$ each evaluation $(\Phi_t^*g)_p(U,V)$ is a smooth real function of $t$. The mean value theorem on the interval joining $0$ and $t$ makes it constant, hence $\Phi_t^*g=g$ for every $t$. This calculation does not require $T$ to be nonzero. [given, F1, F5, F6, F8]

2.1 Put $\Sigma^{\prime}=\phi(\widehat\Sigma)$. The differential takes each tangent space onto that of the image, and metric invariance makes the image spacelike. Since $\phi$ preserves time orientation, $d\phi(n)$ is its future unit normal $n^{\prime}$. Consequently $h^{\prime}(d\phi U,d\phi V)=h(U,V)$ and $k^{\prime}(d\phi U,d\phi V)=-g(\nabla_{d\phi U}n^{\prime},d\phi V)=-g(\nabla_U n,V)=k(U,V)$. Tracing in an $h$-orthonormal basis and its $d\phi$ image gives equal metric traces, so maximality is preserved. These identities hold up to the boundary with the supplied smooth structure. [given, F1, F2, F8, step 1.1]

3.1 Fix $p$ and define $w_s=(d\Phi_s|_p)^{-1}N_{\Phi_s(p)}\in T_pM$. Smoothness and the isometry identity make $s\mapsto w_s$ a continuous timelike path, with $w_0=N_p$. It stays in the future component of the timelike set of $T_pM$. The linear isometry $d\Phi_s|_p$ permutes the two timelike components and maps $w_s$ to the future vector $N_{\Phi_s(p)}$; it therefore maps the future component onto the future component. Thus every $\Phi_s$ preserves time orientation. Applying steps 2.1 and 1.2 to $\phi=\Phi_s$, and using the hypothesized setwise invariance $\Phi_s(S)=S$, proves the claimed boundary and maximality assertions for every translate. [given, F1, F5, F7, step 2.1, step 1.2, step 1.3] ∎
