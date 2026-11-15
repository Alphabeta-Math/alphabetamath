---
id: def-author-fd2999663761-temporal-angle-data
title: Temporal normal angle and compact positive-height portions
kind: definition
status: published
origin: pipeline
domain: mathematics
deps:
  - def-spacelike-maximal-hypersurface-data
  - def-causal-exterior-and-boundary-data
  - math:def-axiom-of-choice
  - physics:def-gr-inverse-metric-and-musical-isomorphisms
  - math:def-riemannian-gradient-of-a-smooth-function
  - math:def-riemannian-divergence
  - math:def-laplace-beltrami-operator-as-trace-of-the-hessian
  - math:thm-compactness-under-continuous-maps
dependency_roles:
  def-spacelike-maximal-hypersurface-data: mathematical-premise
  def-causal-exterior-and-boundary-data: mathematical-premise
  math:def-axiom-of-choice: mathematical-premise
  physics:def-gr-inverse-metric-and-musical-isomorphisms: mathematical-premise
  math:def-riemannian-gradient-of-a-smooth-function: mathematical-premise
  math:def-riemannian-divergence: mathematical-premise
  math:def-laplace-beltrami-operator-as-trace-of-the-hessian: mathematical-premise
  math:thm-compactness-under-continuous-maps: mathematical-premise
provenance:
  statement: ai-generated
  proof: not-applicable
dependency_level: 2
---

## Definition

Work in ZFC on a smooth time-oriented Lorentzian four-manifold of signature $(-,+,+,+)$. Let $g$ be its metric and $\Sigma$ a smooth embedded spacelike maximal hypersurface, smooth up to its actual boundary $\partial\Sigma$, with future unit normal $n$. Maximal means its induced mean curvature vanishes.

Fix a compact ambient set $Q$, allowed to be empty, and let $\tau$ be a smooth real function on an open neighborhood of $\Sigma\cup Q$. A compact positive-height portion is the entire set $P=\Sigma\cap\{\tau\ge0\}$, assumed compact and contained in $Q$; it is not a clipping of $\Sigma$ by $Q$. Require the metric gradient of $\tau$ to be past-directed timelike on an open neighborhood of $P$. On that temporal neighborhood put $\alpha=\sqrt{-g^{-1}(d\tau,d\tau)}>0$ and $V=-\alpha^{-1}\operatorname{grad}_g\tau$, where $\operatorname{grad}_g\tau$ is characterized by $g(\operatorname{grad}_g\tau,Y)=d\tau(Y)$ for every ambient tangent vector $Y$. Along the hypersurface in that neighborhood put $v=-g(n,V)$. Thus $V$ is future unit timelike and $v$ is the temporal normal angle.

Write $h=g|_{T\Sigma}$. For a real function $f$ smooth on an open subset of $\Sigma$, smooth up to any actual boundary there, write $\nabla_\Sigma f=\operatorname{grad}_h f$ and $\Delta_\Sigma f=\operatorname{div}_h(\nabla_\Sigma f)$ for the positive-trace Laplacian. If $f$ is an ambient function, these operators act on its restriction to $\Sigma$. At actual boundary points use the smooth one-sided extensions of these local operators.

Fix an arbitrary real exponent $\mu>0$. For nonempty $Q$ set $T=\max_{q\in Q}\max\{\tau(q),0\}$, and for empty $Q$ set $T=0$. Set $B=\sup_{\partial\Sigma\cap\{\tau>0\}}\tau^\mu v$, with the supremum zero for an empty set. At positive height only the actual hypersurface boundary contributes a boundary term.

## Definition references

[[def-spacelike-maximal-hypersurface-data]]

[[def-causal-exterior-and-boundary-data]]

[[math:def-axiom-of-choice]]

[[physics:def-gr-inverse-metric-and-musical-isomorphisms]]

[[math:def-riemannian-gradient-of-a-smooth-function]]

[[math:def-riemannian-divergence]]

[[math:def-laplace-beltrami-operator-as-trace-of-the-hessian]]

[[math:thm-compactness-under-continuous-maps]]

## Justification

The normal and induced metric are those of the spacelike hypersurface interface; the temporal orientation is that of the causal interface. The inverse metric and metric dual of $d\tau$ have the musical-isomorphism convention. Dividing a past timelike gradient by its positive Lorentzian norm and reversing its sign gives a future unit timelike $V$. In a Lorentz-orthonormal frame with time axis $V$, the unit equation for the future $n$ gives $v=\sqrt{1+|n^{\mathrm{space}}|^2}\ge1$.

The Riemannian gradient and divergence suppliers define the two intrinsic operators. The Laplace–Beltrami supplier identifies their composition with the positive metric trace of the Hessian and supplies the stated one-sided boundary convention. The gradient's inverse-metric formula also extends smoothly in boundary half-charts, since $h$ stays positive definite and $f$ is smooth up to the boundary; its values there are determined by its values in the interior.

For nonempty $Q$, the continuous function $q\mapsto\max\{\tau(q),0\}$ attains a finite maximum by the compactness supplier's extreme-value assertion. If $Q$ is empty, so is $P$, and the explicit convention defines $T$. On nonempty compact $P$, smoothness up to the actual boundary makes $v$ continuous and bounded for each individual hypersurface, again by that extreme-value assertion. Since $\mu>0$, the weight $\tau^\mu$ is continuous on $P$, with value zero at zero height, and $0\le\tau\le T$ there. Thus the actual boundary supremum is finite, and its empty-set convention covers empty $P$ as well. No uniform bound along a sequence is assumed.
