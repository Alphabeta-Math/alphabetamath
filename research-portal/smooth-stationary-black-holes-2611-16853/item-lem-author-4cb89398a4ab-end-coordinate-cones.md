---
title: Coordinate cones and the separate stationary generator
status: published
research_item: lem-author-4cb89398a4ab-end-coordinate-cones
dependency_level: 3
---

## Prerequisites

- [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)
- [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)


## Statement

For an end satisfying the exact asymptotically stationary end contract, the coordinate vector $\partial_t$ is uniformly timelike on $O_1$, and every nonzero vector tangent to a coordinate level set of $t$ in $O_1$ is spacelike. The separate hypothesis $g(T,T)<-C^{-1}$ on $\Sigma_1$ concerns the complete stationary generator $T$, not merely $\partial_t$. If a second Killing field $K$ and a Killing horizon $H$ for $K$ are supplied, meaning that $H$ is a smooth embedded null hypersurface and $K$ is tangent and normal on its nonempty dense nonzero part, the end conditions do not imply that $K$ is timelike on $\Sigma_1$ or $O_1$. This non-implication holds even if $K$ is complete.

## Statement references

[def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)

[def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

## Facts & Assumptions

[F1] The end contract supplies $g_{00}<-C^{-1}$, $g_{ij}Z^iZ^j\ge C^{-1}|Z|^2$ and the separate uniform timelikeness condition for $T$ on $\Sigma_1$. It also supplies the smooth time-oriented Lorentzian and causal conventions, the acausal hypersurface and its smooth end/remainder realization, the remaining coordinate estimates on $O_1$, and the completeness and asymptotics of $T$. [def-author-4cb89398a4ab-asymptotically-stationary-end](item-def-author-4cb89398a4ab-asymptotically-stationary-end)

[F2] A Killing horizon for a specified Killing field $K$ is a smooth embedded null hypersurface on whose nonempty dense nonzero-generator part $K$ is tangent and normal. The null normal line is the radical of the induced metric. This definition asserts no relation between $K$ and the stationary field $T$, and imposes no field equation. [def-bifurcate-killing-horizon-data](item-def-bifurcate-killing-horizon-data)

## Proof

**Given:** An end and coordinates satisfying [F1]; any additional horizon and field use [F2].

**Goal:** Prove the coordinate-cone conclusions and exhibit an end with a complete horizon-normal field that is not timelike on that end.

1.1 Since $g(\partial_t,\partial_t)=g_{00}<-C^{-1}$ on $O_1$, the coordinate time vector is uniformly timelike there. [F1]

1.2 A nonzero tangent vector to $t=\mathrm{constant}$ has the form $v=\sum_iZ^i\partial_{x^i}$ with $Z\ne0$, so $g(v,v)=g_{ij}Z^iZ^j\ge C^{-1}|Z|^2>0$. The bound on $g(T,T)$ is separately imposed in end clause (3), on $\Sigma_1$. [F1]

1.3 For the countermodel take $M=\mathbb R^4$ with its standard smooth structure and orientation, $g=-dt^2+(dx^1)^2+(dx^2)^2+(dx^3)^2$, time orientation $N=\partial_t$, and $T=\partial_t$. Set $\Sigma=\{t=0\}$, $\Sigma_1=\{t=0,\ |x|>1\}$, $\Sigma'=\{t=0,\ |x|\le1\}$ and $O_1=\{(t,x):|x|>1\}$. These are the standard embedded hyperplane, open exterior and closed ball, with their usual smooth structures. For a future causal vector $(a,b)$, the metric and orientation give $a\ge|b|$ and $a>0$. Thus along every nonconstant future causal curve the locally absolutely continuous coordinate $t$ is strictly increasing, by integrating its positive almost-everywhere derivative on any compact parameter subinterval. Consequently $\Sigma$ is acausal. [F1, construct]

2.1 Take $R_1=1$, $E=\{z:|z|>1\}$, $\overline E=\{z:|z|\ge1\}$, $e(z)=(0,z)$, $j(z)=(0,z)$ and $h=j|_{\partial\overline E}$. The sphere $S=\partial\Sigma'=\{t=0,|x|=1\}$ is connected; $h$ is a diffeomorphism onto $S$, $j(\overline E)\cap\Sigma'=S$ and $j(\overline E)\cup\Sigma'=\Sigma$. With $C=2$, $k=2$, $\alpha=\lambda=1$, all metric differences, positive-order derivatives and Hölder differences in end clause (1) vanish. Its remaining bounds are $-1<-1/2$ and $|Z|^2\ge|Z|^2/2$, and $r>1$ throughout $O_1$. The complete flow $\phi_u(t,x)=(t+u,x)$ preserves $g$, so $T$ is Killing, $g(T,T)=-1<-1/2$, and the asymptotics hold with $A=1$ and zero error. This verifies all three end clauses. [F1, step 1.3, construct]

3.1 Define $K=\partial_t+\partial_{x^1}$ and $H=\{t=x^1\}$. Its flow $\psi_u(t,x^1,x^2,x^3)=(t+u,x^1+u,x^2,x^3)$ is defined for all real $u$ and preserves the constant metric, so $K$ is a complete Killing field distinct from $T$. The map $(s,y,z)\mapsto(s,s,y,z)$ smoothly embeds $\mathbb R^3$ onto $H$; the induced form is $dy^2+dz^2$, with radical spanned by the everywhere nonzero tangent vector $K$. Equivalently, $g(K,\cdot)=-dt+dx^1$ annihilates $TH$. Thus $H$ is a Killing horizon for $K$ under [F2]. But $g(K,K)=-1+1=0$ everywhere, including on $\Sigma_1$ and $O_1$. The fully verified end therefore does not force even pointwise timelikeness of a separate complete horizon-normal field, while retaining all coordinate and stationary bounds. [F1, F2, step 1.1, step 1.2, step 1.3, step 2.1] ∎
