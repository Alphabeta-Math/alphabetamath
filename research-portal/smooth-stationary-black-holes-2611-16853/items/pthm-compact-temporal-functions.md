---
id: pthm-compact-temporal-functions
title: Local causality and temporal functions on compact tubes
kind: physics-theorem
status: published
origin: pipeline
domain: physics
deps:
  - pthm-compact-timelike-length-bound
  - thm-compact-temporal-function-input
  - def-causal-exterior-and-boundary-data
  - def-stationary-lorentzian-data
  - def-harrison-one-form-family
  - pthm-harrison-electrovacuum
  - math:def-axiom-of-choice
  - math:def-riemannian-metric-and-riemannian-manifold
  - math:cor-every-smooth-manifold-admits-a-riemannian-metric
  - math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric
  - physics:lem-gr-causal-curve-calculus
  - physics:lem-gr-temporal-functions-and-time-functions
  - math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions
  - math:thm-lipschitz-images-of-null-sets-in-rn-are-null
dependency_roles:
  pthm-compact-timelike-length-bound: physical-result
  thm-compact-temporal-function-input: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  def-stationary-lorentzian-data: mathematical-premise
  def-harrison-one-form-family: mathematical-premise
  pthm-harrison-electrovacuum: physical-result
  math:def-axiom-of-choice: mathematical-premise
  math:def-riemannian-metric-and-riemannian-manifold: mathematical-premise
  math:cor-every-smooth-manifold-admits-a-riemannian-metric: mathematical-premise
  math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric: mathematical-premise
  physics:lem-gr-causal-curve-calculus: mathematical-premise
  physics:lem-gr-temporal-functions-and-time-functions: mathematical-premise
  math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions: mathematical-premise
  math:thm-lipschitz-images-of-null-sets-in-rn-are-null: mathematical-premise
provenance:
  statement: ai-altered
  proof: ai-generated
proof_strategy: direct
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF page 20, §3.2.3
      attribution: The article uses a compact-tube length bound to exclude a trapped
        inextendible causal curve and obtains a temporal function near the
        smaller tube that remains temporal for the approximating metrics on that
        tube.
      hypotheses: The stationary vacuum construction and candidate-section estimates
        used in §3.2.3, with positive limiting parameter and nested compact
        tubes.
      reading_limits: Historical reading note retained from the current source; this
        maintenance revision claims no fresh article or external full-text
        reading. Read the frozen extracted article passage. This reference
        attributes the claim and is not used as a proof premise.
physical_scope: Conditional geometric deduction in the classical stationary
  vacuum model and its Harrison family; the candidate maximal sections and their
  estimates are assumed, and no observation is asserted.
dependency_level: 17
---

## Statement

Assume all hypotheses and notation of [[pthm-compact-timelike-length-bound]], including the candidate-section and uniform-estimate hypotheses, $q_j\to q_*\in[\delta,1]$, and the compact tubes $Q\subset\widetilde Q^\circ\Subset\mathcal E$. The metrics $g_{q_j}$ and $g_{q_*}$ are the corresponding time-oriented Harrison metrics. A future causal curve is a locally Lipschitz curve with nonzero future causal tangent almost everywhere; inextendibility means inextendibility as an unparametrized causal curve in $\mathcal E$.

There is an open neighborhood $O$ of $Q$ and a smooth function $\tau_*$ on $O$ whose $g_{q_*}$-gradient is past timelike. On $Q$, the $g_{q_j}$-gradient of the same function is past timelike for all sufficiently large $j$. No inextendible $g_{q_*}$-causal curve is contained in $Q$. Consequently, if such a curve were contained in $Q$, it could be deformed to future timelike curves in $\widetilde Q$ of arbitrarily large $g_{q_*}$-length; this conditional is vacuous because its antecedent is impossible.

## Facts & Assumptions

[F1] The compact-tube bound supplies a common finite upper bound for the $g_{q_*}$-length of every future Lipschitz curve in $\widetilde Q$ whose tangent has a curve-dependent strictly negative upper bound for its squared norm. It applies under the full hypotheses named in the Statement. [[pthm-compact-timelike-length-bound]]

