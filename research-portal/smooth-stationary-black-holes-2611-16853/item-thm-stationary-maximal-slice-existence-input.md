---
title: Stationary maximal hypersurface existence with a horizon boundary
status: draft
research_item: thm-stationary-maximal-slice-existence-input
dependency_level: 3
sources:
  references:
    - title: Piotr T. Chruściel and Robert M. Wald, Maximal Hypersurfaces in
        Asymptotically Stationary Spacetimes
      url: https://arxiv.org/pdf/gr-qc/9304009
      locator: Definitions 2.1 (2.1)–(2.5), pp.8–9; 2.3, p.11; (2.13)–(2.17),
        pp.11–12; Definition 2.4, p.13; (4.1)–(4.3) and Theorem 4.2, pp.24–25;
        Remark 3, p.25
      statement: "There is a family $\\widehat\\Sigma_s$ of smooth spacelike maximal
        asymptotically flat hypersurfaces, $s\\in\\mathbb R$, with
        $\\partial\\widehat\\Sigma_s=S$, $\\widehat\\Sigma_s$ diffeomorphic to
        $\\Sigma$, $\\phi_t(\\widehat\\Sigma_s)=\\widehat\\Sigma_{s+t}$ and
        interiors covering $U$ and Cauchy there in the source convention. If $X$
        is timelike on $U$, or if $\\operatorname{Ric}(Z,Z)\\geq0$ for every
        timelike $Z$, their interiors foliate $U$. The source's asymptotic
        flatness means end graphs obeying Definition 2.4:
        $|u|+\\sum_{j=1}^{k+1}r^j|\\partial^ju|\\leq Cw_\\alpha(r)$, with
        $w_\\alpha$ as in the graph-translation lemma, together with the
        corresponding weighted Hölder condition on the highest derivatives. In
        particular at $\\alpha=1$ logarithmic height growth is allowed."
      hypotheses: Let $(M,g)$ be a smooth connected time-oriented strongly causal
        spacetime and $\Sigma$ a connected closed acausal hypersurface with
        boundary $S$. Closed means closed as a subset of $M$; acausal means that
        no causal curve connects distinct points of $\Sigma$. Suppose $\Sigma$
        is the union of finitely many exterior ends $\Sigma_i$ and a compact
        interior $\Sigma_{\rm int}$ with boundary, glued along their boundary
        components. Each $\Sigma_i$ is diffeomorphic to $\mathbb
        R^3\setminus\overline B(R_i)$. For some $k\geq2$, $0<\alpha\leq1$,
        $0<\lambda\leq1$ and end-dependent $C$, each has a neighborhood chart
        with $r=|x|$, $g_{00}<-C^{-1}$, $|g_{\mu\nu}-\eta_{\mu\nu}|\leq
        Cr^{-\alpha}$, $g_{ij}v^iv^j\geq C^{-1}|v|^2$ and $|\partial^j
        g_{\mu\nu}|\leq Cr^{-\alpha-j}$ for $1\leq j\leq k$. Order-$k$
        derivatives have difference bound
        $Cr^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$ for
        $|t-\tau|\leq1$ and $|x-y|\leq r(x)/2$. The sphere bounding each end is
        identified diffeomorphically with a connected boundary component of its
        complementary portion. A Killing field $X$ is complete on $M$, uniformly
        timelike on each end, tangent to $S$, and in each chart is
        $(A_i+O(r^{-\alpha}))\partial_t+O(r^{-\alpha})\partial_{x^i}$ with
        $A_i\ne0$. These are Definitions 2.1 and 2.3, called class (b); the
        definition does not require $X=0$ on $S$ or a bifurcate Killing horizon.
        Set $M_i=\bigcup_{t\in\mathbb R}\phi_t(\Sigma_i)$, $M_{\rm
        ext}=\bigcup_iM_i$, $B=M\setminus I_M^-(M_{\rm ext})$, $W=M\setminus
        I_M^+(M_{\rm ext})$. Let $D(\Sigma)$ use the source's
        inextendible-timelike-curve convention and put
        $U=\operatorname{int}D(\Sigma)$. Require $(B\cup W)\cap U=\varnothing$.
      reading_limits: "Consulted the PDF text of gr-qc/9304009: section 2 introductory
        conventions and Definitions 2.1, 2.3 and 2.4 (printed pp.8–13),
        equations (2.1)–(2.5) and (2.13)–(2.17), and section 4 equations
        (4.1)–(4.3), Theorem 4.2 and Remark 3 (printed pp.24–25). Checked the
        stated hypotheses, domain-of-dependence convention, boundary and
        covariance conclusions, conditional foliation and allowed logarithmic
        graph growth. The nonlinear elliptic existence proof and its cited
        sources were not independently reconstructed or reviewed; PDF
        screenshots were unavailable."
