---
title: Causal curves from a common chronological boundary obey two barriers
status: draft
research_item: lem-author-ca4ffba327b3-causal-boundary-barriers
dependency_level: 0
---

## Prerequisites

- [physics:def-gr-future-and-past-sets](https://alphabetamath.cc/physics/item/def-gr-future-and-past-sets)
- [physics:lem-gr-push-up-rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)
- [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)
- [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)
- [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)
- [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)
- [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)


## Statement

Work in ZFC. Let $(M,g,N)$ be a time-oriented smooth Lorentzian four-manifold, let $E\subseteq M$, and let $p,q\in M$. Use the locally absolutely continuous causal and timelike curve conventions for the relations $\le$ and $\ll$ and the chronological sets $I^\pm$. Let $G=I^-(E)$, $F_+=I^+(E)$, and $p\in\partial G\cap\partial F_+$. If $p\le q$, then $q\notin G$ and $q\in\overline{F_+}$. If $p\ll q$, then $q\notin\overline G$ and $q\in F_+$. Here $\le$ allows equality and denotes future causal reachability; $\ll$ denotes future timelike reachability. Boundaries and closures are taken in the manifold topology of $M$. The time-reversed conclusions hold for the causal and chronological past of $p$.

## Statement references

[physics:def-gr-future-and-past-sets](https://alphabetamath.cc/physics/item/def-gr-future-and-past-sets)

[Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness)

[math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

[physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects)

[physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

## Facts & Assumptions

[F0] The field $N$ is smooth with $g(N,N)<0$; a timelike vector $v$ is future-directed when $g(v,N)<0$. The relations $\le$, $\ll$ and sets $I^\pm(E)$ have the causal-curve, timelike-curve and union definitions, with equality permitted in $\le$. [physics:def-gr-smooth-lorentzian-objects](https://alphabetamath.cc/physics/item/def-gr-smooth-lorentzian-objects) [physics:def-gr-causal-curves-and-reachability](https://alphabetamath.cc/physics/item/def-gr-causal-curves-and-reachability)

[F1] The chronological sets are open past/future sets. [physics:def-gr-future-and-past-sets](https://alphabetamath.cc/physics/item/def-gr-future-and-past-sets)

[F2] Chronology is open in its endpoints, and a causal segment followed by a timelike segment, or vice versa, gives a chronological relation. [physics:lem-gr-chronology-openness](https://alphabetamath.cc/physics/item/lem-gr-chronology-openness) [Push-up rule](https://alphabetamath.cc/physics/item/lem-gr-push-up-rule)

[F3] For any $x\in M$ and $v\in T_xM$ there is a smooth geodesic $\gamma$ on an open interval about $0$ with $\gamma(0)=x$ and $\gamma'(0)=v$. Only this local existence and smoothness are used here. [physics:thm-gr-local-geodesics-and-exponential-map](https://alphabetamath.cc/physics/item/thm-gr-local-geodesics-and-exponential-map)

[A1] Use the ZFC convention, including the choice assumptions inherited through these causal interfaces. [math:def-axiom-of-choice](https://alphabetamath.cc/item/def-axiom-of-choice)

## Proof

**Given:** The data and hypotheses in the Statement.

**Goal:** Establish the stated conclusions under exactly those hypotheses.

1.1 Fix $x\in M$. Apply [F3] with initial vector $v=N_x$. At $t=0$ both $g(\gamma'(t),\gamma'(t))$ and $g(\gamma'(t),N_{\gamma(t)})$ equal $g_x(N_x,N_x)<0$. Smoothness and continuity make both negative for $0\le t\le\epsilon$ for some $\epsilon>0$. Thus for $0<t\le\epsilon$ the smooth segment $\gamma|_{[0,t]}$ is future timelike in the curve convention [F0], and $x\ll\gamma(t)$ while $\gamma(t)\to x$ as $t\downarrow0$. The choice convention [A1] covers the inherited supplier hypotheses; this construction uses the specified vector $N_x$ and no additional choice of vectors. [F0, F3, A1]

2.1 If $p\le q$ and $q\in G$, some $e\in E$ satisfies $q\ll e$. Push-up gives $p\ll e$, contrary to $p\in\partial G$ and openness of $G$. Thus $q\notin G$. For any $q'\gg q$, push-up gives $p\ll q'$. Since $p\in\overline{F_+}$ and $I^-(q')$ is an open neighborhood of $p$, choose $f\in F_+\cap I^-(q')$. Its future-set property puts $q'\in F_+$. Apply step 1.1 at $q$: the endpoints $q'=\gamma(t)$ lie in $F_+$ and approach $q$, so $q\in\overline{F_+}$. [F0, F1, F2, step 1.1]

3.1 If $p\ll q$, the same open-endpoint argument puts $q\in F_+$: the open neighborhood $I^-(q)$ of $p\in\overline{F_+}$ meets $F_+$, and its future-set property applies. If $q\in\overline G$, openness of $I^+(p)$ would give $g\in G$ with $p\ll g$, and the past-set property would put $p\in G$, a contradiction. Hence $q\notin\overline G$. Replacing $N$ by $-N$ reverses the relations and interchanges $G$ with $F_+$; the same arguments prove the past statements. [F0, F1, F2, step 2.1] ∎