[F2] The compact temporal-function input applies to a $C^2$ time-oriented Lorentz metric on an open set when every compact subset has a uniform length bound for all future Lipschitz curves with such a curve-dependent strict timelikeness bound. It yields a smooth past-timelike gradient near any chosen compact subset and its persistence on compact sets under sufficiently small uniform metric perturbations. [[thm-compact-temporal-function-input]]

[F3] The selected Harrison family is smooth in the spacetime and parameter variables, so $g_{q_j}\to g_{q_*}$ uniformly on compact sets. The time orientations are chosen consistently for sufficiently close parameters. [[def-harrison-one-form-family]] [[pthm-harrison-electrovacuum]] [[def-stationary-lorentzian-data]]

[F4] A past-timelike gradient pairs positively with every nonzero future causal vector. Its composite with a future causal curve is locally absolutely continuous, has derivative equal to the covector applied to the velocity almost everywhere, and is strictly increasing. The future causal cones and time orientation are those of the stated Lorentzian data. The causal-curve calculus applies also to the locally Lipschitz subclass used here. [[physics:lem-gr-temporal-functions-and-time-functions]] [[physics:lem-gr-causal-curve-calculus]] [[def-causal-exterior-and-boundary-data]] [[def-stationary-lorentzian-data]]

[A1] The inherited stationary-data convention is ZFC. In particular, countable choice supplies an auxiliary smooth Riemannian metric, and countable choice and dependent choice supply the absolutely continuous calculus used below; these are already included assumptions, not additional physical hypotheses. [[def-stationary-lorentzian-data]] [[math:def-axiom-of-choice]]

[F5] A smooth Riemannian metric $h$ exists on the smooth manifold $\mathcal E$ under [A1]. Write $|v|_h=\sqrt{h(v,v)}$. On each compact coordinate ball there is a constant $D<\infty$ with $|dx(v)|\le D|v|_h$. [[math:def-riemannian-metric-and-riemannian-manifold]] [[math:cor-every-smooth-manifold-admits-a-riemannian-metric]] [[math:lem-local-comparison-of-a-riemannian-metric-with-the-euclidean-metric]]

[F6] An absolutely continuous scalar function on a compact interval equals its initial value plus the integral of its almost-everywhere derivative. Apply this also componentwise in a chart. [[math:thm-fundamental-theorem-of-calculus-for-absolutely-continuous-functions]]

[F7] A Lipschitz map of the real line sends null sets to null sets. For a locally Lipschitz interval map, apply this on a countable compact exhaustion, extending each compact-interval restriction constantly outside its endpoints. This extension is Lipschitz with the same bound. [[math:thm-lipschitz-images-of-null-sets-in-rn-are-null]]

## Proof

**Given:** The hypotheses, sequence and nested tubes in the Statement.

**Goal:** Construct the temporal function, establish its persistence on $Q$, and exclude causal curves imprisoned in $Q$.

1.1 Put $B=\widetilde Q^\circ$. Every compact $C\subset B$ lies in $\widetilde Q$, so the single finite bound in [F1] bounds every eligible curve in $C$, with the curve class and quantifiers required by [F2]. Apply [F2] to $g_{q_*}$ on $B$ and the compact set $Q$. This gives an open $O\subset B$ containing $Q$ and a smooth $\tau_*$ with past-timelike $g_{q_*}$-gradient. [F1, F2]

2.1 Since $Q$ is compact and $g_{q_j}\to g_{q_*}$ uniformly there, the perturbation conclusion of [F2], with the consistent orientation in [F3], makes $\operatorname{grad}_{g_{q_j}}\tau_*$ past timelike on $Q$ for all sufficiently large $j$. [F2, F3, step 1.1]