external_input: true
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [lem-author-9e5789a3d617-end-holder-interface](item-lem-author-9e5789a3d617-end-holder-interface)
- [lem-author-9e5789a3d617-compact-boundary-flow](item-lem-author-9e5789a3d617-compact-boundary-flow)
- [lem-author-9e5789a3d617-exterior-exclusion-interface](item-lem-author-9e5789a3d617-exterior-exclusion-interface)
- [lem-author-9e5789a3d617-maximal-isometry-covariance](item-lem-author-9e5789a3d617-maximal-isometry-covariance)
- [lem-author-9e5789a3d617-graph-decay-translation](item-lem-author-9e5789a3d617-graph-decay-translation)
- [` Piotr T. Chruściel and Robert M. Wald, Maximal Hypersurfaces in Asymptotically Stationary Spacetimes · Definitions 2.1 (2.1)–(2.5), pp.8–9; 2.3, p.11; (2.13)–(2.17), pp.11–12; Definition 2.4, p.13; (4.1)–(4.3) and Theorem 4.2, pp.24–25; Remark 3, p.25 `](https://arxiv.org/pdf/gr-qc/9304009)


## Statement

Under the exact class-(b) hypotheses and exclusion condition [F1], There is a family $\widehat\Sigma_s$ of smooth spacelike maximal asymptotically flat hypersurfaces, $s\in\mathbb R$, with $\partial\widehat\Sigma_s=S$, $\widehat\Sigma_s$ diffeomorphic to $\Sigma$, $\phi_t(\widehat\Sigma_s)=\widehat\Sigma_{s+t}$ and interiors covering $U$ and Cauchy there in the source convention. If $X$ is timelike on $U$, or if $\operatorname{Ric}(Z,Z)\geq0$ for every timelike $Z$, their interiors foliate $U$. The source's asymptotic flatness means end graphs obeying Definition 2.4: $|u|+\sum_{j=1}^{k+1}r^j|\partial^ju|\leq Cw_\alpha(r)$, with $w_\alpha$ as in the graph-translation lemma, together with the corresponding weighted Hölder condition on the highest derivatives. In particular at $\alpha=1$ logarithmic height growth is allowed.

## Facts & Assumptions

[F1] The complete class-(b) hypotheses and exclusion condition are as follows. Let $(M,g)$ be a smooth connected time-oriented strongly causal spacetime and $\Sigma$ a connected closed acausal hypersurface with boundary $S$. Closed means closed as a subset of $M$; acausal means that no causal curve connects distinct points of $\Sigma$. Suppose $\Sigma$ is the union of finitely many exterior ends $\Sigma_i$ and a compact interior $\Sigma_{\rm int}$ with boundary, glued along their boundary components. Each $\Sigma_i$ is diffeomorphic to $\mathbb R^3\setminus\overline B(R_i)$. For some $k\geq2$, $0<\alpha\leq1$, $0<\lambda\leq1$ and end-dependent $C$, each has a neighborhood chart with $r=|x|$, $g_{00}<-C^{-1}$, $|g_{\mu\nu}-\eta_{\mu\nu}|\leq Cr^{-\alpha}$, $g_{ij}v^iv^j\geq C^{-1}|v|^2$ and $|\partial^j g_{\mu\nu}|\leq Cr^{-\alpha-j}$ for $1\leq j\leq k$. Order-$k$ derivatives have difference bound $Cr^{-\alpha-k-\lambda}(|t-\tau|^\lambda+|x-y|^\lambda)$ for $|t-\tau|\leq1$ and $|x-y|\leq r(x)/2$. The sphere bounding each end is identified diffeomorphically with a connected boundary component of its complementary portion. A Killing field $X$ is complete on $M$, uniformly timelike on each end, tangent to $S$, and in each chart is $(A_i+O(r^{-\alpha}))\partial_t+O(r^{-\alpha})\partial_{x^i}$ with $A_i\ne0$. These are Definitions 2.1 and 2.3, called class (b); the definition does not require $X=0$ on $S$ or a bifurcate Killing horizon. Set $M_i=\bigcup_{t\in\mathbb R}\phi_t(\Sigma_i)$, $M_{\rm ext}=\bigcup_iM_i$, $B=M\setminus I_M^-(M_{\rm ext})$, $W=M\setminus I_M^+(M_{\rm ext})$. Let $D(\Sigma)$ use the source's inextendible-timelike-curve convention and put $U=\operatorname{int}D(\Sigma)$. Require $(B\cup W)\cap U=\varnothing$.

[F2] The declared definitions supply stationary Lorentzian geometry, ambient chronological relations, spacelike maximality and differentiated end bounds. [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data) [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[F3] The five intermediate lemmas explain the quantitative end interface, invariant compact boundary, precise exclusion test, isometry covariance and graph decay limitations. [lem-author-9e5789a3d617-end-holder-interface](item-lem-author-9e5789a3d617-end-holder-interface) [lem-author-9e5789a3d617-compact-boundary-flow](item-lem-author-9e5789a3d617-compact-boundary-flow) [lem-author-9e5789a3d617-exterior-exclusion-interface](item-lem-author-9e5789a3d617-exterior-exclusion-interface) [lem-author-9e5789a3d617-maximal-isometry-covariance](item-lem-author-9e5789a3d617-maximal-isometry-covariance) [lem-author-9e5789a3d617-graph-decay-translation](item-lem-author-9e5789a3d617-graph-decay-translation)

## External input

Import Chruściel–Wald Theorem 4.2 under exactly [F1], with asymptotic flatness in their Definition 2.4 and source domain-of-dependence/Cauchy convention. This is an existence and covariance input; its nonlinear elliptic existence argument is not reconstructed here. The five authored local lemmas establish the indicated interfaces and consequences but are not represented as a proof of the existence theorem. For an application with the explicit additional mathematical hypothesis $\operatorname{Ric}(g)=0$, one has $\operatorname{Ric}(Z,Z)=0\geq0$ for every timelike $Z$. Thus the timelike-convergence alternative applies once the class-(b) and exclusion hypotheses have been established.

## Source notes

Neither the imported existence theorem nor the local graph estimate supplies stronger differentiated decay, a zero-height end gauge, or an identification of $U$ with a separately specified exterior. Consumers must establish these additional application obligations. Strong causality here is an ambient hypothesis, not merely a property of a smaller exterior. No source bifurcation-surface hypothesis has been inserted into class (b). The source defines $D$ using inextendible timelike curves (p.8); this item retains that convention rather than silently substituting the local causal-curve formulation.
