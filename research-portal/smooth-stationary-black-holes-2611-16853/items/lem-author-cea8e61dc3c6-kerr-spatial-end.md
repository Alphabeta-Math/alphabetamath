---
id: lem-author-cea8e61dc3c6-kerr-spatial-end
title: The Boyer–Lindquist spatial end and differentiated expansion
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - lem-author-cea8e61dc3c6-kerr-exterior-tensor
  - def-stationary-asymptotic-decay-data
  - def-spacelike-maximal-hypersurface-data
dependency_roles:
  lem-author-cea8e61dc3c6-kerr-exterior-tensor: mathematical-premise
  def-stationary-asymptotic-decay-data: mathematical-premise
  def-spacelike-maximal-hypersurface-data: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The Kerr Metric
      url: https://arxiv.org/pdf/1410.2130
      locator: §2, equations (2.1), (2.5)–(2.8), PDF pp. 2–3
      statement: The review gives ingoing and Boyer–Lindquist Kerr forms, their
        coordinate transformation, and the asymptotic identification of mass M
        and angular momentum J=aM.
      hypotheses: The Kerr metric in the stated coordinate systems and their indicated
        domains.
      reading_limits: Consulted section 2, equations (2.1), (2.5)–(2.8) and adjacent
        discussion on PDF pages 2–3. These supply coordinate and parameter
        background only. The differentiated end bounds and the identification of
        lapse and shift are derived locally using the declared mathematical
        suppliers; no source proof of the full indexed statement was
        reconstructed.
dependency_level: 2
---

## Statement

On a constant $t$ slice of the Kerr exterior, set $x=r(\sin\theta\cos\phi,\sin\theta\sin\phi,\cos\theta)$ and $n=x/r$. Its induced metric satisfies
$$h_{ij}=\delta_{ij}+\frac{2M}{r}n_in_j+O_2(r^{-2}).$$
The lapse is $N=1+O_2(r^{-1})$ and its shift one-form $\beta=g_{ti}dx^i$ has Cartesian components $O_2(r^{-2})$. These are fixed-parameter bounds uniform in angular directions, with no assertion of uniformity as parameters vary.

## Statement references

[[lem-author-cea8e61dc3c6-kerr-exterior-tensor]]

[[def-stationary-asymptotic-decay-data]]

[[def-spacelike-maximal-hypersurface-data]]

## Facts & Assumptions

[F1] The following exact suppliers supply the geometric objects and earlier conclusions used here: [[lem-author-cea8e61dc3c6-kerr-exterior-tensor]] [[def-stationary-asymptotic-decay-data]]

[F2] For a spacelike slice, the induced metric is $h(U,V)=g(U,V)$ on tangent vectors. For $T=\partial_t$ and its unit normal $\nu$, the lapse and tangent shift are $N=-g(T,\nu)$ and $X=T-N\nu$. The shift one-form is the tangent covector $\beta=h(X,\cdot)$. Use the time orientation with $dt(\nu)>0$ on the constant $t$ slices; their spacelikeness is verified below. These are the induced-metric and normal–tangent conventions of [[def-spacelike-maximal-hypersurface-data]].

## Proof

**Given:** The exterior metric and differentiated fixed-chart convention of [F1], and the induced-metric and lapse–shift conventions of [F2].

**Goal:** Establish the required asymptotically flat end expansions.

1.1 The slice metric is diagonal in the polar chart: $h_{rr}=\Sigma/\Delta=1+2M/r+O(r^{-2})$, $h_{\theta\theta}=r^2+a^2\cos^2\theta$, and $h_{\phi\phi}=(r^2+a^2+2Ma^2r\sin^2\theta/\Sigma)\sin^2\theta$. Relative to the smooth sphere metric and its rotation one-form, the last two correction terms are bounded smooth sphere tensors. Transforming their covariant components to Cartesian coordinates introduces $r^{-2}$, whereas $dr=n_i dx^i$. This gives the displayed Cartesian expansion. Smooth rational functions of $1/r$ and smooth angular tensors have the indicated derivative bounds; all denominators are bounded away from zero for sufficiently large $r$. Moreover, globally on the sphere the induced metric is $h=(\Sigma/\Delta)dr^2+\Sigma\gamma+a^2(1+2Mr/\Sigma)\alpha\otimes\alpha$, where $\gamma$ is the round metric and $\alpha=\sin^2\theta\,d\phi$ is its smooth rotation one-form. Since $\Delta,\Sigma,r,M>0$, this is positive definite everywhere on each exterior slice, including the axes. Thus the slices are spacelike and [F2] applies. [given, F1, F2]

2.1 Set $D=(r^2+a^2)^2-a^2\Delta\sin^2\theta=(r^2+a^2)\Sigma+2Ma^2r\sin^2\theta>0$. Inverting the exterior $t,\phi$ block gives $g^{tt}=-D/(\Sigma\Delta)<0$ away from the axes; this smooth scalar formula extends across them. For the unit normal in [F2], the covector $g(\nu,\cdot)$ vanishes on the slice tangents and takes the value $-N$ on $T$, so $g(\nu,\cdot)=-N\,dt$. Taking its inverse-metric squared norm gives $-1=N^2g^{tt}$. Also $1=dt(T)=Ndt(\nu)$, since $X$ is tangent, so the chosen orientation gives $N>0$. Consequently $N=(-g^{tt})^{-1/2}=(\Sigma\Delta/D)^{1/2}$. This is a smooth function of $1/r$ and smooth angular data near $1/r=0$, with value $1$ there and denominators bounded away from zero, hence $N=1+O_2(r^{-1})$ in the convention of [F1]. [given, F1, F2, step 1.1]

3.1 For every tangent vector $U$, orthogonality gives $\beta(U)=h(X,U)=g(T,U)$, so in the adapted coordinates $\beta_i=g_{ti}$, as claimed in the Statement. The exterior tensor therefore gives $\beta=-2Mar\sin^2\theta\,d\phi/\Sigma$. Since $\sin^2\theta\,d\phi=(-x^2dx^1+x^1dx^2)/r^2$, its Cartesian coefficients are $O_2(r^{-2})$, smoothly across the axes. The smooth rational coefficients give the differentiated bounds by the same fixed-parameter argument as in step 1.1. [given, F1, F2, step 1.1, step 2.1] ∎

## External input

The cited Kerr coordinate formulas provide background for the local calculation in this item.