2.2 Use [A1] and [F5] to choose $h$. If $Q$ is empty all conclusions hold, so suppose it is nonempty. The $h$-unit future causal vectors based at $Q$ form a compact set: in a finite cover by relatively compact coordinate trivializations, the unit condition gives bounded fiber coordinates and the unit and future causal conditions are closed. By [F4], the continuous function $v\mapsto d\tau_*(v)$ is strictly positive there, so it has a minimum $c>0$. By positive homogeneity, $d\tau_*(v)\ge c|v|_h$ for every future causal $v$ over $Q$. For a future causal $\gamma:I\to Q$, put $f=\tau_*\circ\gamma$. By [F4] and [F6], for any $a<b$ in $I$ one has $c\int_a^b|\dot\gamma(t)|_h\,dt\le f(b)-f(a)$. Since $f$ is increasing and bounded on $I$, it has finite endpoint limits, and the integral of $|\dot\gamma|_h$ has arbitrarily small tails at either end. This argument uses the original parametrization, without invoking an arc-length theorem. [A1, F4, F5, F6, step 1.1]

3.1 Here is the endpoint argument in local coordinates. Let $\beta=\sup I$ and let $p\in Q$ be a cluster point of $\gamma(t)$ as $t\to\beta$; such a point exists by compactness (the closures in $Q$ of the nested nonempty tails have nonempty intersection). Choose coordinates $x$ centered at $p$ whose image contains a closed ball of radius $2r>0$ lying in $O$, and take $D$ as in [F5] on this ball. Choose $a$ sufficiently late that $|x(\gamma(a))|<r/2$ and $D\int_a^\beta|\dot\gamma(t)|_h\,dt<r/2$. Until a first exit from the radius-$r$ ball, [F6] gives $|x(\gamma(t))-x(\gamma(a))|\le D\int_a^t|\dot\gamma|_h<r/2$, which forbids that exit. The entire tail therefore stays in that ball. The same inequality on any subinterval of the tail makes its coordinates Cauchy at $\beta$. Their limit is $x(p)$, since $p$ was a cluster point. Thus $\gamma(t)\to p\in Q$. Reversing the parameter gives the past endpoint as well. No completeness assumption on $h$ is used. [F5, F6, step 2.2]

4.1 For completeness, these endpoints give extensions in the stated locally Lipschitz causal class, with its unparametrized meaning. The function $f$ is continuous and strictly increasing by [F4], and thus has an increasing continuous inverse on its image $J=f(I)$. Reparametrize the future tail by $u=f(t)$ and write $\eta(u)=\gamma(f^{-1}(u))$. For any two parameters on the tail, the chart estimate and step 2.2 give $|x(\eta(v))-x(\eta(u))|\le(D/c)(v-u)$ when $u<v$. Thus $\eta$ extends Lipschitz continuously to the finite endpoint $u_+=\lim_{t\to\beta}f(t)$ with value $p$. To verify its causal orientation, discard the null set of original parameters where $\gamma$ or $f$ is not differentiable, their chain rule fails, or $\dot\gamma$ is not nonzero future causal. The map $f$ is locally Lipschitz, since $\gamma$ is locally Lipschitz and $\tau_*$ is smooth; [F7] makes the image of this exceptional set null. At every remaining parameter, $f'=d\tau_*(\dot\gamma)\ge c|\dot\gamma|_h>0$. The elementary inverse difference quotient gives $(f^{-1})'(f(t))=1/f'(t)$, and hence $\eta'(f(t))=\dot\gamma(t)/f'(t)$, a positive multiple of a nonzero future causal vector. A short smooth future timelike segment from $p$ exists: in a chart a straight line with an initially future timelike tangent stays future timelike for sufficiently small positive time by openness of the timelike cone. Adjoin it at $u_+$; both pieces are Lipschitz in the endpoint chart, and their common endpoint gives a Lipschitz concatenation. Off the single junction the velocities are nonzero future causal almost everywhere, so this extends the unparametrized future causal curve in $\mathcal E$. The past extension is identical with a past endpoint and a future-directed segment arriving there. [F4, F5, F7, step 2.2, step 3.1]

5.1 Consequently no causal curve contained in $Q$ is inextendible in $\mathcal E$. The conditional deformation assertion follows because its antecedent is false. Together with the temporal function of step 1.1 and its persistence from step 2.1 this proves all stated conclusions. [step 1.1, step 2.1, step 3.1, step 4.1] ∎

## Source notes

The article describes a timelike-deformation contradiction before obtaining the temporal function. Here the completed compact-length temporal input is applied first; non-imprisonment then proves the same conditional deformation statement by contradiction, without asserting a separate construction of the deformations.
