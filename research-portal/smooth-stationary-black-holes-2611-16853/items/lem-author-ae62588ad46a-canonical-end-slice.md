---
id: lem-author-ae62588ad46a-canonical-end-slice
title: Canonical stationary end expansions give the precise source slice decay
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - def-stationary-asymptotic-decay-data
  - def-spacelike-maximal-hypersurface-data
  - math:def-levi-civita-connection
  - math:thm-fundamental-theorem-of-riemannian-geometry
  - math:prop-christoffel-formula-for-the-levi-civita-connection
  - math:def-dual-connection
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  math:def-levi-civita-connection: mathematical-premise
  math:thm-fundamental-theorem-of-riemannian-geometry: mathematical-premise
  math:prop-christoffel-formula-for-the-levi-civita-connection: mathematical-premise
  math:def-dual-connection: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: Yishen Huang, Junbin Li, and Xi-Ping Zhu, Nonexistence of Multiple Black
        Holes in Stationary Analytic Vacuum Spacetimes
      url: https://arxiv.org/pdf/2611.03766
      locator: arXiv:2611.03766v1, Section 1, hypothesis (H1), printed p. 2 (PDF page
        2), including the little-o convention immediately following its
        displayed formulas.
      statement: H1 specifies $h_{ij}=(1+2M/r)\delta_{ij}+o_2(r^{-1})$ and
        $k_{ij}=o_2(r^{-1})$; $u=o_l(r^{-p})$ requires each derivative of order
        $a\le l$ to be $o(r^{-p-a})$.
      hypotheses: These are prescribed data on a spacelike exterior slice
        diffeomorphic to $\mathbb R^3\setminus B(R)$, in Cartesian coordinates
        with $r=|x|$; H1 also identifies $M$ as ADM mass. Only its two
        differentiated decay clauses and notation are compared here.
      reading_limits: Read the extracted PDF text of Section 1 through H1 on PDF page
        2. This checks the formulation and notation only; no proof of the paper,
        existence of a canonical stationary gauge, exterior topology, or ADM
        identification is imported or reconstructed.
dependency_level: 1
---

## Statement

Suppose a smooth stationary vacuum end, meaning $\operatorname{Ric}(g)=0$ on the end, has adapted coordinates $T=\partial_t$ and, for a constant $m$, $g_{00}=-1+2m/r+o_3(r^{-1})$, $g_{ij}=(1+2m/r)\delta_{ij}+o_3(r^{-1})$, and $g_{0i}=o_3(r^{-1})$. Then a sufficiently far-out $t=0$ slice is spacelike and has $h_{ij}=(1+2m/r)\delta_{ij}+o_2(r^{-1})$ and second fundamental form $k_{ij}=o_2(r^{-1})$. These are exactly the two differentiated decay requirements in (H1) of Huang–Li–Zhu; this comparison does not assert its exterior-slice topology or identify $m$ as ADM mass. Here $o_j(r^{-b})$ means that derivatives of order $\ell\le j$ are $o(r^{-b-\ell})$.

## Facts & Assumptions

[F1] The metric, Killing field, Ricci tensor and covariant-derivative conventions are [[def-stationary-lorentzian-data]]. The differentiated end convention is [[def-stationary-asymptotic-decay-data]]; the normal and second fundamental form are [[def-spacelike-maximal-hypersurface-data]]. Vacuum is the mathematical restriction $\operatorname{Ric}(g)=0$, which this calculation does not use. The displayed expansions are hypotheses here; no existence of coordinates with these expansions is deduced.

[F2] The source H1 specifies the two differentiated slice-decay forms and the little-o convention recorded in External input below (Huang–Li–Zhu, Section 1, H1, p. 2). Its additional topology and ADM-mass clauses are outside this comparison.

[F3] For the smooth Riemannian metric $h$, a Levi–Civita connection is torsion-free and metric-compatible, and exists uniquely. [[math:def-levi-civita-connection]] [[math:thm-fundamental-theorem-of-riemannian-geometry]] Its coordinate symbols obey the Christoffel formula. [[math:prop-christoffel-formula-for-the-levi-civita-connection]] Its action on covectors is the dual connection, characterized by $(D_U\alpha)(V)=U(\alpha(V))-\alpha(D_UV)$. [[math:def-dual-connection]]

## Proof

**Given:** The adapted stationary end and its displayed differentiated expansions.

**Goal:** Obtain the exact asymptotic forms of its induced metric and second fundamental form.

1.1 The matrix $g_{ij}$ tends to the identity, hence is positive definite for large $r$. It is the induced metric $h$. Its inverse is bounded with the corresponding differentiated decay. In the decomposition $T=Nn+\beta$, the shift covector is $\beta_i=g_{0i}$, the vector is $\beta^i=h^{ij}\beta_j$, and $N^2=-g_{00}+h^{ij}g_{0i}g_{0j}$. Thus $N\to1$, $\beta=o_3(r^{-1})$ and $h=(1+2m/r)\delta+o_3(r^{-1})$. [given, F1, algebra]

2.1 Let $D$ be the unique Levi–Civita connection of the induced Riemannian metric $h$, so $Dh=0$ and $D$ is torsion-free. Its symbols are $\Gamma^a{}_{ij}=\tfrac12 h^{ab}(\partial_i h_{jb}+\partial_j h_{ib}-\partial_b h_{ij})$, and its dual action on the shift covector is $D_i\beta_j=\partial_i\beta_j-\Gamma^a{}_{ij}\beta_a$. Stationarity gives $\partial_t h=0$. Differentiating the induced metric along $T=Nn+\beta$ yields $2Nk=\pm\mathcal L_\beta h$, with the sign determined by the second-form convention and irrelevant for the estimate. Explicitly its components are, up to that sign, $N^{-1}(D_i\beta_j+D_j\beta_i)/2$. The first derivatives of $\beta$ and their derivatives through order two are $o(r^{-2})$ with the corresponding extra inverse powers. The $h$-Christoffel symbols are $O_2(r^{-2})$ by their coordinate formula, so their products with $\beta$ decay faster. Hence $k=o_2(r^{-2})$, which implies the weaker required $o_2(r^{-1})$, and the claim for $h$ follows from step 1.1. [given, F1, F3, step 1.1, algebra]

3.1 The estimates for $h$ and $k$ in steps 1.1 and 2.1 have precisely the two differentiated decay forms in [F2], with the source coefficient $M$ replaced by $m$. The derivative convention in the Statement is the same as that of H1. This establishes the asserted comparison of decay requirements alone; neither an exterior-slice topology nor an ADM-mass identification follows from this calculation. [F2, step 1.1, step 2.1] ∎

## External input

Huang–Li–Zhu, Section 1, H1, printed p. 2 (PDF page 2), prescribes $h_{ij}=(1+2M/r)\delta_{ij}+o_2(r^{-1})$ and $k_{ij}=o_2(r^{-1})$, with derivatives of order $a\le l$ in $o_l(r^{-p})$ required to be $o(r^{-p-a})$. Only this formulation is imported for [F2]; the slice estimates are proved locally above. The full H1 additionally prescribes exterior topology and identifies $M$ with ADM mass. [Source PDF, H1](https://arxiv.org/pdf/2611.03766).
