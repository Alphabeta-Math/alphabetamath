---
title: "Proposition 2.1: Einstein–Maxwell equations and regularity"
status: draft
research_item: pthm-harrison-electrovacuum
dependency_level: 9
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF p.9, Proposition 2.1 and equation (2.7)
      statement: The article asserts the Einstein–Maxwell equations on E and in the
        extension near S, with the stated metric/field regularity and endpoint
        values.
      hypotheses: The article regular stationary vacuum construction with original
        maximal exterior section and mass normalized to one. Attribution only.
      reading_limits: Read frozen original PDF p.9 image and corresponding extracted
        text. This citation attributes the original claim and is not its
        prerequisite proof.
    - title: Alexandru F. Radu, Rigidity of stationary black holes with small ADM
        angular momentum
      url: https://arxiv.org/html/2610.09729v1#A1.SS2
      locator: Appendix A.2, (A.12)–(A.25), and paragraph immediately following
        (A.25); spacetime formulas (3.11), (3.24)
      statement: The local stationary Harrison differential calculation verifies
        Einstein–Maxwell for non-null compatible stationary vacuum/potential
        jets, constructs compatible timelike stationary two-jets approaching a
        nonzero null jet while preserving the primitive normalization constant,
        and concludes the equations wherever T is nonzero, extending to zeros by
        smoothness and density of the nonzero locus of a nontrivial Killing
        field.
      hypotheses: Smooth stationary vacuum metric of signature (-,+,+,+); F=one half
        dT-flat; sigma=f+i psi with d sigma=2 i_T(F+i star F); stationary W0
        with dW0=4((f-1)F+psi star F) and W0(T)=d0-D0;
        Wq=(1-q)^2W0-4q(1-q)T-flat; q in [0,1]; Dq>0 and Dq+Wq(T)>0. The
        pointwise nonzero-field proof uses no global exterior assumption beyond
        existence of these local data. Density extension additionally requires a
        nontrivial Killing field on a connected spacetime.
      reading_limits: Consulted actual arXiv HTML v1 Appendix A.2, (A.12)–(A.25) and
        its concluding zero-locus and exact-gauge paragraphs, together with
        spacetime formulas (3.11), (3.12), (3.13) and (3.24), and Section 1.1
        GR/SBS. Checked the listed local hypotheses against the supplied data.
        The non-null reduction, compatible-jet construction and Killing-field
        density fact are imported, not independently reconstructed or certified.
        Global Proposition 3.1 is not invoked. The positivity, polynomial lift,
        regularity and endpoint argument below is a local composition using the
        declared suppliers.
---

