---
title: Axial averaging and positive boost at the pole
status: published
research_item: pthm-axial-averaging-positive-boost
dependency_level: 38
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 28–29, proof of Proposition 5.1, final paragraphs
      statement: At the axial pole the article averages a future normal over the axial
        circle and obtains the positive normal boost identity.
      hypotheses: The regular stationary vacuum construction, nontrivial stationary
        field on the bifurcation sphere, maximal original exterior section and
        mass-one normalization.
      reading_limits: Read the frozen article text at the cited passage for
        attribution; the article is not used as a proof premise.
---

PDF p. 28: ` Proof of Proposition 5.1, final paragraphs `; PDF p. 29: ` Proof of Proposition 5.1, final paragraphs `

## Prerequisites

- [post-stationary-vacuum-model](item-post-stationary-vacuum-model)
- [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime)
- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [def-harrison-normalization](item-def-harrison-normalization)
- [def-harrison-one-form](item-def-harrison-one-form)
- [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)
- [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)
- [pthm-horizon-invariant-one-form](item-pthm-horizon-invariant-one-form)
- [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)
- [pthm-pole-ernst-normal-derivative](item-pthm-pole-ernst-normal-derivative)


## Statement

Adopt the stationary vacuum model and regular non-degenerate stationary construction, with maximal original exterior section, ADM mass one and $T|_S\not\equiv0$, where $S$ is the bifurcation sphere. Let $K=T+\Omega_H Z$ and the pole $p\in S$ be the supplied local fields and common zero, with $Z$ generating the normalized circle action and $K$ having positive normal boost rate $\kappa$. Use the supplied normalized Ernst potential $\sigma$, limiting Harrison metric $g_0$, and $d_0=|1-\sigma(p)|^2>0$. Write $\nabla$ and $\nabla^{(0)}$ for the Levi–Civita connections of $g$ and $g_0$.

There is a smooth future $g_0$-unit timelike normal field $\bar n$ along $S$, invariant under the local circle action. Its Lie bracket with $Z$ vanishes along $S$; at $p$, $\nabla^{(0)}_{\bar n}Z=\nabla^{(0)}_Z\bar n=0$. If $\bar\nu$ is the outward $g_0$-unit spacelike normal at $p$ orthogonal to $\bar n$, then

$$2\operatorname{Re}\frac{1}{1-\sigma(p)}-1=g(\nabla_{\bar n}T,\bar\nu)(p)=\frac4{d_0}g_0(\nabla^{(0)}_{\bar n}K,\bar\nu)(p)=\frac{4\kappa}{d_0}>0.$$

Here outward selects the normal direction into the exterior; invariance of a field along $S$ means equivariance under the differential of the circle flow.

## Facts & Assumptions

[A1] The model, regular construction, maximality, nontriviality and mass normalization are as stated. [post-stationary-vacuum-model](item-post-stationary-vacuum-model) [def-regular-stationary-vacuum-spacetime](item-def-regular-stationary-vacuum-spacetime) [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data) [def-harrison-normalization](item-def-harrison-normalization)

[F1] The local fields satisfy $K=T+\Omega_HZ$, $K|_S=0$, $T(p)=Z(p)=0$ and the normal action of $\nabla K$ is the boost taking a future unit normal to $\kappa$ times its outward orthogonal unit normal, with $\kappa>0$. The circle preserves $S$. [pthm-local-hawking-circle-fields](item-pthm-local-hawking-circle-fields)

[F2] The supplied $\sigma$ and $W_0$ are invariant under $Z$, and $g_0=(D_0/4)A_0^*g$, where $D_0=|1-\sigma|^2$ and $A_0v=v+D_0^{-1}W_0(v)T$. The limiting metric makes $S$ spacelike. [pthm-horizon-invariant-one-form](item-pthm-horizon-invariant-one-form) [def-harrison-one-form](item-def-harrison-one-form) [pthm-bifurcate-horizon-preservation](item-pthm-bifurcate-horizon-preservation)

[F3] The circle-average construction turns a supplied smooth future timelike normal field along an invariant surface into a smooth invariant future unit normal. [def-circle-action-and-invariant-normal-data](item-def-circle-action-and-invariant-normal-data)

[F4] At $p$, $g_0=(d_0/4)g$, $d_0>0$, and for every future/outward $g_0$-orthonormal normal pair $(n,\nu)$, $g(\nabla_nT,\nu)=2\operatorname{Re}(1/(1-\sigma(p)))-1$ and $\nabla^{(0)}_nT=\nabla_nT$. [pthm-pole-ernst-normal-derivative](item-pthm-pole-ernst-normal-derivative)

## Proof

**Given:** The model, fields, limiting metric and pole in the Statement.

**Goal:** Construct the invariant normal and prove the displayed positive identity.

1.1 The circle flow preserves $g$ and $T$, and by [F2] preserves $D_0$ and $W_0$; hence it preserves $g_0$. It also preserves $S$ and, being connected to the identity, preserves the future cone. The original spacelike section supplies a smooth future $g$-unit normal $n$ along $S$. Because $T$ is tangent to $S$, $A_0$ maps $TS$ to itself. Thus $A_0^{-1}n$ is $g_0$-normal to $S$ and is timelike by the pullback formula. Choose its future sign continuously using the supplied Harrison family, which joins $g_0$ to the original metric. Applying [F3] gives the smooth invariant future $g_0$-unit normal $\bar n$. [F1, F2, F3, A1]

2.1 Differentiate the equivariance of $\bar n$ along the circle flow. This gives $[Z,\bar n]=0$ along $S$, with the bracket computed using any local extension of $\bar n$; it is independent of the extension because $Z$ is tangent to $S$. At the fixed point $p$, $\nabla^{(0)}_Z\bar n=0$. Torsion-freeness then gives $\nabla^{(0)}_{\bar n}Z=0$ there as well. [F1, step 1.1]

3.1 Since $K(p)=0$, the difference of the two connections applied to $K$ vanishes at $p$. By [F4] the two metrics are positive scalar multiples there, so their normal planes and future/outward orientations agree. The boost in [F1] consequently gives $\nabla^{(0)}_{\bar n}K=\kappa\bar\nu$ at $p$. The relation $K=T+\Omega_HZ$ and step 2.1 give $\nabla^{(0)}_{\bar n}T=\nabla^{(0)}_{\bar n}K$ there. [F1, F4, step 2.1]

4.1 Apply [F4] to $(\bar n,\bar\nu)$ and use $g=(4/d_0)g_0$ at $p$. Step 3.1 yields the displayed chain of equalities. Its last term is strictly positive because both $\kappa$ and $d_0$ are positive. This proves the claim. [F4, step 3.1, algebra] ∎

## Source notes

The article is cited for attribution. The argument uses the declared completed suppliers, including the independently authored pole identities, rather than the article's assertion as a premise.
