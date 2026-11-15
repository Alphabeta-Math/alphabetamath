---
id: lem-author-9a15bef58785-affine-generator-acceleration
title: Affine generator profiles give constant signed acceleration
kind: lemma
status: draft
origin: pipeline
domain: mathematics
deps:
  - def-stationary-lorentzian-data
  - physics:def-gr-metric-selected-connection
  - def-bifurcate-killing-horizon-data
  - lem-author-9a15bef58785-affine-generator-zero-locus
  - math:def-embedded-submanifold-and-slice-chart
  - math:def-action-of-a-vector-field-on-smooth-functions
dependency_roles:
  def-stationary-lorentzian-data: mathematical-premise
  physics:def-gr-metric-selected-connection: mathematical-premise
  def-bifurcate-killing-horizon-data: mathematical-premise
  lem-author-9a15bef58785-affine-generator-zero-locus: mathematical-premise
  math:def-embedded-submanifold-and-slice-chart: mathematical-premise
  math:def-action-of-a-vector-field-on-smooth-functions: mathematical-premise
provenance:
  statement: ai-generated
  proof: ai-generated
proof_strategy: direct
dependency_level: 2
---

## Statement

In the preceding generator-profile setting, suppose $L$ is affinely geodesic, meaning $\nabla_LL=0$ along $H$. If $K=csL$ with constant $c\ne0$ and $L(s)=1$, then $\nabla_KK=cK$ along $H$. For a pair of branches with profiles $K=csL_+$ on $H_+$ and $K=-ctL_-$ on $H_-$, where $L_+(s)=L_-(t)=1$ and both generators are affine, the signed coefficients are $c$ and $-c$, respectively. At the bifurcation section the acceleration equation alone does not determine a coefficient.

For a smooth vector field $X$ tangent to $H$ and a smooth vector field $Y$ along $H$ with values in $TM|_H$, write $\nabla_XY=(\nabla_{\widetilde X}\widetilde Y)|_H$, using smooth local ambient extensions $\widetilde X,\widetilde Y$. Local extensions exist, and this expression is independent of their choice, as proved below. For $f\in C^\infty(H)$, $X(f)$ denotes the action of the tangent field on the smooth function on $H$. These conventions apply separately to both branches, including their bifurcation section.

## Statement references

[[def-stationary-lorentzian-data]]

[[physics:def-gr-metric-selected-connection]]

[[def-bifurcate-killing-horizon-data]]

[[lem-author-9a15bef58785-affine-generator-zero-locus]]

[[math:def-embedded-submanifold-and-slice-chart]]

[[math:def-action-of-a-vector-field-on-smooth-functions]]

## Facts & Assumptions

[F1] The metric-selected connection is function-linear in its direction argument and obeys $\nabla_X(fY)=X(f)Y+f\nabla_XY$ for ambient fields and functions. The ambient smooth data and horizon conventions specify a smooth embedded hypersurface $H$. [[physics:def-gr-metric-selected-connection]] [[def-stationary-lorentzian-data]] [[def-bifurcate-killing-horizon-data]]

[F2] The generator profile has zero locus exactly its zero-parameter section. [[lem-author-9a15bef58785-affine-generator-zero-locus]]

[F3] A smooth embedded hypersurface admits local slice coordinates in which it is a coordinate hyperplane. A tangent field on the hypersurface acts on its smooth functions as a derivation. [[math:def-embedded-submanifold-and-slice-chart]] [[math:def-action-of-a-vector-field-on-smooth-functions]]

## Proof

**Given:** The hypotheses and data in the Statement.

**Goal:** Establish well-definedness of the restricted derivative and the stated acceleration conclusions.

1.1 Fix $p\in H$. By [F3], shrink a slice chart to a product coordinate box with coordinates $(x^1,x^2,x^3,r)$ and $H=\{r=0\}$ in this box; put $x^4=r$. The smooth coordinate coefficients of fields along $H$, and of functions on $H$, extend smoothly by making them independent of $r$. Thus the local ambient extensions in the Statement exist. Define smooth functions $\Gamma^a{}_{ij}$ in this chart by $\nabla_{\partial_i}\partial_j=\Gamma^a{}_{ij}\partial_a$. Expanding the ambient connection rules in [F1] gives $(\nabla_{\widetilde X}\widetilde Y)^a=\widetilde X^i\partial_i\widetilde Y^a+\Gamma^a{}_{ij}\widetilde X^i\widetilde Y^j$, with indices from $1$ to $4$. [given, F1, F3]

2.1 If two extensions of $Y$ differ by $A$, then $A^a(x^1,x^2,x^3,0)=0$, so $\partial_iA^a=0$ on $H$ for $i=1,2,3$. Since $X$ is tangent, $\widetilde X^4|_H=0$. The formula in step 1.1 therefore gives $(\nabla_{\widetilde X}A)|_H=0$. Changing an extension of $X$ leaves its values on $H$ fixed, so the same formula gives no change in the derivative there either. The local definitions agree on overlaps because each equals restriction of the same intrinsic ambient connection applied to any local extensions. They consequently define a smooth field along $H$, independent of chart and extensions. Extending a scalar $f$ in the same way gives $\widetilde X(\widetilde f)|_H=X(f)$ by [F3]; restricting the ambient rules therefore proves $\nabla_{fX}Y=f\nabla_XY$ and $\nabla_X(fY)=X(f)Y+f\nabla_XY$ along $H$. [F1, F3, step 1.1]

3.1 Using the now well-defined restricted derivative and its rules, $\nabla_{csL}(csL)=cs\{cL(s)L+cs\nabla_LL\}=c^2sL=cK$. This calculation is valid everywhere on $H$, including $s=0$, using the given $L(s)=1$ and affine condition $\nabla_LL=0$. [given, step 2.1]

4.1 Replacing $c$ by $-c$ gives the coefficient $-c$ for the other branch. Off the section the coefficients are unique because $K\ne0$ by [F2]. On the section, $K=0$ makes both sides zero for any assigned scalar; the constant branch values are limits of the values off the section, not values deduced from this zero equation. [F2, step 2.1, step 3.1] ∎
