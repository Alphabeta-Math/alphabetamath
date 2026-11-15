---
title: AIK perturbative effective constant and its coordinate data
status: published
research_item: def-author-ad064c44a1cc-perturbative-effective-constant
dependency_level: 3
sources:
  references:
    - title: "S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth
        stationary black holes in vacuum: small perturbations of the Kerr
        spaces"
      url: https://arxiv.org/html/0904.0982v1
      locator: Section 1.1 setup and GR/SBS; section 2.1, (2.1)–(2.5), especially the
        three coordinate-construction paragraphs between (2.2) and (2.3).
      reading_limits: Consulted arXiv:0904.0982v1 HTML section 1.1 setup and GR/SBS
        and section 2.1 through (2.5), including the cutoff, field extension,
        flow chart, SBS collar containment and (2.3). Checked these formulas and
        domain conditions against the present definition. The source coordinate
        construction is imported, not locally reconstructed; no global rigidity
        proof, Carleman argument or library proof audit was performed.
      statement: Section 2.1 specifies the quantitative chart package (2.1)–(2.5). For
        a smooth cutoff eta taking values in [0,1], equal to 1 up to 1 and
        supported in (-infinity,2], it constructs a smooth field T-prime near
        Sigma_{3/4}, equal on that slice to eta(r/R1)n+(1-eta(r/R1))T and equal
        to T on the stationary region r>2R1. Its flow gives Phi1 on
        (-epsilon0,epsilon0) times E_{1-epsilon0}, agreeing with the slice and
        stationary charts. Epsilon0 can be chosen small so the r=1 collar lies
        in the SBS neighborhood and (2.3) holds. Equations (2.4)–(2.5) define A2
        and the effective constant from this chart.
      hypotheses: The smooth spacelike reference slice, its parametrization and future
        unit normal, stationary asymptotic chart, mass and angular parameters,
        and GR/SBS neighborhood of section 1.1; constants A1,R1 chosen with the
        slice and end bounds (2.1)–(2.2) and R1 at least A1^4. The flow is that
        of the specified smooth ambient extension of T-prime, with sufficiently
        small positive epsilon0. This coordinate construction adds neither
        maximality nor the PK smallness assumption.
---

## Prerequisites

