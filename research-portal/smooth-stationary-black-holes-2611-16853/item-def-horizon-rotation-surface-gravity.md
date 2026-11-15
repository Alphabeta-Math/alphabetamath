---
title: Rotation, surface gravity and horizon degeneracy
status: draft
research_item: def-horizon-rotation-surface-gravity
dependency_level: 1
sources:
  references:
    - title: The uniqueness of smooth stationary black holes
      url: https://arxiv.org/abs/2611.16853v1
      locator: PDF pp. 2–5, §§1.1 and 1.3
      statement: The article calls a horizon non-rotating when the stationary field is
        tangent to its null generators and rotating when this fails somewhere.
        It calls the constant nonnegative coefficient in the horizon-generator
        equation surface gravity, with positive value non-degenerate and zero
        value degenerate; it describes the bifurcation sphere and multiple
        horizon components.
      hypotheses: The horizon and generator are those in the article's discussion; its
        regular spacetime definition separately assumes smooth transverse future
        and past horizons meeting in a two-sphere.
      reading_limits: Read the frozen article text at the cited passages. This
        reference attributes the terminology and does not establish existence or
        constancy of the generator coefficient.
---

PDF p. 2: ` §1.1, rotation and surface gravity `; PDF p. 5: ` §1.3, degeneracy and multiple black holes `

## Prerequisites

- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)


## Definition

Let $(M,g)$ be a smooth time-oriented Lorentzian four-manifold with Levi–Civita connection $\nabla$, and let $T$ be a stationary Killing field: $\mathcal L_Tg=0$ and $T$ is timelike on a specified nonempty open region. Let $H$ be a smooth null hypersurface. Its null normal line at $p$ is the radical of $g|_{T_pH}$, namely the vectors in $T_pH$ orthogonal to all of $T_pH$; its integral curves, where specified, are the null generators. The horizon is **non-rotating relative to $T$** if $T_p$ lies in this line at every $p\in H$, and **rotating relative to $T$** if this condition fails somewhere. The zero vector belongs to the line.

For a Killing horizon of a specified Killing field $K$, put $H_*=\{p\in H:K_p\ne0\}$ and suppose it is nonempty and dense, with $K$ tangent and normal to $H$ on $H_*$. Its signed surface-gravity function is the unique smooth scalar $\kappa_H$ on $H_*$ satisfying $d(g(K,K))=-2\kappa_H K^\flat$, where $K^\flat=g(K,\cdot)$; equivalently $\nabla_KK=\kappa_H K$. Fixing $K$ fixes its scale. Under a constant rescaling $K\mapsto aK$, $a\ne0$, the signed function becomes $a\kappa_H$.

In the article's convention, suppose the chosen future-horizon generator has a constant coefficient $\kappa_H=\kappa\ge0$. This number is its surface gravity: the horizon is **non-degenerate** if $\kappa>0$ and **degenerate** if $\kappa=0$. Constancy, nonnegativity and the existence of the particular generator are additional properties, not consequences of these definitions. At a point where $K=0$, the equation $\nabla_KK=\kappa K$ by itself determines no value of $\kappa$.

A bifurcate Killing horizon consists locally of two distinct smooth null Killing horizons $H_+$ and $H_-$ of the same field $K$, intersecting transversely in a smooth spacelike two-surface $S$ on which $K=0$; spacelike means that the induced metric on $S$ is positive definite. If $S$ is diffeomorphic to the two-sphere, call it a **bifurcation sphere**. A surface-gravity value on $S$ is specified by the common value only when the branch functions extend smoothly there and agree. In the article's terminology, **multiple black holes** means that the horizon has several connected components.

## Definition references

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

## Facts & Assumptions

[F1] The horizon interface defines the null normal line, the rotation condition relative to $T$, and the signed surface-gravity function on the nonzero-generator part of a Killing horizon. It also gives the equivalent acceleration equation and constant-rescaling rule. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

[F2] The bifurcate-horizon interface specifies the transverse branches, spacelike intersection, vanishing field and the qualification needed to assign a common surface-gravity value at the intersection. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

## Justification

**Given:** The data and hypotheses stated in the Definition.

**Goal:** Show that the terminology and the stated numerical conventions are well-defined under those hypotheses.

1.1 The null normal line and the pointwise membership condition give complementary rotation alternatives. On the nonzero part of the specified Killing horizon, the horizon interface supplies a unique smooth signed coefficient and identifies its covector and acceleration equations. Its constant-rescaling rule shows why the numerical coefficient depends on the chosen scale of $K$. [given, F1]

2.1 When the coefficient is assumed constant and nonnegative, exactly one of $\kappa=0$ and $\kappa>0$ holds, so the two degeneracy labels are unambiguous. At a zero of $K$, both sides of the acceleration equation vanish, so that equation alone selects no coefficient. The bifurcation and extension conditions give the stated intersection terminology without asserting existence of an extension; the sphere and connected-component conditions are additional classifications of the supplied sets. [given, F2, step 1.1] ∎

## Source notes

The article attributes the existence of its horizon generator and the constant nonnegative coefficient to rigidity results. The present definition records the convention conditional on those properties; it does not prove them.
