---
title: Exact AIK global, horizon and quantitative hypotheses
status: published
research_item: def-author-0a41d659d5ab-aik-quantitative-package
dependency_level: 2
sources:
  references:
    - title: S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary
        black holes with small angular momentum on the horizon
      url: https://arxiv.org/pdf/1304.0487v2
      locator: §1.1.1–§1.1.2, (1.1)–(1.4), SBS, PDF pp. 3–4; §1.2 (1.6)–(1.10), PDF
        pp. 5–6
      statement: The source specifies the GR and SBS hypotheses, the maximal section
        and quantitative bounds (1.6)-(1.10). Bound (1.7) holds on Phi0(R times
        E_R1); the flow chart agrees with Phi0 on its initial slice and on
        (-epsilon0,epsilon0) times E_2R1. The fixed quantitative constant is
        A=max(R1,A2,epsilon0^-1,(M^2-J)^-1).
      hypotheses: Smooth stationary Ricci-flat spacetime, the specified
        section/end/horizon, and the quantitative chart bounds stated in the
        Definition. The end radius is chosen sufficiently large before fixing A.
      reading_limits: Consulted the linked PDF text at the assumption paragraphs and
        formulas on PDF pp. 3–6, including the domains of (1.7) and the
        interpolation and chart-agreement paragraph before (1.8). The coordinate
        construction is imposed as part of the package; no existence of a
        maximal surface or horizon is inferred. The null-form well-definedness
        and rescaling argument is local, not attributed to these passages. No
        rigidity proof or separate cited construction was reviewed.
    - title: E. Minguzzi, Lorentzian causality theory
      url: https://s3.cern.ch/inspire-prod-files-7/7a575d682fd15aaad8463a778fac1609
      locator: Definition 2.130, PDF p. 76; Definition 3.35, PDF p. 95
      statement: A partial Cauchy hypersurface is an acausal edgeless set; the edge
        predicate is the local timelike-bypass predicate stated in the
        Definition.
      hypotheses: An achronal subset of a time-oriented spacetime, with chronological
        relations relative to each specified neighborhood.
      reading_limits: Consulted the linked PDF text of Definitions 2.130 and 3.35 on
        PDF pp. 76 and 95 for the edge and partial-Cauchy terminology. No
        causality theorem proof was reviewed.
---

## Prerequisites

- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [` S. Alexakis, A. D. Ionescu and S. Klainerman, Rigidity of stationary black holes with small angular momentum on the horizon · §1.1.1–§1.1.2, (1.1)–(1.4), SBS, PDF pp. 3–4; §1.2 (1.6)–(1.10), PDF pp. 5–6 `](https://arxiv.org/pdf/1304.0487v2)
- [` E. Minguzzi, Lorentzian causality theory · Definition 2.130, PDF p. 76; Definition 3.35, PDF p. 95 `](https://s3.cern.ch/inspire-prod-files-7/7a575d682fd15aaad8463a778fac1609)


## Definition

The **AIK quantitative stationary package** is the following collection of data and assumptions; it is separate from a generic bifurcate Killing horizon and from other black-hole comparison packages.

Let $(M,g,N,o)$ be a connected oriented, time-oriented, paracompact smooth Lorentzian four-manifold without boundary of signature $(-,+,+,+)$, with $\operatorname{Ric}(g)=0$ and a smooth Killing field $T$. Let $E_r=\{x\in\mathbb R^3:|x|>r\}$ and let $\Phi_0:E_{1/2}\to\Sigma_0\subset M$ be a diffeomorphism onto an embedded spacelike partial Cauchy hypersurface. Here partial Cauchy means acausal and edgeless: no two distinct points are causally related, and there is no $q\in\overline{\Sigma_0}$ such that every neighborhood $U$ of $q$ contains a timelike curve, avoiding $\Sigma_0$, from a point of $I^-_U(q)$ to a point of $I^+_U(q)$. No claim that it is Cauchy for all of $M$ is imposed. Write $\Sigma_r=\Phi_0(E_r)$ and $S_0=\Phi_0(\{|x|=1\})$. Require $\Sigma_1$ to be maximal. Let $\nu$ be the future unit normal to $\Sigma_0$, $h=g|_{T\Sigma_0}$, $n=-g(T,\nu)$, and $X=T-n\nu$.

**GR.** For sufficiently large $R_0$, the map on $E_{R_0}$ extends to a diffeomorphism $\Phi_0:\mathbb R\times E_{R_0}\to M^{\rm end}$ onto an open end, with $T=\partial_0$. Put $r=|x|$. There are $M_0>0$ and $S^1,S^2,S^3\in\mathbb R$, with $J=((S^1)^2+(S^2)^2+(S^3)^2)^{1/2}<M_0^2$, such that $g_{00}=-1+2M_0/r+O_6(r^{-2})$, $g_{ij}=\delta_{ij}+O_6(r^{-1})$, and $g_{0i}=-2\epsilon_{ijk}S^jx^k/r^3+O_6(r^{-3})$. The alternating symbol has $\epsilon_{123}=1$. Differentiated bounds count all coordinate derivatives through total order six, including $x^0$ derivatives (which vanish on this stationary end). Set $E=I^-_M(M^{\rm end})\cap I^+_M(M^{\rm end})$. Require $E$ to be globally hyperbolic, $\Sigma_0\cap I^-_M(M^{\rm end})=\Sigma_0\cap I^+_M(M^{\rm end})=\Sigma_1$, $T\ne0$ on $E$, and every $T$-orbit in $E$ to be complete and intersect $\Sigma_1$ transversely.

**SBS.** In a neighborhood $O$ of $S_0$, require $H^+=O\cap\partial_M I^-_M(M^{\rm end})$ and $H^-=O\cap\partial_M I^+_M(M^{\rm end})$ to be smooth embedded null non-expanding hypersurfaces intersecting transversely in $S_0$. Here is the precise non-expansion convention, which applies to either null hypersurface $H=H^\pm$. Let $L_p=T_pH\cap(T_pH)^{\perp_g}$ be its null normal line and $Q_p=T_pH/L_p$ the two-dimensional quotient. Its positive-definite metric is $q_p([U],[V])=g_p(U,V)$, with $[U]$ denoting the class modulo $L_p$. For a smooth nowhere-zero local section $\ell$ of $L$, the **null second fundamental form** is the symmetric form on $Q$ given by $B_\ell([U],[V])=g(\nabla_U\ell,V)$, where $U,V$ are tangent to $H$ and $\nabla$ is the ambient Levi–Civita connection. Tangential covariant differentiation may use any smooth ambient extension of $\ell$. Its **expansion** is $\theta_\ell=\operatorname{tr}_q B_\ell=q^{AB}(B_\ell)_{AB}$, where $A,B=1,2$ label any local frame of $Q$ and $(q^{AB})$ is the inverse quotient metric. The hypersurface is **non-expanding** when $\theta_\ell=0$ on every such local domain. The local justification below proves well-definedness and $\theta_{f\ell}=f\theta_\ell$ for every smooth nowhere-zero real function $f$, so this vanishing condition needs no normal scale or affine parametrization. Require $T$ to be tangent to both and not identically zero on $S_0$. These conditions do not identify $T$ with a horizon-generating Killing field vanishing on $S_0$.

**Quantitative choices.** Fix large $A_1\ge2$ and $R_1\ge\max(R_0,A_1^4,8M_0,2\sqrt{A_1},2)$. On $\Sigma_{3/4}$ require $A_1^{-1}|v|^2\le h_{ij}v^iv^j\le A_1|v|^2$ and $\sum_{i=1}^3|g(\partial_i,T)|+|g(\nu,T)|\le A_1$. On the restricted end $\Phi_0(\mathbb R\times E_{R_1})$ require
$$\sum_{m=0}^6r^{m+1}\sum_{j,k=1}^3|\partial^m(g_{jk}-\delta_{jk})|+\sum_{m=0}^6r^{m+2}|\partial^m(g_{00}+1-2M_0/r)|+\sum_{m=0}^6r^{m+3}\sum_{i=1}^3|\partial^m(g_{0i}+2\epsilon_{ijk}S^jx^kr^{-3})|\le A_1.$$

Here $|\partial^m u|$ is the sum over all four-coordinate derivatives of total order $m$; the displayed decay bound is imposed on $\Phi_0(\mathbb R\times E_{R_1})$, rather than on all of the original $R_0$ end.

As in source §1.2, specify a smooth cutoff $\chi:\mathbb R\to[0,1]$ supported in $(-\infty,2]$ and equal to one on $(-\infty,1]$. Specify a smooth ambient vector field $T'$ in a neighborhood of $\Sigma_{3/4}$ and on $\Phi_0(\mathbb R\times E_{2R_1})$, with $T'=\chi(r/R_1)\nu+(1-\chi(r/R_1))T$ on $\Sigma_{3/4}$ and $T'=T$ on $\Phi_0(\mathbb R\times E_{2R_1})$. For $0<\eta_0<1/4$ sufficiently small, require the local flow of $T'$ to give the diffeomorphism $\Phi_1:(-\eta_0,\eta_0)\times E_{1-\eta_0}\to\widetilde M$, with $\Phi_1(t,x)=\operatorname{Fl}^{T'}_t(\Phi_0(x))$ and $\partial_0=T'$ in these coordinates. Require $\Phi_1(0,x)=\Phi_0(x)$ for $x\in E_{1-\eta_0}$ and $\Phi_1(t,x)=\Phi_0(t,x)$ for $(t,x)\in(-\eta_0,\eta_0)\times E_{2R_1}$. No stationary-coordinate agreement is required for $R_0<r\le2R_1$ away from the slice. Require $\sum_{j=1}^3|g_{0j}|+|g_{00}+1|\le A_1/(R_1+r)$ throughout $\widetilde M$ in the $\Phi_1$ coordinates, and put
$$A_2=\sup_{\widetilde M}\sum_{m=0}^6\left(\sum_{\alpha,\beta=0}^3|\partial^mg_{\alpha\beta}|+\sum_{\alpha=0}^3|\partial^mT^\alpha|\right),\qquad A=\max(R_1,A_2,\eta_0^{-1},(M_0^2-J)^{-1})<\infty.$$

The source uses $\epsilon_0$ for $\eta_0$ and $\epsilon$ for the independent horizon-smallness parameter. The extra lower bounds $R_1\ge8M_0,2\sqrt{A_1},2$ are a choice of a sufficiently large end radius, permitted before fixing $A$; they impose no smallness assumption on a spacetime. One can enlarge the end radius and redo the source's cutoff construction before fixing the quantitative constants.

## Facts & Assumptions

[A1] Work in ZFC, including the axiom of choice and its inherited countable and dependent choice uses. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[F1] The Lorentzian, stationary-field, curvature and index conventions, including the inverse metric and the torsion-free metric-compatible Levi–Civita connection, are those of [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data).

[F2] The horizon vocabulary distinguishes the stationary field from a Killing generator and defines nullness, the radical null normal line and bifurcation transversality. The quotient metric, null second fundamental form and expansion are defined locally in the present Definition and justified below. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F3] Spacelike sections, the future unit normal, maximality, lapse and shift use [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data).

[F4] Fixed-chart differentiated decay uses [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data); the present Definition explicitly extends its derivative counting to the four source coordinates.

[F5] Exterior chronological sets, completeness, transversality and global hyperbolicity have the domain-relative meanings of [def-causal-exterior-and-boundary-data](item-def-causal-exterior-and-boundary-data).

[F6] The independent source assumption contract is recorded in External input.

[F7] The local-flow notation for $T'$ uses [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow) on the open neighborhood where $T'$ is smooth. Its domain and integral-curve laws require neither a Killing field nor completeness; the uniform time interval, chart diffeomorphism and agreement properties remain imposed hypotheses.

## Justification

**Given:** The data and hypotheses in the Definition, with the set-theoretic convention [A1].

**Goal:** Verify that the package is a definite collection of hypotheses, without asserting its existence.

1.1 The specified charts and section determine $r$, all component derivatives, the end, the exterior, and the sphere. The geometric interfaces make the smoothness, causal, spacelike-normal and maximality conditions predicates on these data. The flow notation is interpreted on the open neighborhood where $T'$ is specified, in the sense of [F7]. The flow chart uses $E_{1-\eta_0}\subset E_{3/4}$, and its agreement sets are the slice and $(-\eta_0,\eta_0)\times E_{2R_1}$; on the latter the interpolating field equals $T$. The decay sum uses only the restricted $R_1$ end. These charts, interpolation and inequalities are supplied hypotheses, not conclusions of generic stationarity. The SBS tangencies concern $T$, whereas a Killing generator in [F2] is separately specified; the two are not equated. [given, F1, F2, F3, F4, F5, F6, F7]

1.2 For a local defining function $u$ of the embedded null hypersurface $H$, $du\ne0$ and $H=\{u=0\}$ locally. Nondegeneracy gives a smooth nonzero normal $g^{-1}(du)$ spanning $(TH)^{\perp_g}$, which is one-dimensional and contained in $TH$ by nullness. Thus $L$ is a smooth line bundle with local nonzero sections. At any point, normalize the supplied timelike orientation vector to $e_0$, with $g(e_0,e_0)=-1$. A nonzero null vector can be written $\ell=a(e_0+e_1)$, with $a\ne0$ and $e_1\in e_0^\perp$ of length one. The space $e_0^\perp$ is positive definite by signature $(-,+,+,+)$. Every $U\in TH=\ell^\perp$ then has the unique form $U=b(e_0+e_1)+v$ with $v\in e_0^\perp\cap e_1^\perp$. For $V=c(e_0+e_1)+w$, $g(U,V)=g(v,w)$. This proves that $q$ is well-defined and positive definite on the two-dimensional quotient $Q$; smoothness follows in local quotient frames from smoothness of $g$ and $L$. [given, F1, F2, algebra]

2.1 For tangent fields $U,V$, metric compatibility gives $g(\nabla_U\ell,V)=-g(\ell,\nabla_UV)$. Torsion freedom and tangency of $[U,V]$ give $B_\ell(U,V)-B_\ell(V,U)=-g(\ell,[U,V])=0$. Also $g(\nabla_U\ell,\ell)=\tfrac12U(g(\ell,\ell))=0$, so symmetry makes both slots vanish on $L$. The expression is bilinear over smooth functions in $U,V$, descends to $Q$, and is independent of representatives. Any two ambient extensions of $\ell$ differ by a field vanishing along $H$, whose covariant derivative in a tangent direction vanishes there; hence the formula is extension-independent and defines a smooth symmetric form. [step 1.2, F1, F2, algebra]

3.1 The positive-definite quotient metric has an inverse, so the contraction defining $\theta_\ell$ is independent of the quotient frame. For any smooth nowhere-zero $f$, the connection product rule gives $g(\nabla_U(f\ell),V)=f g(\nabla_U\ell,V)+(Uf)g(\ell,V)=f B_\ell([U],[V])$. Consequently $B_{f\ell}=fB_\ell$ and $\theta_{f\ell}=f\theta_\ell$. Every pair of local nonzero sections of $L$ differs by such an $f$ on their overlap. Thus vanishing of the expansion is independent of all local choices and defines the non-expansion predicate used in SBS. [step 1.2, step 2.1, F1, F2, algebra]

4.1 The finite derivative sums and the displayed supremum define $A_2$ as an extended nonnegative number; the explicit finiteness requirement makes $A$ finite. The strict condition $J<M_0^2$ makes its last term positive and finite. Fixing these charts and bounds before choosing a small horizon parameter makes dependence on $A$ unambiguous. Choosing the end radius sufficiently large, and the flow interval sufficiently small, is the source §1.2 convention and does not infer existence of any unassumed geometric object. Together with the local null-form calculation, this makes the entire package a definite collection of hypotheses. [step 1.1, step 3.1, F4, F6, algebra] ∎

## External input

AIK §§1.1–1.2 supplies the GR, SBS, maximal-section and quantitative-coordinate assumption contract (1.1)–(1.4), (1.6)–(1.10), including the restricted end for (1.7) and the slice/far-end agreement for the flow chart. These are imposed assumptions, not conclusions of generic stationarity, an I-plus-regularity equivalence or a local reconstruction of a rigidity theorem. The null quotient metric, second fundamental form and scale-invariant zero-expansion predicate are supplied by the local Definition and Justification, rather than imported as an unstated source theorem. Minguzzi Definitions 2.130 and 3.35 supply the edge and partial-Cauchy conventions.
