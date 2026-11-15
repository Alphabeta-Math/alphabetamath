---
id: lem-author-294e9b08725d-stationary-vacuum-kid-double
title: Smooth reflection of the stationary vacuum Killing initial data
kind: lemma
status: draft
origin: pipeline
domain: mathematics
proof_strategy: direct
deps:
  - lem-author-294e9b08725d-smooth-vacuum-data-double
  - lem-author-294e9b08725d-canonical-section-reflection-parities
  - physics:def-gr-killing-field
  - physics:thm-gr-constraint-equations-in-normal-frame
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  lem-author-294e9b08725d-smooth-vacuum-data-double: mathematical-premise
  lem-author-294e9b08725d-canonical-section-reflection-parities: mathematical-premise
  physics:def-gr-killing-field: mathematical-premise
  physics:thm-gr-constraint-equations-in-normal-frame: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
sources:
  references:
    - title: Robert Beig and Piotr T. Chruściel, Killing Initial Data
      url: https://arxiv.org/pdf/gr-qc/9604040v1
      locator: Section 2, printed pp. 3–4 (PDF pages 3–4), equations (2.3)–(2.13),
        especially (2.6), (2.10), (2.13).
      statement: The induced pair obeys $\mathcal L_Xh+2NK=0$ and $\mathcal
        L_XK+D^2N=N(\operatorname{Ric}_h+(\operatorname{tr}_hK)K-2K\circ K)$ in
        vacuum; $(K\circ K)_{ij}=h^{ab}K_{ia}K_{bj}$.
      hypotheses: A smooth spacelike hypersurface in a smooth Ricci-flat Lorentzian
        four-manifold; a smooth ambient Killing field $T=Nn+X$, $N=-g(T,n)$,
        $K(U,V)=g(\nabla_U n,V)$.
      reading_limits: Inspected §2, (2.3)–(2.13), including the Gaussian-coordinate
        sign convention and Einstein-tensor projections. Importing the necessary
        identities, without reconstructing their derivation or importing
        converse/global extension claims.
dependency_level: 4
---

## Statement

In the preceding data-double construction, suppose $T$ is Killing in an actual vacuum neighborhood of the positive section and commutes with the exact boost field on the canonical collar. Assume that throughout the entire positive section the supplied $h$ and $K$ are the data induced by this same ambient metric $g$, with future unit normal $n$, $h(U,V)=g(U,V)$ and $K(U,V)=g(\nabla_U n,V)=-k(U,V)$ for tangent $U,V$. Its induced lapse and shift $(N,X)$ extend to $C_-$ as minus the reflected lapse and the reflected shift. These are smooth on $\widehat C$ and satisfy the vacuum Killing-initial-data equations everywhere: $\mathcal L_Xh+2NK=0$ and $\mathcal L_XK+\nabla_h^2N-N(\operatorname{Ric}_h+(\operatorname{tr}_hK)K-2K\circ K)=0$. This is a statement about initial data, not yet a global Killing flow or an identification of the original exterior.

## Facts & Assumptions

**Given:** The data and hypotheses of the Statement.

**Goal:** Smooth reflected lapse and shift satisfying both vacuum KID equations.

[F1] The complete reflected metric and second fundamental form are smooth vacuum constraint data. [[lem-author-294e9b08725d-smooth-vacuum-data-double]]

[F2] The canonical lapse and shift jets have odd lapse and reflected-vector shift parities. [[lem-author-294e9b08725d-canonical-section-reflection-parities]]

[F3] The positive-side KID equations are the imported necessary identities recorded below; the constraint equations alone do not establish the second identity.

[F4] Here $K(U,V)=g(\nabla_U n,V)=-k(U,V)$ and $T=Nn+X$, $N=-g(T,n)$. The normal-frame supplier uses this positive-sign $K$ convention, while the hypersurface definition uses $k$; Killing means $\mathcal L_Tg=0$. [[def-spacelike-maximal-hypersurface-data]] [[physics:thm-gr-constraint-equations-in-normal-frame]] [[physics:def-gr-killing-field]]

## External input

Import the necessary identities from [Beig–Chruściel, §2, (2.6), (2.13)](https://arxiv.org/pdf/gr-qc/9604040v1) in the Ricci-flat specialization, with their $Y=X$ and $g_{ij}=h_{ij}$. Their convention $\partial_t h_{ij}=2K_{ij}$ matches F4. Their projections $\rho,\tau_{ij}$ in (2.10) vanish in vacuum. These identities require no division by $N$. Only these premises are imported; the reflection argument is local below.

## Proof

**Given:** The data and hypotheses of the Statement.

1.1 Extend $N$ with a minus sign and $X$ by reflected vector pullback. The all-jet collar parities give smoothness across $S$ by the componentwise pasting criterion proved in the data-double supplier (Proof 3.1); it applies to scalar and vector components as well as to the data tensors. [F1, F2, algebra]

1.2 Apply F3 on the positive open half with the induced data from F4: the actual ambient metric is smooth and Ricci-flat there and $T$ is Killing. Thus both displayed equations hold on that half, including at zeros of $N$. [F3, F4, given]

2.1 On the negative open half use the charts copied from the positive half. In these charts $(h,K,N,X)$ becomes $(h,-K,-N,X)$, with the same component functions and coordinate derivatives before the displayed sign changes. Thus the Levi–Civita connection and $\operatorname{Ric}_h$ have the same components, while $D^2N$ and $\mathcal L_XK$ change sign. The terms $(\operatorname{tr}_hK)K$ and $K\circ K$ do not change. Consequently the first KID expression is unchanged and the entire second expression changes by a common minus sign; both vanish by step 1.2. Smoothness of all data and of $(N,X)$ makes the KID expressions continuous across $S$, so vanishing on the dense union of the open halves proves vanishing on the seam. This establishes precisely the initial-data conclusion. [F1, step 1.1, step 1.2, algebra] ∎
