---
title: A variable-time flow through a fixed boundary has the boosted unit normal
status: published
research_item: lem-author-840894718169-fixed-boundary-flow-normal-boost
dependency_level: 2
---

## Prerequisites

- [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)
- [physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)
- [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)
- [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)
- [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)
- [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)


## Statement

Let a smooth Killing field $K$ vanish on a compact spacelike boundary surface $S$ of a reference spacelike section in a smooth time-oriented Lorentzian four-manifold $(M,g)$ of signature $(-,+,+,+)$. Let $\bar n$ be the future unit reference normal and $\bar\nu$ the exterior unit boundary normal. Fix $\kappa>0$ and impose the signed normal-boost convention $\nabla_{\bar n}K=\kappa\bar\nu$ and $\nabla_{\bar\nu}K=\kappa\bar n$ on $S$, where $\nabla$ is the Levi–Civita connection. Let $\phi^K:\mathcal D\to M$ be a local flow of $K$. On a reference neighborhood of $S$, let $u$ be smooth down to $S$, with $(u(x),x)\in\mathcal D$, and suppose the variable-time map $\Phi(x)=\phi_{u(x)}^K(x)$ is a smooth embedding with spacelike image, the candidate section. Then on $S$ its future unit normal is $n=\cosh(\kappa u)\bar n+\sinh(\kappa u)\bar\nu$. In particular $-g(n,\bar n)=\cosh(\kappa u)$. The derivative of $u$ contributes nothing to the boundary tangent map because $K=0$ there.

## Statement references

[def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[physics:def-gr-killing-field](https://alphabetamath.cc/physics/item/def-gr-killing-field)

[lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)

[math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)

## Facts & Assumptions

[F1] A smooth embedded spacelike section has its unique future unit normal, including at its smooth spacelike boundary. [def-spacelike-maximal-hypersurface-data](item-def-spacelike-maximal-hypersurface-data)

[F2] With the stated signed infinitesimal boost in the ordered normal basis $(\bar n,\bar\nu)$, the Killing flow fixes $S$ pointwise, its differential is the identity on $TS$, and its normal-plane differential is the boost with off-diagonal entries $\sinh(\kappa t)$. [lem-killing-normal-boost-and-invariant-tensors](item-lem-killing-normal-boost-and-invariant-tensors)

[F3] The derivative of a smooth flow with respect to its time is its generating field at the image point. [math:def-local-and-global-flow](https://alphabetamath.cc/item/def-local-and-global-flow)

[F4] For composable smooth maps $F,G$, the differential satisfies $d(G\circ F)_p=dG_{F(p)}\circ dF_p$. [math:thm-chain-rule-for-differentials-of-smooth-maps](https://alphabetamath.cc/item/thm-chain-rule-for-differentials-of-smooth-maps)

[F5] A smooth embedding between manifolds with boundary is an immersion and a homeomorphism onto its image; its differential on the full tangent spaces is injective at every point, including boundary points. [math:def-smooth-immersion-and-embedding-for-manifolds-with-boundary](https://alphabetamath.cc/item/def-smooth-immersion-and-embedding-for-manifolds-with-boundary)

## Proof

**Given:** The reference section, its boundary $S$, the signed boost hypotheses, and the smooth variable-time embedding with spacelike image in the Statement.

**Goal:** Establish the boundary normal formula, the angle identity, and independence of height derivatives in the boundary tangent map.

1.1 At $p\in S$, the flow fixes $p$. Apply the chain rule to $x\mapsto(u(x),x)\mapsto\phi_{u(x)}^K(x)$. For every vector $X$ in the reference tangent space at $p$, this gives $d\Phi_p(X)=d\phi_{u(p)}^K|_p(X)+du_p(X)K_{\phi_{u(p)}^K(p)}=d\phi_{u(p)}^K|_p(X)$, since $\phi_{u(p)}^K(p)=p$ and $K_p=0$. At the boundary this calculation is made using smooth local extensions in boundary charts; smoothness down to $S$ ensures that the resulting differentials agree with those of the given maps. Thus the candidate tangent hyperplane is the image of the reference tangent hyperplane under $d\phi_{u(p)}^K|_p$, independently of all height derivatives. [F1, F2, F3, F4, F5]

2.1 The identity action on $T_pS$ and the normal-plane boost preserve $g_p$, so $d\phi_{u(p)}^K|_p$ is a linear isometry. Its image of $\bar n_p$ is $\cosh(\kappa u(p))\bar n_p+\sinh(\kappa u(p))\bar\nu_p$, a future unit timelike vector because $\cosh(\kappa u(p))>0$ and $\cosh^2(\kappa u(p))-\sinh^2(\kappa u(p))=1$. By step 1.1 this vector is orthogonal to the candidate tangent hyperplane, hence is its unique future unit normal. Pairing with $\bar n_p$ and using $g(\bar n_p,\bar n_p)=-1$ and $g(\bar\nu_p,\bar n_p)=0$ gives $-g(n_p,\bar n_p)=\cosh(\kappa u(p))$. [F1, F2, step 1.1, algebra] ∎