- [def-author-ad064c44a1cc-perturbative-gr-sbs](item-def-author-ad064c44a1cc-perturbative-gr-sbs)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Uniqueness of smooth stationary black holes in vacuum: small perturbations of the Kerr spaces · Section 1.1 setup and GR/SBS; section 2.1, (2.1)–(2.5), especially the three coordinate-construction paragraphs between (2.2) and (2.3). `](https://arxiv.org/html/0904.0982v1)



## Definition

An **AIK perturbative quantitative chart package** consists of the preceding GR/SBS data with the choices and bounds of AIK §2.1. Write $\Sigma_r=\Phi_0(E_r)$ and let $n$ be the future unit normal to $\Sigma^0$. Choose $A_1,R_1\ge R_0$ with $R_1\ge A_1^4$, such that on $\Sigma_{3/4}$,
$$A_1^{-1}|v|^2\le g_{ij}v^iv^j\le A_1|v|^2,\qquad \sum_{i=1}^3|g(\partial_i,T)|+|g(n,T)|\le A_1.$$
On the end $r\ge R_1$, require the sum of weighted derivatives through order six of the three remainders to be bounded by $A_1$: their weights for $g_{ij}-\delta_{ij}$, $g_{00}+1-2M_0/r$ and $g_{0i}+2\epsilon_{ijk}S^jx^kr^{-3}$ are respectively $r^{m+1}$, $r^{m+2}$ and $r^{m+3}$ at derivative order $m$.

Choose a smooth cutoff $\eta:\mathbb R\to[0,1]$ with $\eta(u)=1$ for $u\le1$ and $\operatorname{supp}\eta\subset(-\infty,2]$. Supply the smooth ambient field $T'$ of the AIK construction on a neighborhood of $\Sigma_{3/4}$ and on the distant stationary end, with
$$T'|_{\Sigma_{3/4}}=\eta(r/R_1)n+(1-\eta(r/R_1))T,\qquad T'=T\ \text{on }\Phi_0(\mathbb R\times E_{2R_1}).$$

Here $r$ in the slice formula is the radius in $\Phi_0$; the choice of smooth extension off the slice is part of the package. Let $F_s$ be its local flow: $F_0(p)=p$ and $\frac{d}{ds}F_s(p)=T'(F_s(p))$. Choose $0<\varepsilon_0<1/4$ sufficiently small that
$$\Phi_1(s,x)=F_s(\Phi_0(x)):\ (-\varepsilon_0,\varepsilon_0)\times E_{1-\varepsilon_0}\longrightarrow\widetilde M$$
is a diffeomorphism onto an open neighborhood of $\Sigma^0\cap\overline E$, with $\Phi_1(0,x)=\Phi_0(x)$, agreement with the stationary chart for $r>2R_1$, and $\partial_0=T'$ in these coordinates. The restriction on $\varepsilon_0$ puts its initial points in $\Sigma_{3/4}$. Writing $O$ for the supplied SBS neighborhood of $S_0$, require
$$\Phi_1\big((-\varepsilon_0,\varepsilon_0)\times\{x:1-\varepsilon_0<|x|<1+\varepsilon_0\}\big)\subset O.$$

Require $\sum_i|g_{0i}|+|g_{00}+1|\le A_1/(R_1+r)$ throughout $\widetilde M$. The availability of this source-specific field and flow chart is the imported construction recorded in External input. With $|\partial^m|$ denoting the sum over all spacetime coordinate derivatives of total order $m$ and all displayed tensor indices, set
$$A_2=\sup_{\widetilde M}\sum_{m=0}^6\left(\sum_{a,b=0}^3|\partial^m g_{ab}|+\sum_{a=0}^3|\partial^mT^a|\right),\qquad \overline A_{\rm PK}=\max\{R_1,A_2,\varepsilon_0^{-1},(M_0^2-J)^{-1}\}.$$
Require $A_2<\infty$. These are the choices and bounds of AIK (2.1)–(2.5), not an unspecified coordinate-invariant norm of the metric.

## Definition references

[def-author-ad064c44a1cc-perturbative-gr-sbs](item-def-author-ad064c44a1cc-perturbative-gr-sbs)

[def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[AIK, section 2.1, (2.1)–(2.5) and the flow construction between (2.2) and (2.3)](https://arxiv.org/html/0904.0982v1)

## Facts & Assumptions

[F1] [def-author-ad064c44a1cc-perturbative-gr-sbs](item-def-author-ad064c44a1cc-perturbative-gr-sbs) provides $M_0,J$, the slice and the exterior chart. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) supplies its future unit normal and positive induced metric.

[F2] [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data) supplies differentiated component bounds and the meaning of one common finite bound; here spacetime derivatives in the interpolated chart are explicitly included.

[F3] AIK section 2.1 supplies the cutoff-field and flow-chart construction, its slice and stationary-end agreements, the SBS collar containment and the coordinate bounds. This imported input is specified in External input and the statement-bearing source reference.

## Justification

The field extension and its flow chart are supplied by the cited AIK construction, rather than inferred from the three general definitional suppliers alone. All coefficient arrays and coordinate derivatives are defined on the supplied charts. The prescribed spacelike metric makes the two-sided quadratic bound meaningful, and the normal exists on the supplied slice. Supremum over a specified set is an extended nonnegative number; the explicit finiteness condition gives a finite $A_2$. Since $M_0^2-J>0$ in the source GR package and $\varepsilon_0>0$, the displayed maximum is a finite positive number. This definition records the actual chart package on which the source threshold depends; it proves neither existence of uniformly bounded packages in a family nor independence from their choices.

## External input

[AIK, section 2.1, between (2.2) and (2.3)](https://arxiv.org/html/0904.0982v1) supplies the smooth interpolating field and its flow chart under the preceding source GR/SBS data and bounds (2.1)–(2.2). The cutoff, slice value, distant-end agreement, flow equation, chart domain and SBS collar restriction are transcribed in Definition. Equations (2.3)–(2.5) supply the subsequent chart bound and effective-constant conventions. The full imported statement, hypotheses and reading limits are in the source reference. This is an imported coordinate construction; the finite-constant justification above does not claim a local proof of its existence.
