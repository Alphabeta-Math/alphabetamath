---
id: lem-author-c92bdd91a36e-stationary-local-jets
title: Stationary flow-box data for a nonzero Killing field
kind: lemma
status: published
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - math:def-smooth-differential-k-form
  - math:def-lie-derivative-of-a-function
  - math:def-lie-derivative-of-a-tensor-field
  - math:thm-flow-box-theorem
  - math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor
  - math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields
  - math:def-ck-and-multi-index-notation-in-several-variables
  - math:thm-clairaut-schwarz-mixed-partials
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  math:def-smooth-differential-k-form: mathematical-premise
  math:def-lie-derivative-of-a-function: mathematical-premise
  math:def-lie-derivative-of-a-tensor-field: mathematical-premise
  math:thm-flow-box-theorem: mathematical-premise
  math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor: mathematical-premise
  math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields: mathematical-premise
  math:def-ck-and-multi-index-notation-in-several-variables: mathematical-premise
  math:thm-clairaut-schwarz-mixed-partials: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
sources:
  references: []
dependency_level: 1
---

## Statement

Let $(M,g,T)$ be stationary Lorentzian data, so $M$ is a smooth four-manifold and $T$ is a smooth Killing field with $\mathcal L_Tg=0$. On an open neighborhood $U$ of $x$, let $\psi\in C^\infty(U,\mathbb R)$ be a smooth scalar function and $W_0\in\Omega^1(U)$ a smooth real covariant one-form. Assume both are stationary along $T$, meaning $\mathcal L_T\psi=0$ and $\mathcal L_TW_0=0$ on $U$.

If $T_x\ne0$, there are local coordinates $(t,x^1,x^2,x^3)$ near $x$, contained in $U$, with $T=\partial_t$. All coordinate components of $g,\psi,W_0$ are then independent of $t$, whether $T_x$ is timelike, spacelike or null.

Their stationary two-jets at $x$ mean their values and coordinate derivatives through total order two in this chart, with every derivative involving $\partial_t$ equal to zero. In particular, for each component function $h$ of $g,\psi,W_0$, these data are $h(x)$, $\partial_a h(x)$ and $\partial_a\partial_b h(x)$ for $a,b\in\{0,1,2,3\}$, where $x^0=t$; the second derivatives are symmetric in $a,b$. This is a chartwise description of the two-jets, not an assertion that component lists are invariant under changes of chart.

## Facts & Assumptions

[F1] The smooth four-manifold, metric, Killing field and local-flow definition of $\mathcal L_Tg$ are those of [[def-stationary-lorentzian-data]]. No timelike or complete-flow hypothesis is part of stationarity here.

[F2] A smooth $k$-form is a smooth section of $\bigwedge^kT^*U$, with $\Omega^0(U)=C^\infty(U)$, by [[math:def-smooth-differential-k-form]]. Thus $\psi$ is a scalar and $W_0$ is a covariant one-form, locally $W_0=(W_0)_a\,\mathrm dx^a$. Their Lie derivatives use [[math:def-lie-derivative-of-a-function]] and [[math:def-lie-derivative-of-a-tensor-field]], respectively. The vanishing of both Lie derivatives is an explicit hypothesis, not a consequence of the Killing condition for $g$.

[F3] At a nonzero point of a smooth vector field, [[math:thm-flow-box-theorem]] supplies coordinates straightening it to a coordinate vector field; the chart can be restricted to a product neighborhood contained in $U$.

[F4] For any smooth covariant $k$-tensor $A$ and smooth vector field $X$, [[math:prop-coordinate-formula-for-the-lie-derivative-of-a-covariant-tensor]] gives $(\mathcal L_XA)_{i_1\cdots i_k}=X^j\partial_jA_{i_1\cdots i_k}+\sum_{a=1}^k(\partial_{i_a}X^j)A_{i_1\cdots j\cdots i_k}$. For a smooth scalar $h$, [[math:prop-lie-derivative-agrees-with-x-on-functions-and-bracket-on-vector-fields]] gives $\mathcal L_Xh=Xh$.

[F5] Coordinate derivatives and their total order use [[math:def-ck-and-multi-index-notation-in-several-variables]]. Every component here is smooth, hence $C^2$, so [[math:thm-clairaut-schwarz-mixed-partials]] gives $\partial_a\partial_bh=\partial_b\partial_ah$ for every component $h$ and all coordinate indices.

## Proof

**Given:** The stationary Lorentzian data, smooth scalar and one-form, vanishing Lie derivatives and nonzero point in the Statement.

**Goal:** Construct the stated stationary chart and identify its two-jet data.

1.1 Apply [F3] at $x$ to arrange $T=\partial_t$ in a product chart contained in $U$. The components of this vector field are constant, so all terms $\partial_aT^b$ in [F4] vanish. Applying its covariant-tensor formula to $g$ and $W_0$, and its scalar formula to $\psi$, gives $(\mathcal L_Tg)_{ab}=\partial_tg_{ab}$, $(\mathcal L_TW_0)_a=\partial_t(W_0)_a$ and $\mathcal L_T\psi=\partial_t\psi$. By [F1] and the stationary-field hypotheses in [F2], these expressions vanish throughout the chart. Thus the components are independent of the product coordinate $t$. [given, F1, F2, F3, F4]

2.1 For each component function $h$, differentiate the identity $\partial_t h=0$ from step 1.1 in any coordinate direction to obtain $\partial_a\partial_t h=0$. By [F5], $\partial_t\partial_a h=\partial_a\partial_t h=0$ as well, including $a=0$. The same mixed-partial identity makes all second derivatives symmetric. Consequently the component values, first derivatives and second derivatives through total order two are precisely the stationary two-jet data described in the Statement, with all time-containing derivatives zero. The construction required only $T_x\ne0$, so applies also at nonzero null or spacelike points. [F5, step 1.1] ∎