PDF p. 9: ` Proposition 2.1; (2.7) `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form)
- [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive)
- [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data)
- [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data)
- [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [lem-author-c92bdd91a36e-common-positive-neighborhood](item-lem-author-c92bdd91a36e-common-positive-neighborhood)
- [lem-author-c92bdd91a36e-stationary-local-jets](item-lem-author-c92bdd91a36e-stationary-local-jets)
- [lem-author-c92bdd91a36e-residual-jet-continuity](item-lem-author-c92bdd91a36e-residual-jet-continuity)
- [lem-author-c92bdd91a36e-compatible-jet-limit](item-lem-author-c92bdd91a36e-compatible-jet-limit)
- [lem-author-c92bdd91a36e-dense-residual-extension](item-lem-author-c92bdd91a36e-dense-residual-extension)
- [thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input)
- [pthm-ernst-potential-existence](item-pthm-ernst-potential-existence)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [math:cor-transverse-intersection-theorem](https://alphabetamath.cc/item/cor-transverse-intersection-theorem)
- [` Alexandru F. Radu, Rigidity of stationary black holes with small ADM angular momentum · Appendix A.2, (A.12)–(A.25), and paragraph immediately following (A.25); spacetime formulas (3.11), (3.24) `](https://arxiv.org/html/2610.09729v1#A1.SS2)


## Statement

In the article's regular stationary vacuum construction with mass one, original exterior section maximal and $T|_S\not\equiv0$, choose the single smooth stationary primitive $W_0$ supplied by the global one-form construction and set $W_q=(1-q)^2W_0-4q(1-q)T^\flat$. For every $q\in[0,1]$, the regular Harrison metric and electromagnetic form satisfy

$$\operatorname{Ric}(g_q)_{ab}=2\left((F_q)_{ac}(F_q)_b{}^c-\tfrac14(g_q)_{ab}(F_q)_{cd}(F_q)^{cd}\right),\qquad \mathrm dF_q=0,\qquad \mathrm d\star_{g_q}F_q=0.$$

These equations hold on the exterior $E$ and throughout one open neighborhood $O$ of the bifurcation sphere, including its portion outside $\overline E$. All raised indices and the star use $g_q$. The metrics are jointly smooth in spacetime and $q\in[0,1]$; the two-forms are smooth in spacetime and continuous in $q$, with $(g_1,F_1)=(g,0)$.

## Facts & Assumptions

[A1] Adopt [post-stationary-vacuum-model](item-post-stationary-vacuum-model) and the conditions of [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime), with original exterior section maximal, $T|_S\not\equiv0$, the mass-one normalization of [def-harrison-normalization](item-def-harrison-normalization), and ZFC including [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice). The geometric meanings of stationarity, maximality, smoothness and differentiated end bounds are [def-stationary-lorentzian-data](item-def-stationary-lorentzian-data), [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) and [def-stationary-asymptotic-decay-data](item-def-stationary-asymptotic-decay-data).

[F1] The definitions [def-harrison-one-form](item-def-harrison-one-form) and [def-harrison-electromagnetic-form](item-def-harrison-electromagnetic-form) give the actual spacetime formulas, complex self-duality and index conventions using [def-complex-self-dual-two-form-data](item-def-complex-self-dual-two-form-data) and [def-source-free-geometric-electrovacuum-data](item-def-source-free-geometric-electrovacuum-data).

[F2] Under [A1], [pthm-ernst-potential-existence](item-pthm-ernst-potential-existence) supplies the unique normalized smooth stationary potential $\sigma=f+i\psi\to1$ on $E$ and its smooth extension across $S$, with $f=-g(T,T)$ and $\mathrm d\sigma=2\iota_T(F+i\star_gF)$. The regular vacuum, maximal-section and $T|_S\not\equiv0$ hypotheses of [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields) are included in [A1], so it supplies a common zero $p\in S$ of $T$ and the local rotational field. With these data, [pthm-global-harrison-one-form](item-pthm-global-harrison-one-form) gives one $W_0$ smooth and stationary on $E$ and a neighborhood of $S$, with $\mathrm dW_0=4((f-1)F+\psi\star_gF)$ and constant $W_0(T)+D_0$. Evaluating this constant at the same zero $p$ identifies it as $D_0(p)$, so $W_0(T)=D_0(p)-D_0$. The identification $F=\tfrac12\mathrm dT^\flat$ and vacuum Killing identities are [thm-vacuum-killing-ernst-input](item-thm-vacuum-killing-ernst-input).

[F3] Under the regular stationary vacuum model with maximal original outer section and mass one, [pthm-harrison-denominator-positive](item-pthm-harrison-denominator-positive) gives $D_q>0$ on $E$ for every $q\in[0,1]$, for the smooth normalized Ernst data supplied in [F2]. This is the exterior-positivity input used here.

[F4] The common local positivity, stationary coordinates, residual dependence, compatible-jet limit and dense-locus extension are [lem-author-c92bdd91a36e-common-positive-neighborhood](item-lem-author-c92bdd91a36e-common-positive-neighborhood), [lem-author-c92bdd91a36e-stationary-local-jets](item-lem-author-c92bdd91a36e-stationary-local-jets), [lem-author-c92bdd91a36e-residual-jet-continuity](item-lem-author-c92bdd91a36e-residual-jet-continuity), [lem-author-c92bdd91a36e-compatible-jet-limit](item-lem-author-c92bdd91a36e-compatible-jet-limit) and [lem-author-c92bdd91a36e-dense-residual-extension](item-lem-author-c92bdd91a36e-dense-residual-extension).

[F5] For transverse embedded submanifolds, the tangent space of their intersection is the intersection of their tangent spaces. Applied to the two smooth embedded horizon branches in [A1], this gives $T_sS=T_s\mathcal H^+\cap T_s\mathcal H^-$ for each $s\in S$. [math:cor-transverse-intersection-theorem](https://alphabetamath.cc/item/cor-transverse-intersection-theorem)

[L1] The independent local differential input is Radu Appendix A.2: (A.12)–(A.18) verify the transformed equations as identities of compatible stationary vacuum/potential two-jets where $f\ne0$, in both signatures of the orbit metric. At a nonzero null point, (A.19)–(A.25) construct compatible stationary two-jets with $f_\epsilon>0$ converging through order two, keeping the normalization constant fixed. The concluding paragraph also uses that the nonzero locus of a nontrivial Killing field on a connected spacetime is dense. These are explicitly imported inputs, not locally reconstructed proofs.

## Proof

**Given:** The hypotheses in the Statement and the specified supplier interfaces.

**Goal:** Establish the stated conclusions.

1.1 The ambient model is smooth stationary vacuum on a connected spacetime. Under [A1], the Ernst-existence supplier in [F2] gives the normalized potential and its smooth horizon extension, and the local Hawking-field supplier in [F2] gives $p\in S$ with $T(p)=0$: regularity, maximality and $T|_S\not\equiv0$ are exactly its hypotheses. The global one-form construction then applies with these data and the mass-one normalization, giving the chosen smooth stationary $W_0$. Its constant $W_0(T)+D_0$ equals $D_0(p)$ because $W_0(T)(p)=W_{0,p}(0)=0$. Shrink to a common open neighborhood $U$ of $S$ on which both $\sigma$ and $W_0$ obey their identities. By [A1], $T_s$ lies in both $T_s\mathcal H^+$ and $T_s\mathcal H^-$; [F5] identifies their intersection with $T_sS$. Thus $T$ is tangent to the spacelike compact sphere. These data and the same zero $p$ satisfy the common-positive-neighborhood lemma in [F4]. It gives a single open $O\subseteq U$ containing $S$ with $D_q>0$ and $D_q+W_q(T)=d_q>0$ for every $q$. On $E$, the regular-model, maximality, mass and normalized-potential hypotheses of [F3] are exactly [A1] and [F2], so [F3] gives $D_q>0$ there as well. [A1, F2, F3, F4, F5]

2.1 Write $d_0=D_0(p)$. Expanding the denominator gives $D_q=(1-q)^2D_0+4q(1-(1-q)f)$. Since $T_p=0$, $f(p)=0$ and $d_q=(1-q)^2d_0+4q=(1+q)^2+(1-q)^2\psi(p)^2>0$. The supplied contraction and $T^\flat(T)=-f$ give $W_q(T)=(1-q)^2(d_0-D_0)+4q(1-q)f=d_q-D_q$ throughout $E\cup O$. Also $\mathrm dT^\flat=2F$ gives $\mathrm dW_q=4(1-q)(((1-q)f-(1+q))F+(1-q)\psi\star_gF)$. Thus the full one-form identities hold on this domain. Finally $\mathrm d\sigma(T)=2(F+i\star_gF)(T,T)=0$, so $\psi$ is stationary; $g,T^\flat,W_0$ and hence $W_q$ are stationary as well. These are the local identities required by [L1], with the same pole normalization. [A1, F1, F2, algebra, step 1.1]

3.1 The smooth bundle map $A_qv=v+D_q^{-1}W_q(v)T$ has inverse $A_q^{-1}v=v-d_q^{-1}W_q(v)T$. By [F1], $g_q=(D_q/4)A_q^*g$ is Lorentzian. The original time-orienting field $N$ gives the smooth $g_q$-timelike field $A_q^{-1}N$, since $g_q(A_q^{-1}N,A_q^{-1}N)=(D_q/4)g(N,N)<0$; use the original manifold orientation for its Hodge star. The metric formula has smooth spacetime coefficients, polynomial parameter inputs and positive denominator, hence is jointly smooth on $(E\cup O)\times[0,1]$. The electromagnetic formula in [F1] has smooth spacetime factors and continuous parameter factor $\sqrt{1-q^2}$, so is spacetime smooth and continuous in $q$. These statements follow directly from the formulas and do not require any additional global construction hypotheses. [A1, F1, F2, algebra, step 1.1, step 2.1]

4.1 Fix $q$ and $x\in E\cup O$ with $T_x\ne0$. The stationary-chart lemma in [F4] applies because step 2.1 established stationarity of $\psi,W_0$, and gives $T=\partial_t$ without a timelike assumption. If $f(x)\ne0$, apply the non-null local identity of [L1], with the same spacetime formulas, orientation, vacuum and Ernst identities, curl and normalization verified above. If $f(x)=0$, the compatible stationary two-jets of [L1] approach the actual two-jet with $f_\epsilon>0$ and the same $d_0$. By positivity at the limit and continuity, they lie in $D_q>0$, $D_q+W_q(T)>0$ for all sufficiently small $\epsilon$. Their transformed residuals vanish by the non-null identity of [L1]. The residual-continuity and compatible-jet-limit lemmas in [F4] therefore give vanishing residuals at the original null jet. This uses evaluations on compatible jets, without assuming local vacuum solutions realizing the perturbed jets. [A1, F1, F2, F4, L1, step 1.1, step 2.1, step 3.1]

5.1 The field $T$ is nontrivial since it is timelike near infinity. The Killing-field density assertion of [L1] applies on the connected ambient spacetime, so its nonzero locus is dense also in the open set $E\cup O$. For each fixed $q$, step 3.1 supplies the smooth Lorentzian metric, time orientation and real two-form required by the dense-extension lemma in [F4]. That lemma extends the equations in step 4.1 to every zero of $T$ in this open set. The argument applies throughout the supplied neighborhood, including the portion outside $\overline E$. [A1, F1, F4, L1, step 3.1, step 4.1]

6.1 At $q=1$, the defining formulas give $W_1=0$, $B_1=2$, $D_1=4$ and $\sqrt{1-q^2}=0$. Hence $A_1$ is the identity, $g_1=g$ and $F_1=0$. Together with steps 3.1 and 5.1 this proves all the asserted equations, regularities and endpoint values; no differentiability of $F_q$ in $q$ at one is asserted. [F1, step 3.1, step 5.1, algebra] ∎

## External input

Import [L1] from Radu Appendix A.2, (A.12)–(A.25) and the paragraph after (A.25), at the hypotheses and reading limits in the independent source reference. Its local differential identity and compatible-jet argument are used in step 4.1, and its density assertion in step 5.1; the local data, positivity and regularity are checked in steps 1.1, 2.1 and 3.1. The local composition proves positivity applicability, the polynomial lift, regularity and endpoints from the declared suppliers. The differential identity, compatible-jet approximation and Killing-field density remain imported premises.

## Source notes

Radu Section 1.1 imposes additional global GR/SBS hypotheses for Proposition 3.1. This argument uses the existing exterior-positivity supplier under its stated hypotheses and the pointwise calculation of Appendix A.2. In that calculation, nonvanishing of T permits the local stationary chart; the subsequent formulas require only the local data recorded in the independent reference. The original PDF p.9 is cited for attribution only. The statement and its original coverage are unchanged. This repairs a generated supplier application and makes no author-defect or independent-review claim.
